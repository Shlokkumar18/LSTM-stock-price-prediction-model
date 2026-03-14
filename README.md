# LSTM-Based Stock Price Forecasting

## Overview

This project implements a **time-series forecasting model using LSTM (Long Short-Term Memory) neural networks** to predict future stock prices based on historical data.

The goal of this project is to demonstrate an **end-to-end machine learning pipeline**, including data preprocessing, feature engineering, sequence generation, model training, evaluation, and visualization.

The model learns patterns from historical price data and predicts **future price movements using deep learning techniques**.

---

## Technologies Used

* Python
* TensorFlow / Keras
* Pandas
* NumPy
* Matplotlib
* scikit-learn

---

## Project Pipeline

### 1️⃣ Data Collection

Historical stock price data was used including:

* Open
* High
* Low
* Close
* Volume

---

### 2️⃣ Feature Engineering

Additional statistical indicators were created to help the model capture market behavior:

* 30-day Moving Average
* Rolling Standard Deviation (Volatility)

These features provide information about **trend and volatility**.

---

### 3️⃣ Data Preprocessing

* Missing values handled
* Features scaled using **MinMaxScaler**
* Dataset converted into **time-series sequences**

Input format for LSTM:

```
(samples, time_steps, features)
```

Example:

```
(2000, 90, 3)
```

---

### 4️⃣ Model Architecture

The LSTM network consists of:

* LSTM layer (64 units)
* Dropout layer
* LSTM layer (32 units)
* Dense layer
* Output layer (price prediction)

The model learns **temporal dependencies in stock price movements**.

---

### 5️⃣ Model Evaluation

Performance was evaluated using:

* MAE (Mean Absolute Error)
* RMSE (Root Mean Squared Error)
* MAPE (Mean Absolute Percentage Error)
* R² Score

Example results:

```
MAE:  $3.96
RMSE: $5.31
MAPE: 1.96%
R²:   0.973
```

---

### 6️⃣ Forecasting

The trained model is used to generate **future price predictions** using recursive forecasting.

The project also visualizes:

* Historical stock prices
* Model predictions
* Multi-day forecasts

---

## Visualization

The model output is visualized to compare:

* Actual prices
* Predicted prices

This helps understand how well the model captures market trends.

---

## Key Learnings

This project demonstrates:

* Time-series forecasting with deep learning
* Feature engineering for financial data
* LSTM sequence modeling
* Model evaluation for regression tasks
* Visualization of predictions

---

## Future Improvements

Possible improvements include:

* Adding technical indicators (RSI, MACD, Bollinger Bands)
* Walk-forward validation
* Trading strategy simulation
* Transformer-based time-series models

---

## Disclaimer

This project is intended **for educational purposes only**.
It does not provide financial advice or trading recommendations.

---

## Author

Machine Learning & Embedded Systems Enthusiast
Focused on combining **AI with real-world engineering systems**.
