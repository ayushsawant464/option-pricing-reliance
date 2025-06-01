# Reliance Options Implied Volatility & Technical Analysis
This repository contains a Jupyter notebook for analyzing Reliance Industries options and equity data, focusing on implied volatility modeling and technical indicator-based signal generation.

# Features
Options Data Processing:
Loads and processes a large dataset of Reliance options (calls and puts) from January 2023 to May 2025, including strike, expiry, close price, underlying value, and more.

Equity Data Download:
Fetches historical price and volume data for Reliance Industries (RELIANCE.NS) using Yahoo Finance.

Implied Volatility Calculation:

Implements the Black-Scholes option pricing model for both calls and puts.

Computes implied volatility (IV) for each option using Brent's method, with no-arbitrage checks for price validity.

Visualizes the implied volatility surface across strikes and expiries.

# Technical Indicators:
Calculates key technical indicators on the underlying stock:

Moving Averages (MA50, MA100, MA200)

Relative Strength Index (RSI)

Moving Average Convergence Divergence (MACD)

Signal columns for each indicator (Buy/Sell/Hold)

# Helper Functions:

In/Out-of-the-money checks for options.

Kelly criterion for position sizing based on historical returns.

# Strategy Skeleton:
Framework for generating monthly trading signals based on technical indicators and linking them to options data.(inefficient)

# Data Sources
Options Data:
CSV file: /content/options-JAN2023-MAY2025 (taken from nseindia)
Columns include: Date, Symbol, Option type, Strike Price, Close, Underlying Value, Expiry, TimetoExpiry, RiskFreeRate.

Equity Data:
Downloaded using yfinance for ticker RELIANCE.NS from 2023-01-01 to 2025-05-29.

# Requirements
Python 3.8+

# Libraries: 
yfinance, pandas, numpy, scipy, matplotlib, mpl_toolkits.mplot3d

# Usage
Clone the repository and open the notebook in Jupyter or Google Colab.

Ensure the options CSV file is available at the specified path.

Run all cells in order for data loading, analysis, and visualization.

# Example Workflow
Load options and equity data

Calculate implied volatility using Black-Scholes and Brent's method

Visualize the implied volatility surface

Compute technical indicators (MA, RSI, MACD) and generate trading signals

Use helper functions for moneyness checks and Kelly criterion

