# ETF Recommender 
-------------------
You got a job at Charles Schwab!

* As your first project, your boss wants you to create an **ETF Recommender** for your company.
* Whenever an investor is about to buy an ETF, you can recommend him/her other ETFs that are similar.
  * Parse the web for ETF holdings
  * Devise a method to compute the similarity between ETFs
  * Recommend similar ETFs, and state if there are any benefits from switching such as lower expense ratios.
* What would your recommendation be if an investor wishes to buy:
  * SPY
  * QQQ
  * ARKK
  * IBB
  * DIA
  * IWM
  * XLF
  * RTH
* In particular for QQQ, what would your recommendation be? Are investors rational in their behavior, or are there limits to rationality?


Additional Notes
* After that, we started web scraping. We used MongoDB to record our data
 * We got 14 ETF holdings (including their expense ratios) from Investco, 50 from iShares, 124 from StockAnalysis.com

* After loading everything into MongoDB, we wrote functions to calculate the cosine similarities between the ETFs
 * The advantage of using cosine similarity is that it accounts for differences in the market value of each holding. If one ETF is investing heavily in one stock and not so heavily in the other, we can use that information in our comparison. 
