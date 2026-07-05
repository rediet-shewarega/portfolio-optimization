# Time Series Forecasting for Portfolio Management Optimization

## Project Overview
This project analyzes historical financial data for TSLA, BND, and SPY from January 1, 2015 to June 30, 2026. The goal is to explore trends, risk, volatility, and begin forecasting Tesla stock prices for portfolio management.

## Assets
- TSLA: High-risk, high-growth stock
- BND: Low-risk bond ETF
- SPY: Moderate-risk S&P 500 ETF

## Interim Submission
The interim submission includes:
- Task 1: Data extraction, cleaning, EDA, stationarity testing, volatility analysis, and risk metrics
- Task 2: Initial ARIMA model for TSLA forecasting

## Project Structure
- data/raw: Raw data downloaded from yfinance
- data/processed: Cleaned data and calculated metrics
- notebooks: Jupyter notebooks for EDA and modeling
- src: Source code folder
- tests: Test folder
- scripts: Utility scripts

## How to Run
Install dependencies:

```bash
pip install -r requirements.txt
```
Then run the notebooks in this order:

1. `notebooks/01_eda_and_preprocessing.ipynb`
2. `notebooks/02_arima_modeling.ipynb`

## Notebooks

- `01_eda_and_preprocessing.ipynb`: Data extraction, cleaning, EDA, stationarity testing, volatility analysis, and risk metrics.
- `02_arima_modeling.ipynb`: Initial ARIMA model for TSLA stock price forecasting.

## Key Outputs

- Adjusted closing price visualization for TSLA, BND, and SPY
- Daily returns visualization
- Rolling volatility analysis
- Outlier detection
- ADF stationarity test
- VaR and Sharpe Ratio risk metrics
- Initial ARIMA forecast for TSLA

## Key Insights

- TSLA showed the strongest growth but also the highest volatility.
- BND was the most stable asset and can help reduce portfolio risk.
- SPY provided moderate risk with diversified market exposure.
- The ADF test showed that price data is generally non-stationary, while daily returns are more suitable for risk analysis.
- ARIMA was implemented as the first baseline forecasting model for TSLA.

## Next Steps

- Improve ARIMA parameters using ACF/PACF or auto_arima.
- Build an LSTM model for final submission.
- Compare ARIMA and LSTM using MAE, RMSE, and MAPE.
- Use the best model for future forecasting and portfolio optimization.