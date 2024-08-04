# Argument-detection

This project focuses on training a RoBERTa model using PyTorch to detect whether an input sentence is an argument or not. The dataset used for this project is `sentence_full.csv`.

## Overview 
The goal of this project is to create a model capable of determining whether a given sentence constitutes an argument. This can be beneficial in various applications such as debate analysis, sentiment analysis, and automated essay scoring.

## Dataset
The dataset used in this project is sentence_full.csv. It contains sentences labeled as either arguments or non-arguments.

- sentence_full.csv: This file contains two columns: sentence and label. The sentence column contains the text, and the label column contains binary labels (1 for argument, 0 for non-argument).

## Model

We utilize the RoBERTa model, a robustly optimized BERT pretraining approach, as the base for our classifier. RoBERTa has proven effective in various NLP tasks, making it a suitable choice for argument detection.

## Training

The model was trained using PyTorch. Key training details include:

- Optimizer: AdamW
- Learning Rate: 2e-5
- Batch Size: 16
- Epochs: 3
We fine-tuned the pre-trained RoBERTa model on our dataset to adapt it to the specific task of argument detection.

## Evaluation

The performance of the model was evaluated using accuracy, precision, recall, and F1-score. These metrics help in understanding the effectiveness of the model in identifying arguments.
