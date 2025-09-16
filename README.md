# Amazon-Reviews-LLM-Binary-Classification

In this repository we use `distilbert-base-uncased` for binary classification (positive/negative) of amazon reviews. The model is a smaller, faster, and lighter distilled version of Google's original BERT architecture. As an encoder-only model, it is ideal for language understanding tasks such as text classification. We train the model in a jupyter notebook and save the weights, the we make inferences loading the trained model in other notebook.

## Environmet Setup

Create an Anaconda environment using `python=3.10`. Navigate to the root folder of the project and install requeriments

```bash
pip install -r requeriments.txt
```

## Install PyTORCH

If your machine has a CUDA compatible GPU, install:

```bash
pip install torch==2.8.0 torchvision==0.23.0 torchaudio==2.8.0 --index-url https://download.pytorch.org/whl/cu126
```
Otherwise, install the versions for CPU

```bash
pip install torch==2.8.0 torchvision==0.23.0 torchaudio==2.8.0
```

## Exploratory Data Analysis (EDA) and Training

The full dataset consists of 4 million reviews. We utilize two randomly sampled subsets: 50,000 rows for training and 10,000 for validation. Before training the model, we perform exploratory data analysis, which includes examining the distribution of positive and negative reviews, counting the number of words per review, and identifying the most frequent single tokens (unigrams) and token pairs (bigrams).

## Testing the Model

We evaluate the model in a new 1,000 randomly sampled subset. Here we show the confussion matrix.







