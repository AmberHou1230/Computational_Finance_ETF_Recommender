# Quantitative_Finance
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


Determining the universe of ETFs
-------------------




Data Cleaning
-------------------
- Importing Libraries 
```Python
import pandas as pd
import numpy as np
import plotly.express as px
import matplotlib.pyplot as plt 
print('modules are imported')
```
