# Risk-on-off-Indicator
A risk on/off indicator based on volatility

This is a test of a paper from José P. Dapena, Juan A Serur and Julián R. Siri. the paper is called "Risk on- Risk off: a regime switching model for active portfolio management", December 2019.

The purpose of this code is to test the useness of this paper for a retail investor to switch between two funds: a stock fund and a risk free asset.

When the most likely state is one with a low volatility spread, which means that the realized volatility is increasing more than the implied volatility, the strategy allocates the funds in short-term Treasuries, and the strategy becomes “risk off”; otherwise, the strategy allocates the funds in the S&P 500 Index (proxied by the SPY), where the strategy becomes “risk on”.

To do so we use the "SPY" ETF as the stock fund and the "TLT" ETF as the risk free asset.

For the volatility spread we use the difference of the 20 days realized volatility minus the implied volatility (where we use the VIX Index as a proxy).

