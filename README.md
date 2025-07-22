# ⛵ Time Series Forecasting of Slave Migration Across the Atlantic (ARIMA)

This project uses **time series and spectral analysis** to study the annual number of enslaved people transported by British ships across the Atlantic. The dataset reflects voyage trends over a historical time period and models future trajectories using ARIMA modelling techniques.

---

## 🎯 Objectives

- Analyze long-term and short-term patterns in slave embarkation counts
- Remove linear trend and evaluate residual stationarity
- Fit AR and ARIMA models (ARIMA(3,0,0))
- Assess autocorrelation, model fit, and forecast reliability
- Produce 5-year forecasts with 95% confidence intervals

---

## 📊 Dataset

The original dataset contains annual records of estimated embarkation of enslaved people. Due to sensitivity and licensing, it is not shared here. A **simulated dataset** may be added for demonstration purposes.

**Key variables**:
- `Year`: Time variable (chronological)
- `Num`: Estimated number of enslaved people embarked

---

## 📈 Methodology

- **Detrending** using linear regression
- **Residual analysis**
- **ACF/PACF** plots for AR order selection
- **Yule-Walker equations** to fit AR models
- **Periodogram analysis** to explore dominant frequencies
- **ARIMA model fitting** with log-likelihood and AIC evaluation
- **Forecast generation** for the years 1808–1812

---

## 🔢 Model Summary

**Final model**: ARIMA(3,0,0)  
**Coefficients**:
- AR1: 0.8812  
- AR2: 0.0242  
- AR3: 0.0709  
- σ² (error variance): 33,177,667  
- AIC: 3114.84

---

## 🔮 Forecast (1808–1812)

| Year | Forecast | Lower CI | Upper CI |
|------|----------|----------|----------|
| 1808 | 35,081   | 23,791   | 46,371   |
| 1809 | 34,498   | 19,451   | 49,545   |
| 1810 | 33,809   | 16,256   | 51,363   |
| 1811 | 33,114   | 13,385   | 52,843   |
| 1812 | 32,444   | 10,816   | 54,071   |

---

## 📁 Project Structure

| File | Description |
|------|-------------|
| `scripts/slave_migration_timeseries.R` | R script for full ARIMA analysis |
| `report/slave_migration_analysis_report.pdf` | Full academic report |
| `data/simulated_slave_counts.csv` | Placeholder CSV for reproducibility (optional) |

---

## 👩‍💻 Tools Used

- R: `arima()`, `ar()`, `acf()`, `pacf()`, `predict()`
- Forecasting & spectral analysis libraries
- RMarkdown and visualisation

---

## 🧠 Insights

- The ARIMA(3,0,0) model effectively captured underlying autocorrelation in slave transport patterns.
- Periodograms revealed cyclical fluctuations.
- Forecasts suggest a decreasing trend post-1808, though confidence intervals widen due to historical uncertainties.

---

## ✍️ Author

**Shekhina Mary Jebaraj**  
MSc Data Science (Distinction), University of Leeds  
📍 Leeds, UK  
📧 shekhinamaryjebaraj@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/shekhinamaryjebaraj)

---

## 🔗 Citation

> Jebaraj, S.M. (2023). *Time Series Analysis of Slave Migration Across the Atlantic*, University of Leeds MSc Data Science Project.
