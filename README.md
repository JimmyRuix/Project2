##CMPE 401 Project 2: Time Series Modeling with Deep Learning
Time Series Classification (Transformer) & Time Series Forecasting (LSTM)

1. Project Overview
This project reproduces and improves two official Keras deep learning examples for time series tasks:
Time series classification using Transformer
Time series forecasting using LSTM
2. Datasets
FordA Dataset: Time series classification for engine sensor fault detection
Jena Climate Dataset: Time series forecasting for temperature prediction

3. Baseline Results
Transformer	Time Series Classification	Test Accuracy: 81.59%
LSTM	Time Series Forecasting	Test MAE: 0.28

4. Improvements (3 Valid Modifications)
I improved the Transformer classification model with 3 changes:
Changed num_transformer_blocks from 4 to 2
Adjusted learning rate from 1e-4 to 1e-3 for faster training
Modified batch_size (64 → 32) and patience (10 → 30) for stable training

5. Answers to Required Questions
Q1: Which model did you find easier to understand and why?
The LSTM model is easier to understand. It uses a simple recurrent structure to process sequential data step by step. The Transformer relies on self-attention and positional encoding, which are more abstract and complex for beginners.
Q2: What improvement did you try, and what did you learn from it?
I adjusted the Transformer’s depth, learning rate, batch size and early stopping patience. I learned that hyperparameters strongly affect training stability. Small datasets can make Transformer training unstable, while LSTM is more robust for basic time series tasks.

6. Conclusion
I successfully reproduced both baseline models, implemented three improvements, and compared performance. This project helped me understand the difference between time series classification/forecasting and the behavior of Transformer vs. LSTM on sequential data.
