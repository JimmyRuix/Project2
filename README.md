##CMPE 401 Project 2: Time Series Modeling with Deep Learning

Time Series Classification (Transformer) & Time Series Forecasting (LSTM)
1. Project Overview
This project reproduces, improves, and benchmarks two official Keras deep learning models for time series tasks:
Time series classification using Transformer (FordA Dataset)
Time series forecasting using LSTM (Jena Climate Dataset)
Completed work:
Reproduce baseline results for both models
Implement 3 meaningful improvements on Transformer
Implement 2 meaningful improvements on LSTM
Evaluate performance and record metrics
Answer required project questions

2. Datasets
FordA Dataset: Time series classification for engine sensor fault detection
Jena Climate Dataset: Time series forecasting for temperature prediction

3. Model Improvements
Transformer (3 improvements)
Changed num_transformer_blocks from 4 to 2
Adjusted learning rate from 1e-4 to 1e-3 for stable training
Modified batch_size (64 → 32) and EarlyStopping patience (10 → 30)
LSTM (2 improvements)
Changed LSTM hidden units from 32 to 64
Increased training epochs from 10 to 15

4. Experimental Results
Transformer	Time-Series Classification	Test Accuracy: 51.59%
LSTM	Time-Series Forecasting	Test MAE: 0.28

5. Answers to Required Questions
Q1: Which model did you find easier to understand and why?
The LSTM model is much easier to understand. It uses a simple recurrent structure to process sequential data step-by-step, with clear and intuitive logic. The Transformer relies on self-attention and positional encoding, which are more abstract and complex for beginners.
Q2: What improvement did you try, and what did you learn from it?
I modified model structure, learning rate, batch size, training epochs, and early stopping settings. I learned that hyperparameters directly affect training stability and model performance. LSTM is more robust for small time-series datasets, while Transformer training is more sensitive to parameter settings.

6. Conclusion
I successfully reproduced both baseline models, implemented three improvements, and compared performance. This project helped me understand the difference between time series classification/forecasting and the behavior of Transformer vs. LSTM on sequential data.
