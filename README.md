# deep-learning-for-sentiment-analysis using LSTM AND CNN models

This repository showcases a comparative study and implementation of **Convolutional Neural Networks (CNN)** and **Long Short-Term Memory Networks (LSTM)** for sentiment analysis on product reviews. The project evaluates both models on three datasets: **Yelp**, **IMDB**, and **Amazon**, consisting of balanced positive and negative reviews.

## Overview

The datasets contain a total of 1000 reviews each, with 500 positive and 500 negative reviews. To ensure a focused evaluation:
- Reviews rated as **1 (negative)** are labeled as `0`.
- Reviews rated as **5 (positive)** are labeled as `1`.
- Neutral reviews are excluded.


## Model Architectures

### 1. Convolutional Neural Network (CNN)
CNNs excel in capturing local features and patterns from text data.  
**Architecture**:
- **Embedding Layer**: Converts words into dense word vectors.
- **Convolutional Layer**: With 300 feature maps and **ReLU activation**.
- **Max Pooling**: To downsample and extract prominent features.
- **Dropout**: To prevent overfitting.
- **Fully Connected Dense Layer**: With **Softmax activation** for binary classification.


### 2. Long Short-Term Memory (LSTM)
LSTMs are designed for sequential data, making them effective for understanding context in lengthy reviews.  
**Architecture**:
- **Embedding Layer**: Converts text into meaningful word vectors.
- **Bidirectional LSTM Layer**: Captures dependencies from past and future contexts.
- **Dense Layer**: With **ReLU activation** for intermediate processing.
- **Output Layer**: With **Sigmoid activation** for binary classification.

- CNNs showed high training accuracy but struggled with generalization on the test set.
- LSTMs outperformed CNNs in test accuracy, demonstrating their ability to capture sentiment in reviews effectively.

