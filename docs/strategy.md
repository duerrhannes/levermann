# Introduction and some words on the strategy #

The strategy is a quantitative stock strategy devised by former funds manager Susan Levermann (https://de.wikipedia.org/wiki/Susan_Levermann).
It involves a scoring system based on a set of criteria. The criteria relate to both fundamental and technical characteristics of a stock.
High-scoring stocks in the Levermann model are the ones that the model identifies as likely to outperform their benchmarks. According to the strategy, these high-scoring stocks are bought and held until their score falls below a certain level. Then they are sold and other high-scoring stocks are bought instead.

The original Levermann strategy includes (up to) 13 criteria. Each criterion scores either positive, negative or zero points. These points are added up. Stocks having a certain number of points can be bought, whereas shares whose score then falls below a certain treshold are to be sold again and replaced by other high-scoring shares.
The portfolio size usually recommended for this strategy is 10 to 15 shares.

The list of criteria and the number of points awarded may vary slightly depending on whether the shares are from large, medium or small companies (large caps, mid caps or small caps). A distinction is also made between shares from the financial sector and other business areas.
The strategy on the blog of Petra Wolff (https://petrawolff.blog/experiment-levermann-depot) follows this approach. For more information on the Levermann strategy and an "experiment" with a real depot, check out her website, https://petrawolff.blog. 
In the model I used, this differenciation of market cap and business sector was omitted, for the sake of avoiding an overly complex model (after all, any model is just as good as the data fed into it are...).

## The criteria list ##
The 13 individual criteria and their evaluation logic are listed here.

### Criterion 1: The return on equity in the last financial year. ###
If it is greater than 20%, there is +1 point, if it is less than 10%, there is -1 point. Otherwise 0 points.

### Criterion 2: EBIT margin in the last fiscal year
+1 point if it is greater than 12%, -1 point if it is less than 6%, 0 if it is in between.

### Criterion 3: Equity ratio in the last fiscal year
+1 for greater than 25%, -1 for less than 15%, 0 for values in between.
Last fiscal year in the scope of this project always means the last completed fiscal year. This means that the figures for it are fixed and have already been published.

### Criterion 4: Price/earnings ratio (P/E) over 5 years
+1 for less than 12, -1 for greater than 16, 0 for everything in between. -1 for negative P/E ratio.
The P/E ratio over 5 years is determined by dividing the current price by the average of earnings per share over five years. To calculate the average earnings per share, the figures for the three most recently completed fiscal years and estimates for the current and next fiscal year are used.

### Criterion 5: P/E ratio for the current fiscal year
+1 for less than 12, -1 for greater than 16, 0 for everything in between. -1 for negative P/E ratio.
The P/E ratio for the current fiscal year is calculated by dividing the current share price by the estimated earnings per share for the current fiscal year.

### Criterion 6: Analyst Opinions
If there are five or more analyst opinions, this is a contra indicator, i.e. if the analysts rate Sell, there is +1 point, if they say Buy, there is -1 point, if they recommend Hold, that's 0 points.
However, if there are less than five analysts' opinions, they count directly, i.e. +1 point for Buy, -1 point for Sell and 0 points for Hold. If there are no analyst opinions, this means 0 points.

### Criterion 7: Reaction to quarterly figures
If the reaction is positive, i.e. more than 1% ahead of the benchmark index, +1 point is awarded; if the reaction is negative, i.e. more than 1% behind the benchmark index, -1 point is awarded; between -1% and 1% 0 points are awarded.
For the calculation, the percentage development of the share price from the day of the figures compared to the previous day is determined on the basis of the closing prices, likewise for the benchmark index. The delta between the two percentages is then calculated.

### Criterion 8: Earnings revisions
+1 point if they have been adjusted by more than +5%, -1 point if they have been adjusted by more than -5%, 0 points if they are more or less unchanged (between -5% and 5%).
To do this, in each case the current earnings estimates are compared with those from two or four weeks ago.

### Criterion 9: Price today versus price 6 months ago (relative)
+1 point if higher by more than +5%, -1 point if lower by more than -5%, 0 points in between. 
To consider fluctuations on the markets, the performance is measured against each stocks' benchmark index, i.e. +1 point is awarded if the stock has outperformed its benchmark by at least +5.

### Criterion 10: Price today compared with price one year ago (relative)
As criterion 9, but over a period of one year.

### Criterion 11: Price momentum
There is +1 point if criterion no. 9 gives +1 point and criterion no. 10 gives 0 or -1 point. There is -1 point if there is -1 point for No. 9 and at the same time there is 0 or +1 point for No. 10. Otherwise there are 0 points.

### Criterion 12: Three-month reversal
If the stock has always underperformed the benchmark index in the last three months, +1 point is awarded. If it has always outperformed its benchmark, -1 point is awarded. Otherwise 0 points are awarded.

### Criterion 13: Profit growth
If the expected profit of the next fiscal year exceeds that of the current one by more than 5%, there is +1 point. If the expected profit of the next year is more than -5% below the profit expected in the current year, there is -1 point. Otherwise 0 points are awarded.


## Results
For each stock, the total sum of the above criteria is then calculated. Stocks having a higher score than a defined value are considered as a potential Buy (or to be held, if already in the portfolio). Stocks going below a certain number of points are considered as Sell, if already in the portfolio.


Disclaimer: This tool is intended for personal use only and should not be used for making investment decisions!
