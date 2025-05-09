# Air Pollution Forecasting in Yerevan

This project analyzes and forecasts PM2.5 air pollution levels in Yerevan using both classical statistical models and modern machine learning and deep learning methods, including LSTM and Monte Carlo simulations. The data includes historical pollution levels and derived weather and seasonal features, with predictions at both daily and weekly levels.

---

## 📁 Repository Structure

```
Air-Pollution-in-Yerevan/
├── Analysis/
│   ├── TS_daily_data.ipynb               # Time Series analysis for daily data
│   ├── TS_weekly_data.ipynb              # Time Series analysis for weekly data
│   ├── lstm.ipynb                        # LSTM model for daily PM2.5 prediction
│   ├── monte_carlo_mortality.ipynb       # Monte Carlo mortality simulations
│   ├── data_analysis.ipynb               # EDA and feature engineering
├── Data/
│   ├── Final data/
│   │   ├── df_daily.csv                  # Cleaned and processed daily data
│   │   ├── df_weekly.csv                 # Cleaned and processed weekly data
│   ├── Raw data/
│   │   ├── Daily data/                   # Raw PM2.5 data (hourly & daily)
│   │   └── Weekly data/                  # Aggregated weekly data
├── Error comparisons/
│   ├── daily_error.csv                   # RMSE and error metrics for daily models
│   ├── error_weekly.csv                  # RMSE and error metrics for weekly models
├── Forecasted values/
│   ├── final_forecast_results_daily.csv  # Predicted PM2.5 values (daily)
│   ├── forecast_comparison_weekly.csv    # Predicted PM2.5 values (weekly)
├── Air_pollution.pdf                     # Project report (PDF)
```


---

## 🧠 Models Used

- **SARIMA / SARIMAX** – for classical time-series baseline.
- **XGBoost, SVR, Random Forest** – for traditional machine learning baselines.
- **LSTM, Seq2Seq, BiLSTM** – for deep learning approaches to temporal modeling.
- **Temporal Fusion Transformer (TFT)** – for high-capacity attention-based forecasting.
- **Monte Carlo Simulation** – for scenario-based health impact estimation.

---

## 📈 Key Results

- Best **daily** forecast: **XGBoost (RMSE = 1.49)**
- Best **deep learning** model: **BiLSTM (RMSE = 16.63)**
- Weekly models performed poorly (e.g., SVR RMSE = 14.00), leading to a focus on daily predictions.

---

## 📦 Requirements

- Python 3.8+
- Jupyter Notebook
- `tensorflow`, `scikit-learn`, `xgboost`, `pytorch-forecasting`, `matplotlib`, `pandas`, `numpy`, etc.

You can install all dependencies using:

```bash
pip install -r requirements.txt
