# Equities Pairs Trading Strategy

This project implements a **mean reversion pairs trading model** in Python.  
The strategy identifies potentially cointegrated equity pairs, generates entry and exit signals based on z-score thresholds, and 
evaluates performance using out-of-sample testing.

---

## Methodology
- **Data download**: 7 years of historical daily price data for a user-defined equity index (e.g. CAC40) and its constituents.  
- **Training period**: The first 4 years are used to test for cointegration (using the Augmented Dickey-Fuller test).
- **Optimisation**: The strategy tests multiple exit z-score thresholds and selects the exit threshold with the highest sharpe ratio to perform backtesting with. 
- **Signal generation**: Entry and exit signals are based on z-score thresholds of the trailing 90-day residuals between pairs of equity log returns.  
- **Out-of-sample testing**: The final 3 years of data are used to evaluate performance.  
- **Outputs**:
  - Performance charts  
  - Summary performance statistics
- **Config class:** Users can manually edit the Config class to test various model parameters

---

## Known deficiencies
- yfinance (python's Yahoo finance library) is used for data downloads, because I do not have access to Bloomberg on my personal laptop.
  Thus I can only create a model that tests tickers available on yfinance. E.g. yfinance excludes full rates universe (yield curve constituents). 
- An equity index with a small number of constituents (CAC40) has been intentionally used to limit personal laptop computing power expense
- Transaction costs: dynamic rolling period TCA is ignored for transaction costs
- Additional entry signal validation, such as testing for predictive structure in individual equities’ return series (e.g. autocorrelation).

---

## Purpose
This project demonstrates my skills in:
- Python programming (12 weeks of learning as of 29 August 2025)  
- Data cleaning and manipulation with `pandas`  
- Time series analysis and statistical testing (ADF, cointegration)  
- Quantitative trading strategy design and evaluation  

---

## About Me
I have 20 years of experience in finance:
- 10 years in derivatives sales and structuring at Barclays Capital, Lloyds Banking Group, and Crédit Agricole CIB, where I became a derivatives
  structurign desk head and Deputy Chief Dealer.
- 10 years in non-front office roles at J.P. Morgan, Goldman Sachs and Morgan Stanley, across Risk, Middle Office and Exotic Derivatves Valuations Control.

I am now upgrading my **programming and quantitative skills** with the goal of re-entering investment banking or hedge funds in a quantitative or quant-related role.
