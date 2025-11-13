Market Forecasting and Portfolio Management

📘 Overview

This project benchmarks and compares multiple machine learning models for market forecasting and portfolio management.
We aim to evaluate various models studied throughout the course, identify the best-performing model for forecasting stock market trends, and then leverage its predictions to develop a dynamic portfolio management strategy.

Goal:
Build a machine learning tool capable of identifying optimal investment strategies using historical U.S. stock market data.

💾 Data Description

We use U.S. stock data (2010–2023), including:

Open/Close Prices

Dividends

Stock Splits

Trading Volume

Training & Evaluation Split

Training Period: 2010–2022

Testing Period: 2023

Focused Stocks
Sector	Company	Ticker
Technology	Apple Inc.	AAPL
Consumer Discretionary	Amazon.com Inc.	AMZN
Healthcare	Johnson & Johnson	JNJ
Financials	JPMorgan Chase & Co.	JPM
Communication Services	Alphabet Inc.	GOOGL
Industrials	Boeing Co.	BA
Consumer Staples	Procter & Gamble Co.	PG
Energy	Exxon Mobil Corp.	XOM
Utilities	NextEra Energy Inc.	NEE
Materials	Dow Inc.	DOW
Data Source

We use the open-source Python library yfinance
 to retrieve historical data from Yahoo! Finance.

Each instance of the dataset represents one trading day. From 2010 to 2023, there are approximately 3,000 trading days.

🔮 Part 1: Market Forecasting
Objective

Identify the best model for market performance forecasting based on historical data.

Methodology

Evaluate multiple ML models and hyperparameters.

Test different backtracking periods (length of historical data used).

Use multiple features (dividend, stock splits, volume, etc.) depending on model design.

Target variable: Adjusted close price of selected stocks.

Perform data preprocessing to remove non-lagged features and prevent data leakage.

💹 Part 2: Portfolio Management
Objective

Use the forecasted results from Part 1 to manage a simulated investment portfolio, dynamically adjusting stock weights to maximize returns.

Methodology

Use both historical and forecasted data as features.

Choose flexible target variables (e.g., return rate, portfolio value).

Implement trading strategies that rebalance the portfolio daily based on model predictions.

Goal:
Maximize total return by optimal weight allocation across assets.

🧮 Final Evaluation

Initial Portfolio Value: $1,000,000

Use the models from Part 1 and Part 2 to manage the portfolio over the testing period (2023).

Compare final portfolio returns across models to identify the most effective forecasting and management approach.

Evaluation Metric:
Total return at the end of the testing period.

🛠️ Tools & Libraries

Python 3.9+

yfinance – Stock data retrieval

pandas / numpy – Data manipulation

scikit-learn / XGBoost / LSTM (optional) – Model training and evaluation

matplotlib / seaborn – Visualization

📈 Expected Outcomes

Identify which model best predicts adjusted closing prices.

Develop a data-driven trading and rebalancing strategy.

Quantify performance gains through backtesting and portfolio simulation.
