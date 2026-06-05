# Task 2: Stock Price Prediction

## Objective
Use historical stock data to predict the closing price using regression models.

## Dataset
- **Source:** Yahoo Finance via `yfinance` library — no file download needed
- **Stock used:** Apple Inc. (AAPL)
- **Period:** 2020-01-01 to 2024-12-31
- **Features:** Open, High, Low, Volume
- **Target:** Close price

## Libraries Used
`pandas` `numpy` `matplotlib` `yfinance` `scikit-learn`

## Models Applied
- Linear Regression
- Random Forest Regressor (100 estimators)

## Steps
1. Download historical stock data using yfinance
2. Drop missing values and prepare features
3. Split data into train/test sets (80/20) without shuffling to preserve time order
4. Train Linear Regression and Random Forest models
5. Evaluate both models using MAE, RMSE, and R²
6. Plot actual vs predicted closing prices for both models
7. Plot Random Forest feature importance

## Key Results & Findings
- Random Forest outperforms Linear Regression on stock data
- High and Low prices are the most important features for predicting Close price
- Volume has the least predictive power
- Time series data must not be shuffled during train/test split
- Short-term stock prediction is sensitive to market volatility

## 🙋 Author

Built as part of an AI/ML internship project at **DevelopersHub Coorporation**.
