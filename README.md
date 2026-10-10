# Aspect-Based-Sentiment-Analysis-through-Fine-tuning-DeBERTA-v3-base-model

In this project, we fine-tune a Transformer-based encoder model - DeBERTa-v3-base - for Aspect Sentiment Classification (ASC) purpose. This is augmented with a structured error analysis (confusion matrix, per-domain accuracy, aspect-count wise accuracy and saving row-level incorrect predictions for manual tagging) and an experiment testing whether a class-weighted loss function improves minority-class performance.

The dataset used here is Kaggle's SemEval-2014 dataset containing laptop reviews and restaurant reviews. For more flavour, we have combined these 2 separate datasets into one such that the data we have worked with has both kinds of reviews (6051 rows of data). 

We have chosen DeBERTa-v3-base model for its disentangled attention mechanism, well-suited to distinguishing which part of a sentence a given aspect’s sentiment belongs to, and its replaced-token-detection pretraining, known to transfer well to classification tasks.
