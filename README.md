# Time Series Analysis

A collection of Jupyter notebooks exploring time series forecasting across two domains: **stock price prediction** and **temperature forecasting**. Each notebook experiments with multiple modeling approaches and evaluates performance using standard metrics.

---

## Notebooks

### 1. Stock Forecasting
Forecasts stock prices using classical statistical and deep learning models.

**Models:**
- **ARIMA / SARIMA** — autoregressive integrated moving average models for capturing trend and seasonality
- **LSTM / GRU** — recurrent neural networks for learning long-range temporal dependencies

**Evaluation:** RMSE, MAPE, forecast vs. actual plots

---

### 2. Temperature Analysis *(in progress)*
Forecasts temperature data with a progression from simple baselines to statistical models.

**Models:**
- **Naive** — last observed value as the forecast
- **Historic Average** — mean of all historical observations
- **Window Average** — mean over a rolling window
- **Seasonal Naive** — repeats the value from the same season in the prior period
- **ARIMA / SARIMA** — statistical models capturing trend and seasonal structure

**Evaluation:** RMSE, MAE 

---

## Metrics

| Metric | Description |
|--------|-------------|
| RMSE | Root Mean Squared Error — penalizes large errors |
| MAE | Mean Absolute Error — average magnitude of errors |
| MAPE | Mean Absolute Percentage Error — scale-independent accuracy |

---

## Requirements

```bash
pip install numpy pandas matplotlib statsmodels torch scikit-learn
```

---

## Repository Structure

```
Time-Series-Analysis/
├── stock_forecasting.ipynb       # ARIMA/SARIMA + LSTM/GRU stock models
└── temperature_analysis.ipynb    # Baseline + ARIMA temperature models (WIP)
```
