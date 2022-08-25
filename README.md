# Fundamental-Indexing-and-Smart-Beta
Project on Smart Beta, Fundamental Indexing, Factor Investing and Stock Returns using R. 

Implemented in R using tidyverse packages, using functional programming concepts.

Steps for Hypothesis testing (GRS test) for CAPM model: Estimate the beta of the firm every year for the period for every year. Take window of 1,3,6,12,24 months, analyze and take the best beta for further calculations.

Sort all stocks from selected Beta values, Form deciles of the betas - choose only one beta from previous section and for a Value-weighted portfolio (weighted by the market capitalization) returns. Present the Newey-West t-statistic,(Adjusted using 5 lags) to test the null hypothesis that the average portfolio excess return or CAPM alpha is equal to zero

All the strategies and performance is based on the COMPUSTAT data. The data is lagged by a year to remove the lookahead bias when constructing a portfolio or strategy returns. First we try to achieve a portfolio with fundamental variables as the weights of the stocks to be picked up. and them we delve into different market variables to use as weights in picking up stocks.

Rank the stocks based on each of the fundamental variable as of January 1st of each year. Pick up each of the following fundamental variable one by one.

Use the respective fundamental variable as the weight to construct a portfolio

Hold the respective portfolio for the rest of the year and rebalance on the last trading day of the year

Fundamental Indexing: book value (Book), trailing (past) five-year average cash flow (Cash Flow), trailing five-year average revenue (Revenue), trailing five-year average gross sales (Sales), trailing five-year average gross dividends (Dividends), trailing five year gross investments (Investment), trailing five year profitability, return on assets, (Profitability), asset turnover (Asset turnover), Altman Z-score (Altman-Z), Ohlson score (Ohlson-O)

Market Variables: Beta, Total Volatility, Average monthly volatility in last year, Annulized volatility, Idiosyncratic Volatility (as defined in the added picture) of CAPM, Fama French 3 factor and 5 factor model
