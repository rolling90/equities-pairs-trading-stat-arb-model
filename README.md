# Equities Pairs Trading Strategy

This project implements an **equities pairs trading model** in Python.  
The strategy identifies potentially cointegrated equity pairs, generates entry and exit signals based on z-score thresholds, and evaluates performance using out-of-sample testing.

---

Methodology:
- download data for an equity index and its constituents
- clean data
- convert price data to daily returns and define in-sample (training period) DataFrame
- define performance calculation and presentation functions
- define functions to identify cointegrated pairs for trading strategy
- define functions to generate z-score entry/exit trading signals and portfolio positions
- scale positions by rolling volatility
- evaluate multiple user defined z-score exit threshold levels and automatically select optimal exit threshold
- execute stratey for optimised exit z-score threshold
- display performance charts (returns, signals generated for one example pair, drawdown, duration) and summary data (returns, sharpe, etc)

Known deficiencies:
- Using personal laptop not an institutional machine, so no access to Bloomberg for full markets data universe and limited computational power.
- Use yfinance library for data. Limited to projects that rely on tickers available in yfinance, e.g. equities and FX, not rates.
- Intentional selection of equity index with a small number of constituents to limit computational power expense.
- intentional simplification of transaction costs for illustrative purposes. Ignores dynamic TCA data for a trailing period.

---

## About Me
- 20 years' finance experience
- Prior employers include Morgan Stanley, Deutsche Bank, Barclays Capital, Crédit Agricole CIB.
- 10 years in front office derivatives struturing/trading roles.
