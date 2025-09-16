# Amazon-Reviews-LLM-Binary-Classification

In this repository we use `distilbert-base-uncased`. This model is a smaller, faster, and lighter distilled version of Google's original BERT architecture. As an encoder-only model, it is ideal for language understanding tasks such as text classification.

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
