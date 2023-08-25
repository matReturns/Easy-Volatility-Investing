# Easy Volatility Investing
a replication of Tony Cooper's Paper "Easy Volatility Investing"
from ["matReturns.com"](https://matReturns.com)


# from: [matReturns.com](https://matReturns.com)

In Tony Cooper's ["Easy Volatility Investing"](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2255327), the author explores volatility trading using volatility-related Exchange Traded Funds (ETFs), providing a convenient alternative to traditional options, futures, or variance swaps trading. The paper aims to develop trading strategies using these new investment vehicles. The study not only reveals sources of volatility returns but also introduces five distinct strategies tailored to various investors' profiles. Four of these strategies are straightforward to implement and have yielded impressive returns with high Sharpe Ratios, and low correlation to the S&P500, some even showing negative correlation. However, the study emphasizes the need for caution due to the associated risks and likens the high returns to picking up $100 bills in front of a steamroller.

The strategies are designed to reduce portfolio risk during crisis periods while maintaining positive exposure to markets during favorable times and negative exposure during adverse conditions. Although not consistently delivering absolute returns and experiencing occasional drawdowns, the paper recommends adapting the traditional 60% equities, 40% bonds portfolio to 55% equities, 35% bonds, and 10% volatility to incorporate these strategies effectively.

## ETFs and Indices

The replication uses the following ETFs and indices:

- **SVXY**: ProShares Short VIX Short-Term Futures ETF
- **VIXY**: ProShares VIX Short-Term Futures ETF
- **^GSPC**: S&P 500 Index
- **^VIX**: CBOE Volatility Index
- **^VIX3M**: CBOE S&P 500 3-Month Volatility

## Strategies

The study presents four trading strategies for volatility investing:

1. **Buy and Hold (B/H)**: This basic strategy involves holding the *SVXY* ETF.
2. **Momentum**: This strategy focuses on volatility momentum trading, holding the ETF *SVXY* or *VIXY*, with the best return over a specified number of days (*k*-days). The paper used *k = 83*.
3. **Contango-Backwardation Roll Yield (CBR)**: This strategy maximizes roll yield by investing in *SVXY* during contango and *VIXY* during backwardation of the *VIX* term structure. The rule uses the $10$ day average of *VIX3M*/ *VIX* ratio to determine investments.
4. **Volatility Risk Premium (VRP)**: This strategy captures the VRP using the HVOL10S strategy, which involves the 5-day moving average of (*VIX* - 10-day historical S&P500 volatility from *^GSPC* index). It decides whether to invest in *SVXY* or *VIXY*.

## Conclusion

In conclusion, the study offers valuable insights into volatility investing and presents multiple strategies catering to different investors' preferences and risk tolerances. It's crucial to thoroughly understand the risks and limitations of each strategy before incorporating them into investment portfolios.





















