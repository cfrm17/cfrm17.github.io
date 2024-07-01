
### Volatility Adjustment Factor Calibration


It is assumed that the distribution of the spread volatility ratio, which is the ratio between issuer-specific spread volatility and its cluster spread volatility, captures the issuer-specific spread risk. And the data 
sample used in the calibration is representative of the market.

The benchmark spread (defined as the average 5-year CDS spreads of all issuers with BBB credit rating) is the key driver for issuer-specific CDS spread in the credit model in AA Studio. The benchmark spread is assumed 
to follow the exponential O-U process

Once the benchmark spread is determined, the transform will be applied to generate generic spread for a given cluster (i.e. industry and rating) and tenor term and then the final issuer-specific spread. Details of the 
transform are in the validation report on CCR Credit Market. However, each individual issuer may have higher or lower level of volatilities than the cluster. For issuers with volatility higher than cluster level, its 
credit exposure tends to be underestimated, while exposure of companies with lower volatilities tends to be overestimated.

In order to capture the issuer-specific spread risk, MD proposes to adjust the benchmark spread volatility according to each issuer’s credit spread volatility. For high risk issuers, their benchmark spread is adjusted 
higher, and vice versa. Once the benchmark spread is simulated, the issuer specific spreads are generated in the same way as defined in the current Adaptive model.

It is assumed that the replacement risk of the interest rate total rate swap (IR TRS) is captured as a combination of an IRS and a CDS in a reasonably accurate way. Recall that the risk factor add-on method is used for 
IR TRS exposure calculation 

Deal-specific liquidity risk is assumed to be captured through scaling method—scaling the exposure using liquidity horizons. Generally, for an IR TRS trade with liquidity horizon〖 LH〗_i, its final exposure is calculated 



References:

[average volatility](https://ia601306.us.archive.org/0/items/averageVol/averageVol.pdf)

[barrier probability](https://ia600203.us.archive.org/31/items/barrierProbabilityNew/barrierProbabilityNew.pdf)

[likelihood ratio](https://ia600600.us.archive.org/7/items/likelihood-ratio/LikelihoodRatio.pdf)





