
### Monte Carlo Value at Risk

Value at Risk (VaR) is the regulatory measurement for assessing market risk. It reports the maximum likely loss on a portfolio for a given probability defined 
as x% confidence level over N days. VaR is vital in market risk management and control. Also regulatory and economic capital computation is based on VaR results. 
Although VaR measure is objective and intuitive, it doesn’t capture tail risk. There are three commonly used methodologies to calculate VaR – parametric, 
historical simulation and Monte Carlo simulation. This presentation focuses on Monte Carlo VaR.  

Monte Carlo VaR assumes  market factors follow certain stochastic processes. It has easy back and stress test and is good for high confidence level and 
tail risk. The drawbacks are dependent on distribution assumption and calibration is required. Most importantly it requires extensive computation.

The only way to verify a VaR system is backtest. At a certain day, compute hypothetic P&L (valuation date and portfolio unchanged). If (hypothetic P&L > VaR), 
then breaches. For one year, if number of breaches is 0-4, the VaR system is in Green zone. If number of breaches is 5-9, the VaR system is in Yellow zone
If number of breaches is 10 or more, the VaR system is in Red zone.


Reference: 

[Monte Carlo VaR](/MonteCarloVaR-14.pdf)

[Hcommon McVar](https://hcommons.org/deposits/download/hc:33594/CONTENT/montecarlovar-14.pdf)

[OSF arrear quanto cms](https://osf.io/g6tp5/download)

[Zenodo mc var](https://zenodo.org/record/4027823/files/MonteCarloVaR-14.pdf)

[OSF mc var](https://osf.io/2a58h/download)

[OSF quanto cms](https://osf.io/u95g2/wiki/home/)
