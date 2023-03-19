
### Parametric Value at Risk

Value at Risk (VaR) is the regulatory measurement for assessing market risk. It reports the maximum likely loss on a portfolio for a given probability defined 
as x% confidence level over N days. VaR is vital in market risk management and control. Also regulatory and economic capital computation is based on VaR results. 
Although VaR measure is objective and intuitive, it doesn’t capture tail risk. There are three commonly used methodologies to calculate VaR – parametric, 
historical simulation and Monte Carlo simulation. This presentation focuses on parametric VaR.  

VaR represents a critical risk model which requires governance around Risks not in VaR (RNIV). RNIV are market factors driving P&L which are not captured in the 
VaR model. Performance of the VaR model can be evaluated through backtesting by comparing the model’s risk measures and actual trading outcomes.

The only way to verify a VaR system is backtest. At a certain day, compute hypothetic P&L (valuation date and portfolio unchanged). If (hypothetic P&L > VaR), 
then breaches. For one year, if number of breaches is 0-4, the VaR system is in Green zone. If number of breaches is 5-9, the VaR system is in Yellow zone
If number of breaches is 10 or more, the VaR system is in Red zone.
	


Reference: 

[Parametric Value at Risk](/ParametricVaR-12.pdf)

[Bitbook p&l](https://cmrm11.gitbook.io/unexplained-profit-and-loss/)

[Bitbook backtest](https://cmrm11.gitbook.io/market-risk-backtest-exception/)

[Zenodo parametric var](https://zenodo.org/record/4027809/files/ParametricVaR-12.pdf)

[Fliphtml5 parametric var](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamUjNzQTN5ITPkl0av9mY)

[OSF parametric var](https://osf.io/uzpk3/download)

[Zenodo xccy swap](https://zenodo.org/record/6588375#.YpEh86gpDq4)

[OSF 3 factors](https://osf.io/pbjf8/download)
