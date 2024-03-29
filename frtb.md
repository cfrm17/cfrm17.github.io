
### FRTB Standarlized Approach

The Fundamental Review of the Trading Book (FRTB) is a new Basel committee framework for the next generation market risk regulatory capital rules. It is 
inspired by the undercapitalisation of trading book exposures witnessed during the financial crisis. FRTB aims to address shortcoming of the current Basel 
2.5 market risk capital framework.

FRTB provides a clear definition of the boundary between the trading book and the banking book. It consists of an overhaul of the internal model 
approach (IMA) to focus on tail risk and an overhaul of the standardized approach (SA) to make it more risk sensitive. Each approach also explicitly 
captures default risk and other residual risks. Liquidity risk is explicitly included for different asset classes via liquidity horizons.

FRTB has an interanl model approach and a standardized approach: the overhaul of the internal model approach (IMA) to focus on tail risk, while the 
overhaul of the standardized approach (sa) to make it more risk sensitive and explicitly capture default risk and other residual risks. It includes 
liquidity horizons explicitly for different asset classes.

The standardized approach (SA)is a regulator-set approach. It contains the sensitivity-based risk charge (SBRC), the default risk charge (DRC-SA), and
the residual add-on (RAD).

The standardized Approach defines three risk measures. They are Delta measure, Vega measure, and Curvature measure. The calculation is based on seven 
risk classes: General interest rate (GII), Credit spread risk, Credit spread risk with non-correlated securitisation, Credit spread risk with 
correlated securitisation, Equity, Commodity, Foreign exchange. 

The sensitivity based risk charge should be calculated separately for each risk class and each risk measure. The reporting hierarchy is portfolio, desk, 
bank. Total risk charge = sensitivity-based risk charge + default risk charge +residual add-on
For example, an equity desk has only equity and interest rate risk, Total risk charge = equity Delta charge + equity Vega charge + equity Curvature 
charge + GII charge + DRC + RAD

The FRTB Default risk charge covers Debt instruments, Equity products, and Securitisation. The Calculation procedure is: First, determine jump-to-default 
(JTD) loss amount; second, offset the JTD amounts of long and short exposures with respect to the same obligor; third, discount the net short exposures 
by a hedge benefit ratio. Finally, apply default risk weights to exposures to arrive at the DRC.


Reference: 

[Fundamental Review of Trading Book](/frtbSa-6.pdf)

[Zenodo frtb](https://zenodo.org/record/4017728/files/frtbSa-6.pdf)

[Fliphtml5 frtb](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamMDNwkzM5ITPkl0av9mY)

[Zenodo cms cliquet](https://zenodo.org/record/6561892/files/cmsCliquet.pdf)

[OSF frtb](https://osf.io/pn768/download)

[Github tarn swap](https://github.com/timxiao1203/TARN-Swap)

[Github LVGM](https://github.com/timxiao1203/LocalVolatilityGaussianModel)

[OSF local vol](https://osf.io/74s83/downloand)
