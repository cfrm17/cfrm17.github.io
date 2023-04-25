
### Dividend Risk Model Calibration


Calibration is based on two-year time series of Bloomberg data field BEST_DPS with BEST_FPERIOD_OVERRIDE set to be 1BF, meaning one-year forward rolling window. Some adjustment may be needed to remove data error, such as beginning of year adjustment.

As described in model description and calibration of the model, the daily innovation to expected dividend of an index is simulated from double exponential distribution with specified correlation with all other risk factors. The daily innovation to expected dividend of a single stock is simulated on the fly without correlation with other risk factors. 

In theory, index dividend yield can be derived from the corresponding underlying index spot price and index futures price.  

By following the above procedure, we will be able to calculate an annualized dividend yield for SPX index for each futures contract in any business day. Usually the trading on the longer term futures is not as active (liquid) as the front contract so the price on longer term futures may be less reliable as the price of the front contract. For simplicity, we will take the average of the yields calculated based on different futures contract as the dividend yield of the underlying index. This will reduce the term structure of the dividend yield to a scalar valued annualized dividend yield. The rationale is mainly based on practicality of reducing unnecessary risk factors. But it is also based on the fact that the long term yield is very uncertain due to illiquid calibration instruments. 

However, we found that the day-to-day volatility of expected dividend calculated from index futures is extraordinarily high. For example, the empirical one-day volatility of expected dividend of SPX index is above 40%, which is not reasonable. A careful investigation leads to the following findings.


References:

[bitbucket pdf](https://bitbucket.org/timxiao1203/dividendcalibration/downloads/dividendCalibration.pdf)

[github exam](https://github.com/cfrm17/baseCorrelationExam)

[github ccirs](https://github.com/cfrm17/ccirs)

[github cdo](https://github.com/cfrm17/cdoMapping)
