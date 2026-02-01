Advanced Time Series Forecasting with Deep Learning and Attention

1. Dataset Overview

Energy consumption (kWh) from industrial blower systems

3 CSV files merged chronologically

~3,600 observations

Irregular timestamps corrected via sorting

2. Preprocessing

IQR-based outlier clipping

MinMax scaling (0–1)

Multivariate feature creation:

Hour of day

Day of week

Month

3. Model Architecture

Primary Model

LSTM → GRU → Bahdanau Attention

Attention improves interpretability by weighting historical time steps

Baseline

Single-layer LSTM

4. Hyperparameters
Parameter	Values
Window Size	24
LSTM Units	64
GRU Units	32
Attention Units	32
Optimizer	Adam
LR Scheduler	ReduceLROnPlateau
5. Results
Model	RMSE	MAE	MAPE
LSTM + GRU + Attention	0.061	0.044	6.9%
Baseline LSTM	0.083	0.062	10.8%
6. Attention Analysis

Strong emphasis on recent time steps

Demonstrates short-term energy dependency

Provides explainability absent in baseline models

7. Conclusion

The attention-based hybrid model:

Outperforms standard LSTM

Provides interpretable forecasting

Is suitable for production energy monitoring systems
