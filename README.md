# 🌦️ WeatherStockPredict-AI

**WeatherStockPredict-AI** explores the intriguing connection between **New York’s weather** and the **Dow Jones Industrial Average (DJI)**. Using time series analysis and machine learning, it investigates how atmospheric factors like temperature and cloud cover might correlate with daily stock market behavior.

---

## 🚀 Overview

This project merges two data streams - historical weather data from LaGuardia Airport and DJI stock data, and applies a complete data science workflow:
- Cleans and resamples weather observations to hourly intervals.
- Averages pre-market weather conditions (8-9 AM) for each trading day.
- Constructs stationary time series using differencing and log transformations.
- Tests stationarity using **ADF** and **KPSS** methods.
- Performs seasonal adjustments using polynomial fitting.
- Sets the stage for predictive modeling using features derived from both datasets.

---

## 🧠 Tech Stack

**Languages & Tools**
- Python 3  
- NumPy · Pandas · SciPy  
- Statsmodels (ADF, KPSS, seasonal diagnostics)  
- Scikit-learn (RandomForestRegressor, TimeSeriesSplit)  
- Matplotlib · Seaborn for visualization  
- tqdm for progress tracking  

---

## 📊 Key Features

- 🌡️ Weather-Market Data Integration  
  Merges climate and economic data at compatible daily frequencies.

- 📈 Stationarity & Seasonal Analysis  
  Log-differencing, ADF/KPSS testing, and polynomial seasonal adjustments.

- 🧮 Feature Engineering  
  Extracts temperature anomalies and log returns for robust predictive features.

- 🤖 Modeling Foundation  
  Framework supports Random Forests or other regressors for forecasting DJI log returns.

---

## 🧾 How to Run

```bash
# Clone this repository
git clone https://github.com/<your-username>/WeatherStockPredict-AI.git
cd WeatherStockPredict-AI

# Install dependencies
pip install -r requirements.txt

# Run the analysis
python WeatherStockPredict_AI.py
```
📈 Results

Verified stationarity of DJI log returns using dual tests (ADF & KPSS).

Seasonal patterns successfully removed from temperature data.

Created a ready-to-model dataset linking morning weather patterns to daily stock movement.

📄 License

Licensed under the MIT License - see the LICENSE file for details.
