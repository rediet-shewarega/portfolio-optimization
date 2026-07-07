# Time Series Forecasting for Portfolio Management Optimization

## Project Overview

This project applies time series forecasting and portfolio optimization techniques to support investment decision-making for GMF Investments. The goal is to analyze historical financial data, forecast Tesla stock price trends, optimize a portfolio using Modern Portfolio Theory, and backtest the strategy against a benchmark portfolio.

The analysis focuses on three assets:

- **TSLA**: Tesla stock, representing a high-risk, high-growth asset.
- **BND**: Vanguard Total Bond Market ETF, representing a low-risk stability asset.
- **SPY**: S&P 500 ETF, representing diversified broad market exposure.

The data was collected using the `yfinance` Python library for the period from **January 1, 2015 to June 30, 2026**.

---

## Business Objective

GMF Investments wants to use historical financial data and forecasting models to improve portfolio management decisions. This project supports that objective by:

1. Exploring asset price behavior and risk characteristics.
2. Building time series forecasting models for Tesla stock.
3. Forecasting future Tesla market trends.
4. Constructing an optimized portfolio using Modern Portfolio Theory.
5. Backtesting the optimized portfolio against a passive benchmark.

---

## Project Structure

```text
portfolio-optimization/
│
├── .github/
│   └── workflows/
│       └── unittests.yml
│
├── data/
│   ├── raw/
│   │   ├── TSLA_raw.csv
│   │   ├── BND_raw.csv
│   │   └── SPY_raw.csv
│   │
│   └── processed/
│       ├── TSLA_cleaned.csv
│       ├── BND_cleaned.csv
│       ├── SPY_cleaned.csv
│       ├── risk_metrics.csv
│       ├── arima_metrics.csv
│       ├── tsla_future_forecast.csv
│       ├── task3_forecast_summary.csv
│       ├── recommended_portfolio_weights.csv
│       ├── recommended_portfolio_summary.csv
│       ├── efficient_frontier_portfolios.csv
│       └── backtest_performance_metrics.csv
│
├── notebooks/
│   ├── 01_eda_and_preprocessing.ipynb
│   ├── 02_arima_modeling.ipynb
│   ├── 03_forecast_future_trends.ipynb
│   ├── 04_portfolio_optimization.ipynb
│   ├── 05_strategy_backtesting.ipynb
│   └── README.md
│
├── reports/
│   └── figures/
│       ├── tsla_future_forecast_confidence_interval.png
│       ├── covariance_matrix_heatmap.png
│       ├── efficient_frontier.png
│       └── backtest_strategy_vs_benchmark.png
│
├── scripts/
├── src/
├── tests/
├── .gitignore
├── README.md
└── requirements.txt