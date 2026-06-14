# CryptoCast: Multi-Horizon Bitcoin Price Forecasting Using Deep Learning

## Project Overview

CryptoCast is a deep learning-based Bitcoin forecasting system that predicts future Bitcoin prices using historical market data.

The project compares multiple deep learning architectures:

* CNN (Convolutional Neural Network)
* RNN (Recurrent Neural Network)
* LSTM (Long Short-Term Memory)
* Transformer

The best-performing model was further extended for multi-horizon forecasting (1-Day, 3-Day, and 7-Day predictions).

## Dataset Features

* Date
* Price
* Open
* High
* Low
* Volume
* Change %

## Technologies Used

* Python
* Pandas
* NumPy
* TensorFlow / Keras
* Scikit-learn
* Matplotlib

## Workflow

1. Data Cleaning and Preprocessing
2. Feature Scaling using MinMaxScaler
3. Sequence Generation (60-Day Window)
4. CNN Model Training
5. RNN Model Training
6. LSTM Model Training
7. Transformer Model Training
8. Model Evaluation
9. Multi-Horizon Forecasting

## Model Performance

| Model       | MAE      | RMSE     | MAPE   |
| ----------- | -------- | -------- | ------ |
| CNN         | 2452.12  | 2944.27  | 7.02%  |
| RNN         | 5003.30  | 7071.32  | 11.74% |
| LSTM        | 2012.50  | 2843.97  | 5.45%  |
| Transformer | 19489.82 | 22900.54 | 51.72% |

## Key Findings

* LSTM achieved the best forecasting performance.
* CNN showed competitive short-term forecasting ability.
* Transformer underperformed due to limited dataset size.
* Forecasting error increased with prediction horizon.

## Future Improvements

* Hyperparameter tuning
* Advanced Transformer architectures
* Additional market indicators
* Real-time prediction dashboard
