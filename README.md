# Equities Pairs Trading Strategy

This project implements an **equities pairs trading model** in Python.  
The strategy identifies potentially cointegrated equity pairs, generates entry and exit signals based on z-score thresholds, and evaluates performance using out-of-sample testing.

---

Purpose:
- To further my career opportunities through upskilling.
- To demonstrate personal progress in python coding proficiency in a quant finance (buy-side) context.
- No python knowledge before 9 June 2025. Today 29 August 2025. 12 weeks of learning.

Methodology:
- download data for an equity index and its constituents
- clean data
- convert price data to daily returns and define in-sample (training period) DataFrame
- define performance calculation and presentation functions
- define functions to identify cointegrated pairs for trading strategy
- define functions to generate z-score entry/exit trading signals and portfolio positions
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
I have 20 years of experience in finance:
- 10 years in derivatives sales and structuring at Barclays Capital, Lloyds Banking Group, and Crédit Agricole CIB, where I became a derivatives
  structuring desk head and Deputy Chief Dealer, generating $26.5m in desk PnL and $15m in individual PnL in top year.
- 10 years in non-front office roles, including at J.P. Morgan and Morgan Stanley, including in Risk and exotic rates derivatves valuations control.

I am now upgrading my **programming and quantitative skills** with the goal of securing a quantitative or quant-related role in a hedge fund or investment bank.
