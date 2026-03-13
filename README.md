# StockSight 📈

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![Streamlit](https://img.shields.io/badge/Framework-Streamlit-red)
![License](https://img.shields.io/badge/License-MIT-green)

A **quantitative finance and machine learning project** that predicts stock prices using historical market data.
The project provides **interactive visualization, volatility analysis, and price forecasting** through a **Streamlit dashboard**.

This tool demonstrates how **data science and machine learning** can be applied to **financial market prediction**.

---

# Project Overview

Quant Market Predictor analyzes historical NASDAQ stock data and applies **Linear Regression models** to forecast future stock prices.

The project includes:

* Financial data collection
* Data preprocessing
* Machine learning prediction
* Risk & volatility analysis
* Interactive visualization dashboard

The system is designed for:

* Data science learners
* Quantitative finance beginners
* Machine learning experimentation
* Financial data analysis

---

# Demo Dashboard

## 📊 Historical Stock Price Visualization

This visualization shows the **historical daily average price of Microsoft (MSFT)** over the selected time period.
Users can analyze **trends and historical price movements using interactive charts**.

![Microsoft Stock Historical Chart](images/plot-data.png)

---

## ⚠️ Stock Risk Analysis

The dashboard calculates a **risk score based on stock volatility**.

In this example, **Microsoft shows a moderate risk level** with a calculated volatility score.

![Microsoft Risk Analysis](images/stock-risk.png)

Example result:

```
Risk Score for MSFT: 0.236
Moderate Risk
```

---

## 🤖 Future Price Prediction

Using a **Linear Regression machine learning model**, the system predicts the future stock price based on historical trends.

Example prediction:

```
Predicted price for MSFT in 30 days: $470.45
```

![Microsoft Price Prediction](images/predict-future.png)

---

# Project Architecture

```
                +----------------------+
                |  Yahoo Finance API   |
                +----------+-----------+
                           |
                           v
                +----------------------+
                |   Data Processing    |
                |  (Pandas / NumPy)    |
                +----------+-----------+
                           |
                           v
                +----------------------+
                | Machine Learning     |
                | Linear Regression    |
                +----------+-----------+
                           |
                           v
                +----------------------+
                |  Visualization Layer |
                | Streamlit + Altair   |
                +----------------------+
```

---

# Project Structure

```
Quant-Market-Predictor
│
├── resources/          
├── scripts/            
├── tests/              
│
├── images/             
│   ├── plot-data.png
│   ├── stock-risk.png
│   └── predict-future.png
│
├── main.py             
├── requirements.txt    
├── setup.py            
├── LICENSE.txt
└── README.md
```

---

# Installation ⚙️

Clone the repository:

```bash
git clone https://github.com/ahmad-masud/Quant-Market-Predictor.git
```

Navigate into the project:

```bash
cd Quant-Market-Predictor
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# Running the Application

Start the Streamlit dashboard:

```bash
streamlit run main.py
```

After running, open the **local Streamlit URL** in your browser.

---

# How to Use

1. Select a **stock ticker** (example: `MSFT`, `AAPL`, `TSLA`)
2. Choose the **historical data period**
3. Select analysis type:

   * Predict Future Price
   * Measure Stock Risk
   * Plot Historical Data
4. View the results in the dashboard.

---

# Dependencies

Main libraries used:

```
numpy
pandas
scikit-learn
streamlit
altair
yfinance
```

Install them with:

```bash
pip install -r requirements.txt
```

---

# Machine Learning Model

The project uses **Linear Regression** to estimate future stock prices from historical data trends.

Possible improvements:

* LSTM neural networks
* ARIMA forecasting models
* Random Forest regression
* Transformer-based time series models

---

# Future Improvements

Possible enhancements for the project:

* Deep learning stock prediction
* Multi-stock portfolio comparison
* Portfolio optimization tools
* Real-time market streaming
* Backtesting trading strategies

---

# Contributing

Contributions are welcome.

1. Fork the repository
2. Create a feature branch

```
git checkout -b feature-name
```

3. Commit your changes

```
git commit -m "Add feature"
```

4. Push your branch

```
git push origin feature-name
```

5. Open a Pull Request.

---

# License

This project is licensed under the **MIT License**.

See the `LICENSE.txt` file for full details.

---

# Disclaimer

This project is **for educational purposes only**.

Stock market predictions generated by this tool **should not be considered financial advice**.
