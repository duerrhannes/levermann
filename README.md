Levermann tool - quantitative stock analysis
==============================

This little python script for quantitative stock analysis uses the valuation method developed by [Susann Levermann](https://de.wikipedia.org/wiki/Susan_Levermann). Some changes to the original strategy (i.e.  were made, following the approach of Petra Wolff, which is also described [on her blog](https://petrawolff.blog/levermann-experiment/).
The data for the financials is fetched from Yahoo Finance, mainly using the python modules `yahooquery` and `yfinance`.

- A manual on how to use the tool can be found in references -> [getting started](docs/getting-started.rst)
- Need some background on the strategy? A brief overview can be found in [Strategy](references/Strategy) (or check the above mentioned link to the Blog of Petra Wolff)
- Sample output can be found in this excel file under [reports](reports) as well as [result plots](reports/figures) <links to specific files/directories to be added>
- A short analysis of the results and interpretation guide is in this [Analysis of the results](reports) <link to specific file to be added>

![Animation](src/visualization/Animation.gif)

Disclaimer: this tool is for information purposes only. It is not intended to be used for making investment decisions!
