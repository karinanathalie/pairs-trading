# Pairs Trading

## Introduction
Pairs trading is a market-neutral trading strategy that attempts to profit from the relative mispricing of two related securities. This repository contains the implementation of a pairs trading strategy using the Engle-Granger cointegration test and visualization of the entry and exit signals.

## About the Strategy
In pairs trading, the goal is to identify a pair of stocks that exhibit a mean-reverting relationship, known as cointegration. When the spread between the two stocks deviates significantly from its historical mean, there is an opportunity to open a trade and profit from the spread reverting to its mean value.

The key steps in the pairs trading strategy implemented in this repository are:

1. **Cointegration Analysis**: The Engle-Granger cointegration test is used to identify pairs of stocks that exhibit a long-term mean-reverting relationship.
2. **Spread Calculation**: The spread between the two cointegrated stocks is calculated and monitored for deviations from the historical mean.
3. **Trade Execution**: When the spread deviates beyond a certain threshold, a trade is opened to capitalize on the expected reversion to the mean.
4. **Trade Management**: The trade is closed when the spread reverts to its mean value, or when a pre-defined stop-loss or profit-taking level is reached.