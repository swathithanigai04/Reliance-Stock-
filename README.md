# Reliance-Stock-

This project presents a comprehensive time series analysis and forecasting of Reliance Industries' stock prices using Python and machine learning techniques. By utilizing high-frequency stock data, the project aims to provide insights into price trends, volatility, and long-term forecasting, empowering investors and analysts to make informed, data-driven decisions.

### Objective

The primary objective of the project is to:

* Perform **Exploratory Data Analysis (EDA)** on historical Reliance stock data.
* Analyze **volatility**, **trends**, and **seasonal patterns** in price movements.
* Apply **time series forecasting** to predict future stock prices using Facebook Prophet.
* Support **risk management** and **investment decision-making** with data-backed insights.

### Dataset

* **Source**: [Kaggle – BSE 15-Minute Interval Stock Data](https://www.kaggle.com/datasets/saurabhshahane/bse-stocks-data-15-minute-interval-historical/data)
* **Frequency**: 15-minute intervals (aggregated to daily data for forecasting)
* **Features**: Date, Open, High, Low, Close, Volume

### Data Preprocessing

* Converted timestamps to standard `datetime` format and extracted relevant components.
* Aggregated 15-minute data to daily intervals.
* Handled missing dates using forward-fill methods.
* Detected outliers using **Z-score** and visualized with histograms and box plots.
* Computed summary statistics (mean, median, standard deviation, quartiles).

### Methodology

* **EDA**: Trend and volatility analysis using line charts, candlestick plots, and moving averages.
* **Forecasting Model**:

  * Used **Facebook Prophet** for time series forecasting.
  * Forecasted stock prices up to **December 2026**.
  * Evaluated with **train-test split** using metrics: **MAE**, **RMSE**, **MAPE**.
* **Visualization**:

  * Interactive **candlestick charts** using Plotly.
  * **Trend decomposition** and **rolling statistics** (20-day & 50-day SMA).
  * Volatility plots showing daily return fluctuations.

### Model Performance

* **Forecast Accuracy**:

  * **Accuracy**: 90.58%
  * **MAPE**: 9.42% (indicating good prediction reliability)
* The model successfully captured long-term trends with minimal seasonal interference, offering a reliable prediction for future price movements.

### Technologies Used

**Languages & Platforms**:
Python, Jupyter Notebook

**Libraries & Frameworks**:
Pandas, NumPy, Matplotlib, Seaborn, Plotly, Facebook Prophet, Scikit-learn

**Techniques**:
Time series forecasting, EDA, outlier detection using Z-scores, rolling average analysis

### Future Work

* **Feature Engineering**: Integrate macroeconomic indicators, earnings reports, or external events for enhanced accuracy.
* **Sentiment Analysis**: Combine stock price data with social media and news sentiment to improve forecasting reliability.
* **Advanced Models**: Compare Prophet’s performance with LSTM or ARIMA for deeper evaluation.

