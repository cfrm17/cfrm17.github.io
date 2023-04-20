## Financial Market Analysis


### Derivatives Pricing Models

[Reference](https://finpricing.com/FinPricing-ProductBrochure.pdf)



### Ratchet Swap

A ratchet swap is an interest rate swap with two legs. One leg is a standard floating leg and the other leg is a ratchet leg. The ratchet leg pays a ratchet floating rate.

The ratchet floating rate coupon is based on an index, e.g., 6-month EURIBOR. The rate is further subject to a minimum decrease of 0 bps and a maximum increase of a threshold, such as, 15 bps. These rates are reset two business days prior to the first day of each coupon period. 



References: 

[OSF ratchet swap](https://osf.io/azy78/download)



### Hull-White Volatility Calibration

In Black’s framework, a European swaption is at the money if the strike level is equal to the forward swap rate. In this case, the prices of a payer and a receiver swaption on the same underlying swap will be equal. 

Mortgages are mapped to short rate volatilities, in order to value the embedded prepayment option. An open mortgage is a mortgage that allows the mortgagee to refinance at any time after a specified date; we will call this date the first exercise date.

Hull-White (HW) short interest rate volatilities are calibrated via at the money European swaptions. 


References: 

[OSF HW vol](https://osf.io/q6sv3/download)



### Quanto CMS Spread Swap

A quanto CMS spread swap is an exotic interest rate swap. The swap consists of two legs: One leg is a fixed rate leg. The other leg pays a fixed rate during a portion of the tenor and a variable rate during the remaining part. The variable rate is based on a spread between GBP and EURO 10 year CMS rates. Depending on the deal, the floating rate payments may last up to 20 years.


References: 

[OSF HW vol](https://osf.io/umeq3/download)


### LIBOR Rate Model

LIBOR Rate Model is used for pricing Libor-rate based derivative securities. The model is applied, primarily, to value instruments that settle at a Libor-rate reset point.  In order to value instruments that settle at points intermediate to Libor resets, we calculate the numeraire value at the settlement time by interpolating the numeraire at bracketing Libor reset points. 


References: 

[OSF HW vol](https://osf.io/wra62/download)



### Credit Valuation Adjustment

As a consequence, the International Accounting Standard (IAS) 39 requires banks to provide a fair-value adjustment due to counterparty risk. Although credit value adjustment (CVA) became mandatory in 2000, it received a little attention until the recent financial crises in which the profit and loss (P&L) swings due to CVA changes were measured in billons of dollars. Interest in CVA began to grow. Now CVA has become the first line of defense and the central part of counterparty risk management.

References:

[core cva pdf](https://core.ac.uk/download/328766597.pdf)



### LMM

The LIBOR Market Model (LMM) is an interest rate model based on evolving LIBOR market forward rates under a risk-neutral forward probability measure. In contrast to models that evolve the instantaneous short rates or instantaneous forward rates, which are not directly observable in the market, the objects modeled using the LMM are market observable quantities. The explicit modeling of market forward rates allows for a natural formula for interest rate option volatility that is consistent with the market practice of using the formula of Black for caps. It is generally considered to have more desirable theoretical calibration properties than short rate or instantaneous forward rate models.

References:

[core lmm pdf](https://core.ac.uk/download/288179622.pdf)




### Convertible Bond Valuation

A company can raise capital in financial markets either by issuing equities, bonds, or hybrids. From an investor’s perspective, convertible bonds with embedded optionality offer certain benefits of both equities and bonds, they have the potential for capital appreciation and like the latter, they offer interest income and safety of principal. The convertible bond market is of primary global importance. 

References:

[core convertible](https://core.ac.uk/download/214006918.pdf)



### Bilateral Credit Risk

Pricing defaultable derivatives or pricing the counterparty credit risk is a
relatively new area of derivatives modeling and trading. Credit value adjustment (CVA)
allows us to quantify counterparty credit risk as a single, measurable Profit & Loss
number. By definition, CVA is the difference between the risk-free trade value and the
true (or risky or defaultable) trade value that takes into account the possibility of
counterparty’s default. Commonly, the CVA is not paid as a lump-sum upfront
premium, but rather is structured into a funding spread. The risk-free trade value is
what brokers quote or what trading systems or models normally report. The
defaultable trade value, however, is a relatively less explored and less transparent
area, which is the main challenge and core theme for credit risk adjustment

References:

[core bilateral](https://core.ac.uk/download/534863091.pdf)




### Jump Diffusion

The jump-diffusion model was first introduced by Merton (1976) in the market risk context for modeling asset price behavior that incorporates small day-to-day diffusive movements together with larger randomly occurring jumps. Over the last decade, people attempt to propagate the model from the market risk domain to the credit risk arena. 

References:

[core jump](https://core.ac.uk/download/328766602.pdf)




### Pricing Credit Risk

Central to the reduced-form models is the assumption that multiple defaults are independent conditional on the state of the economy. In reality, however, the default of one party might affect the default probabilities of other parties. People find that a major credit event at one firm is associated with significant increases in the credit spreads of other firms. People also find that a defaulting firm can weaken the firms in its network of business links. These findings have important implications for the management of credit risk portfolios, where default relationships need to be explicitly modeled.

References:

[core multiple](https://core.ac.uk/reader/334593150)




### Incremental Risk Charge Modeling

The constant level of risk reflects recognition by regulators that securities/derivatives held in the trading book are generally much more liquid than those in the banking book, where a buy-and-hold assumption over one year may be reasonable. It implies that IRC should be modeled under the assumption that banks rebalance their portfolio several times over the capital horizon in order to maintain a constant risk profile as market conditions evolve. Of course, we do not suggest that the constant level of risk framework be taken literally as a model of banks’ behavior: clearly portfolios are altered on a daily basis, not simply held constant for some period then instantaneously rebalanced. Rather, we regard the rollover interpretation as being a reasonable approximation to the way banks manage their trading portfolios over a certain horizon. In general, one should model constant level of risk instead of constant portfolio over one year capital horizon.

References:

[core irc](https://core.ac.uk/download/334593149.pdf)




### CDS Counterparty Risk

We study the sensitivity of the price of a defaultable instrument to changes in the joint credit quality of the parties. For instance, our analysis shows that the effect of default dependence on CDS premia from large to small is the correlation between the protection seller and the reference entity, the comrelation, the correlation between the protection buyer and the reference entity, and the correlation between the protection buyer and the protection seller.

References:

[core cds](https://core.ac.uk/download/334593149.pdf)



### Commodity Price Modeling

The article presents a multi-factor model for pricing commodity derivatives. A primary application is to price commodity swaptions. Swaptions are a relatively illiquid product in commodities market, and the natural flow tends to be one-sided. As a result, dealers typically warehouse long swaption risks. Delta and Vega of these swaptions can be effectively hedged with liquid vanilla options and futures.

References:

[core commodity](https://core.ac.uk/download/533453681.pdf)


### Lookback Call Option 

A model is presented for pricing a European lookback call option on a stock index with guaranteed exchange rate (LBCGER).  In addition a sampling frequency (e.g., daily, weekly, etc.) over the lookback window is specified.


References:

[More details](lookbackCall.md)



### Conditional Probability of Hitting Barrier

A model is developed for evaluating the conditional probability of hitting an upper barrier before a lower barrier, and vice versa, for a tied down geometric Brownian motion with drift. The method produces an analytical value for this probability, assuming that the barrier levels are constant and continuously monitored.


References:

[More details](barrierProb.md)



### Monte Carlo Multi-factor Short Rate Model

The Monte Carlo Multi-factor Short Rate Mode has been used extensively in pricing a variety of interest rate derivative securities. The model assumes that short rates at reset times are lognormally distributed.


References:

[More details](mcShort.md)



### Delta Gamma Vega Value at Risk

The Delta Gamma Vega (DGV) methodology is developed to estimate Value-at-Risk (VaR) for portfolios of equities and equity options in order to comply, in regard to market risk measurement. The model can accurately estimates over-night VaR for portfolios with non-zero convexity or linear risk.


References:

[More details](dgvVaR.md)



### Better-of Cliquet Option 

A model is developed for pricing a swap with better of cliquet option. The floating amount payer makes semi-annual payments based on USD-LIBOR-BBA minus a spread. The fixed rate payer makes a single payment at swap maturity based on the arithmetic average of the S&P 500 Index price over certain pre-specified windows of ten consecutive trading days.


References:

[More details](betterCliquet.md)



### Asian Swap 

A commodity swap is a deal where counter-parties exchange fixed payments for floating payments monthly based on a specific commodity, for example, West Texas Intermediate (WTI) crude oil. The fixed payments are specified as a given quantity times a fixed price; the floating payments are specified as a given quantity times the spot value of the commodity on the payment date. The floating payments may also be based on the arithmetic average of spot commodity price (Asian commodity-price) over the payment period or LIBOR plus a spread.


References:

[More details](asianSwap.md)



