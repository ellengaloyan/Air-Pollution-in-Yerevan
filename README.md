
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
