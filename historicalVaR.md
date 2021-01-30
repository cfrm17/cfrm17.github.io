
### Historical VaR

Value at Risk (VaR) is the regulatory measurement for assessing market risk. It reports the maximum likely loss on a portfolio for a given probability defined 
as x% confidence level over N days. VaR is vital in market risk management and control. Also regulatory and economic capital computation is based on VaR results. 
Although VaR measure is objective and intuitive, it doesn’t capture tail risk. There are three commonly used methodologies to calculate VaR – parametric, 
historical simulation and Monte Carlo simulation. This section focuses on historical VaR.  

The historical VaR approach follows the following procedures: First, obtain one year historical value time series of all market factors, such as a stock 
price time series is ■(x ̅_1&⋯&x ̅_251 ). Assuming today’s value is x_0, generate 250 historical scenarios. The i-th is  x_i=(x ̅_i⁄x ̅_(i-1) -1)x_0. 
Compute base PV at today t as P(x_o), Compute 250 scenario PVs:  P(x_i). Then derive 250 scenario P&L:	P(x_i )-P(x_0). Finally sort 250 scenario P&L. 
The VaR is the average between 2nd and 3rd lowest (negative) numbers.


The only way to verify a VaR system is backtest. At a certain day, compute hypothetic P&L (valuation date and portfolio unchanged). If (hypothetic P&L > VaR), 
then breaches. For one year, if number of breaches is 0-4, the VaR system is in Green zone. If number of breaches is 5-9, the VaR system is in Yellow zone
If number of breaches is 10 or more, the VaR system is in Red zone.


Reference:


[Historical Value at Risk](/HistoricalVaR-7.pdf)

[Pubpub histovar home](https://interestrate.pubpub.org/pub/116rqssv/release/1)

[Pubpub histovar pdf](https://assets.pubpub.org/4u9agnc5/01599313202010.pdf)

[Authorstream histovar](http://www.authorstream.com/Presentation/tommills-4397626-historical-value-risk-introduction/)

[Hcommon histovar](https://hcommons.org/deposits/download/hc:33480/CONTENT/historicalvar-7.pdf)

[PubHtml5 dependency](https://pubhtml5.com/noml/czqz/basic)

[FlipHtml5 historical var](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamQDO1UDN5ITPkl0av9mY)

[Github historical var](https://github.com/cfrm17/historicalVaR/raw/main/HistoricalVaR-7.pdf)

[Pubpub historical var](https://interestrate.pubpub.org/pub/116rqssv/download/pdf)

[Zenodo historical var](https://zenodo.org/record/4017733/files/HistoricalVaR-7.pdf)

[Bitbucket historical var](https://bitbucket.org/cfrm17/historicalvar/downloads/HistoricalVaR-7.pdf)

[Gitlab historical var](https://gitlab.com/cfrm171/historicalvar/-/raw/master/HistoricalVaR-7.pdf)

[ScienceMedia historical var](https://science-media.org/userfiles/1020/presentations/1020_presentation_468.pdf)

[Archive historical var](https://ia801502.us.archive.org/15/items/historical-va-r-7/HistoricalVaR-7.pdf)

