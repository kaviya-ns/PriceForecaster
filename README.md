# PriceForecaster

**Gold price forecasting with time-series and machine-learning models.**

PriceForecaster scrapes historical gold prices, explores trends and seasonality, and compares classical time-series models against machine-learning regressors to forecast future prices.

![Python](https://img.shields.io/badge/Python-3670A0?logo=python&logoColor=ffdd54) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikit-learn&logoColor=white) ![statsmodels](https://img.shields.io/badge/statsmodels-4051B5) ![XGBoost](https://img.shields.io/badge/XGBoost-189FDD) ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)

---

## What's inside

1. **Data collection** — web scraping with `requests-html` + BeautifulSoup
2. **EDA** — trend plots, ACF/PACF, seasonality analysis
3. **Time-series models** — ARIMA, SARIMAX, and Auto-ARIMA (`pmdarima`)
4. **ML regressors** — Linear Regression, KNN, XGBoost, HistGradientBoosting (with decision-tree visualisation)
5. **Evaluation** — MAE, MSE, RMSE and R² side by side

## Results

| Model | Target | Result |
|---|---|---|
| Linear Regression | Gold price | **R² = 0.98** |
| ARIMA | First-differenced evening price | MAE 24.6, RMSE 36.4 |
| XGBoost | Gold price | MAE 108.6, RMSE 171.9 |
| KNN | Gold price | MAE 117.3, RMSE 188.4 |

Full comparison, residual diagnostics and plots in the notebook.

## Run it

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels pmdarima xgboost requests-html beautifulsoup4 tabulate graphviz
```

Open `Gold_price_forecasting_using_time_series_data.ipynb` (Jupyter or Google Colab) and run all cells.

---

*Built as the Machine Learning course package project.*
