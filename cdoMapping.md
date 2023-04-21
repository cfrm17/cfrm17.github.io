
### CDO Mapping

Mapping CDO2 and CDO3 trades to risk equivalent CDO (RE-CDO) trades can be done by matching the b/e spread a RE-CDO is calculated and taken as the proxy of a target CDO2 or CDO3 trade.  Then the MTM of the CDO2 or CDO3 trade can be calculated using the market observed correlations by finding the MTM of the proxy via index base correlations.

At the present time there is no generally accepted methodology of applying market observed correlation information to a bespoke CDO2 or CDO3 trade. The GSP mapping methodology is similar to the idea of a roughly delta hedging of a CDO2 and CDO3 trade with a CDO trade. The tests have shown that the methodology does capture the most of the market risk of credit spread and correlation if calibrated frequently and has been implemented correctly.

However, we have also indicated that such mapping is not based on a sound theoretical foundation and can only be viewed as an approximation. The approximation is acceptable only when each child mezzanine tranches has very similar risk exposure of correlation and credit. 

The model serves the purpose of finding a proxy CDO for a CDO2 or CDO3 trade by matching b/e spread. The proxy CDO has a collateral pool with the same reference names as that of the CDO2 or CDO3 trade and the notional amount of each name is the average of that of all child CDO pools. It has the same thickness of the tranche as that of the CDO2 or CDO3 trade and its attachment is calculated such that the b/e spread matches that of the CDO2 or CDO3 trade. The MTM of the CDO2 or CDO3 trade can then be calculated using the market observed correlations by finding the MTM of the proxy via index base correlations.

The methodology can be illustrated through the following example. As shown in Figure 1, a CDO2 trade has two child pools with the reference names 8~12 being shared. This CDO2 trade can be mapped to another risk equivalent CDO (RE-CDO) with the pool shown in Fig. 1. In this pool the notional of each reference name is the average of that of two child CDOs.  


References:

[zenodo pdf](https://zenodo.org/record/7363084/files/CDOnMapping.pdf)

[archive curve](https://ia601404.us.archive.org/25/items/bondBootstrapping/bondBootstrapping.pdf)

[github credit](https://github.com/cfrm17/creditBasketAnalysis)

[core digital pdf](https://core.ac.uk/download/534866603.pdf)

[core frtb](https://core.ac.uk/works/126047798)

