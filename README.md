# Advanced-Time-Series-Forecasting-with-Deep-Learning-and-Attention-Mechanisms
#Project Description: Energy consumption forecasting using LSTM-GRU with attention


## Project Overview
This project implements a hybrid LSTM–GRU model with Bahdanau Attention to forecast
industrial energy consumption using multivariate time-series data.

## Dataset
- KwhConsumptionBlower78_1.csv
- KwhConsumptionBlower78_2.csv
- KwhConsumptionBlower78_3.csv

## Methodology
- Data preprocessing with outlier handling and MinMax scaling
- Sliding window sequence generation (window size = 24)
- Hybrid LSTM–GRU architecture with attention
- Baseline LSTM comparison
- Evaluation using RMSE, MAE, and MAPE
- Attention-based interpretability analysis

## How to Run
1. Open the notebook in Google Colab
2. Upload the dataset CSV files
3. Run all cells sequentially

## Results
The attention-based model outperforms the baseline LSTM and provides interpretable
attention weights highlighting important historical time steps.

## Author
Aishwarya 

