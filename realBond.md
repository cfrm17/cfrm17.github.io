
### Real Return Bond Introduction


The real return on inflation-linked bonds can be decomposed into normal and breakeven inflation yields. We uses a forecast method to project the cash flows. The forecasting associated with the reference inflation 
number in the future is calculated using the assigned breakeven inflation curve (which is theoretically equivalent to the forward CPI curve). 

Note that when some inflation-linked bonds mature, the greater of the original or adjusted principal is paid. However only the adjusted principal is assumed to be paid. This leads to an underestimation of some 
inflation-linked bond values. Our study shows that often times the CAD and US CPI price indices increase, i.e., in general, the inflation adjusted principal tends to be greater than the original principal. 
Therefore, this impact is considered to be negligible.

Consider a year to year (YOY) inflation bond pays an indexed-linked coupon rate of interest at the ith  cash flow payment date i t , which equals an annual inflation return and a constant spread rate. 

Note that we assume the expected inflation return equals the forward inflation return. Then, a convexity premium is not considered in the YOY inflation bond valuations. Figure 1 shows that the convexity adjustment 
in basis points (bps) is negative and is a decreasing function of the settlement maturity in years for the one year inflation rate. Given the correlation between the spot inflation rates and the Libor rates is 20%, 
the convexity adjustment in bps is immaterial, where convexity adjustment is drived by volatility (see https://finpricing.com/lib/FxVolIntroduction.html)

At the time of default, the price of a deal largely depends on the contract definition and settlement rule. It is hard to define a unique pricing formula. In practice, a generic formula for P&L at default, 
can be used to handle instruments without clear settlement information at default. However, for instruments with available information, the price should be specified more accurately; this is important for IRC 
when default scenarios become more frequent. 

In the DSR and IRC pricing engine, the recovery in the event of default is under the recovery of treasury assumption. That is, if issue defaults at time t , the bond present value is t t PV  R  cf , 
where t cf is the remaining cash flows (or the treasury coupon bond value at the default time). This recovery of treasury assumption is consistent with the risky straight bond pricing formula by setting 
the cumulative default probability 


References:

[Hcommons Put](https://works.hcommons.org/records/aeqwe-48926/files/putprotection.pdf?download=1)

[Hcommons gold](https://works.hcommons.org/records/fvxgt-tbe11/files/goldoption.pdf)



