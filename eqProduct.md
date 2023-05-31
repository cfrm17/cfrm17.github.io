## Equity Products


[Github Tim References](https://github.com/timxiao1203?tab=repositories)


### Stable Value Wrap Model

The stable value model is aimed at estimating the value of providing protection on a portfolio consisting of fixed income and equity instruments.  The fund upon which stable value protection is provided is assumed to be under active management and thus to have a constant duration for the purposes of modeling.  The protection provided by the stable value contract is written on any shortfall between the market value of the fund and a defined “book value” which exists when redemptions of the fund are made.

The book value of the fund is computed as a function of the “crediting rate”, which itself is a function of previous market and book values as well as the equity and/or fixed income indices that indicate the market value of the fund.

References: 

[Zenodo Stable Model pdf](https://zenodo.org/record/7542104/files/stableValueModel.pdf)

[Zenodo Stable Model](https://zenodo.org/record/7542104)

[Github Stable Model](https://github.com/cfrm17/boliFund)



### Credit Default Simulator

The model is designed to take into account credit enhancements in several forms.  The first such form of enhancement is a subordinated tranche, which can be set to an arbitrary percentage of the total face value of the asset pool.  The second type of enhancement is the excess spread.  This is effectively a coupon on the remaining total face value of the pool which is paid into an account.  The balance of this account is deducted from the total default losses in each period, and the excess spread account balance is reset.  The third enhancement is the reserve account, which functions identically to the excess spread, except that payments to the reserve account stop when a specified maximum value is reached.

References:

[Zenodo Credit Simulator pdf](https://zenodo.org/record/7542156/files/creditDefaultSimulator.pdf)

[Zenodo Credit Simulator](https://zenodo.org/record/7542156)

[Github Credit Simulator](https://github.com/cfrm17/defaultSimulator)



### Conduit Administration Fees 

One potential problem is that observed conduit administration fee data is not corrected for reconsideration events. Displayed trending may actually be attributable to this fact. Results from further quantitative tests using supplied reconsideration event data are consistent with this theory. Ultimately, qualitative arguments based on knowledge of conduit fee evolution are needed to address the stationarity of the US conduits. Given the stationary property however, using a lognormal model for all of the conduits appears reasonable based on the Jarque-Bera results obtained using currently available fee data.

Projected fee values are required to receive preferential accounting treatment. A basic stationary process with an appropriate volatility was approved to forecast the conduit administration fees. This certification was made based on the historical data available at the time 

References:

[Zenodo Conduit Fee pdf](https://zenodo.org/record/7548994/files/ConduitAdministrationFees.pdf)

[Zenodo Conduit Fee](https://zenodo.org/record/7548994)

[Github Conduit Fee](https://github.com/cfrm17/ConduitAdministrationFees-)



### Credit Basket Analysis

In the model, names are allowed to migrate ratings on an individual basis according to a credit transition matrix. At the same time, spreads are simulated using mean reverting processes with time dependent parameters. For the purpose of spread evolution, names are grouped into classes of similar credit ratings. This classification simplifies the number of inputs required. Time dependent process parameters allows the inclusion of a spread term structure if desired.

Overall, this model captures the combined stochastic behaviour of both name migrations and spread forecasts. To ensure consistency, all dynamic processes are appropriately correlated with one another. Ultimately, at any simulated time the current basket loss level and pool spread can be used to check for trigger breaches. The portion of first trigger breaches relative to the number of simulated paths is an important measure. It represents an estimate of the probability of ever experiencing a spread trigger breach.

References:

[Zenodo Credit Analysis pdf](https://zenodo.org/record/7566753/files/creditBasketAnalysis.pdf)

[Zenodo Credit Analysis](https://zenodo.org/record/7566753)

[Github Credit Analysis](https://github.com/cfrm17/creditBasketAnalysis)



### Parameter Estimation of Fee Process

Given the strong quantitative evidence from three conduits and strong qualitative evidence from all conduits, we are confident that the fee processes mean-revert in a way that is inconsistent with a geometric Brownian motion assumption.

We are interested in parameter estimation and model selection issues, which ultimately impact
on the expected loss calculations.

We will give an outline of the methodology employed to estimate parameters, and comment on the robustness of the results. We also provide a more realistic methodology for choosing a conservative parameter set 

References:

[Zenodo Fee Estimation pdf](https://zenodo.org/record/7570000/files/FeeProcessParameterEstimation.pdf)

[Zenodo Fee Estimation](https://zenodo.org/record/7570000)

[Github Fee Estimation](https://github.com/cfrm17/feeProcessEstimation)


### Expected Loss Model

The only significant issue is that the State Bank deal has a spread adjustment (SA) that declines from 0.75% to 0.5% in steps of 0.05% over the first 5 years of the deal, whereas the model assumes that SA is fixed throughout the life of the deal. Setting SA=0.75% will result in a conservative exposure calculation, but not necessarily conservative VaR/stress-testing results.

We have added the amortizing spread adjustment to the model and fond that with the current deal parameters (ignoring tax) results in a VaR of _ 3bp, which is underestimates by _ 0.5bp if this adjustment amortization is ignored (as the IPS model does). As the book value of this deal is a relatively small fraction of the entire portfolio (_ 0.3%), this difference is insignificant.

References:

[Zenodo Expected Loss pdf](https://zenodo.org/record/7570310/files/expectedLossModel.pdf)

[Zenodo Expected Loss](https://zenodo.org/record/7570310)

[Github Expected Loss](https://github.com/cfrm17/expectedLoss)


### Portfolio Exposure and Risk 

When performing a VaR calculation, it is not necessarily the case that a conservative assumption in the exposure calculation would necessarily lead to a conservative VaR. That is, assume that we have two approximate (i.e., model-produced) exposure results ˜E1 and ˜E2, resulting from a baseline and VaR or stress-test shift respectively. The ‘actual’ exposures E1 and E2 are not known, but if we have been conservative in our approximations, we know that

References:

[Zenodo Exposure Risk pdf](https://zenodo.org/record/7574314/files/portfilioExposureRisk.pdf)

[Zenodo Exposure Risk](https://zenodo.org/record/7574314)

[Github Exposure Risk](https://github.com/cfrm17/exposureRisk)


### CMBS Valuation 

This involves setting up subordination levels and coupon for the various tranches, together with tranche yields that are ultimately used to value the CMBS.

The subordination levels and yields are input into the system based on recent market activity, while the coupons and specifics of the transaction (e.g. the time tranching of the AAA securities) is determined based on the underlying collateral.

Finally, we use the all this information to project cash flows for the various tranches, and finally value the deal by discounting using the input yields. The actual calculations performed are quite simple, and the largest risk to the model is the parameter inputs (subordination levels and pricing spreads). One needs to ensure that the inputs being used are consistent with the valuation being performed, or that the CMBS structure being considered is consistent with the market data used.

References:

[Zenodo cmbs pdf](https://zenodo.org/record/7574401/files/CMBS.pdf)

[Zenodo cmbs](https://zenodo.org/record/7574401)

[Github cmbs](https://github.com/cfrm17/cmbs)



### Bet Option 

A bet option is a bet on a basket of stocks.  There are multiple reset periods before the maturity of the option.  At the end of each period, if all the stocks in the basket are above their respective strikes, the option will payout a rebate amount for this period at maturity.

[Zenodo bet option pdf](https://zenodo.org/record/7675640/files/BetOption.pdf)

[Zenodo bet option](https://zenodo.org/record/7675640)

[Github bet option](https://github.com/cfrm17/betOption)



### Basket Asian Relative Performance Option 

Monte Carlo simulation associated with stratified sampling variance deduction is employed to evaluate the option.  In the first sample transaction, there are six stocks, one as a reference, and the other five in a basket with equal weight.  These underling stocks and the option are all measured in CAD.

[Zenodo BARPO pdf](https://zenodo.org/record/7675618/files/AsianBasketRpo.pdf)

[Zenodo BARPO](https://zenodo.org/record/7675618)

[Github BARPO](https://github.com/cfrm17/basketAsianRpo)



### Bond Option 

Let B(t)  be a price process of a given bond, and T be a payoff maturity date.  The bond option with the underlying B is a European type derivative security whose matured payoff at the settlement date is given by

[Zenodo bond option pdf](https://zenodo.org/record/7681904/files/BondOption.pdf)

[Zenodo bond option](https://zenodo.org/record/7681904)

[Github bond option](https://github.com/cfrm17/bondOption)



### Bond Futures Option

We present a pricing model for bond futures option. Assuming that the bond futures price at the maturity of the option is lognormal, the model adopts the Black’s analytical closed-form solution.  The futures price is taken directly from the market instead of being calculated from the bond futures calculator.

[Zenodo bond futures option pdf](https://zenodo.org/record/7682025/files/BondFuturesOption.pdf)

[Zenodo bond futures option](https://zenodo.org/record/7682025)

[Github bond futures option](https://github.com/cfrm17/bondFuturesOption)



### Callable Asian Option 

Pricing of callable Asian options involve two stages.  The first stage is for the cases when the current value date is prior to the call date.  This is our focus.  The second is for the cases when the current value date is beyond the call date; in these cases, either the option was called and therefore deceased, or the remaining is just a regular Asian option, which is not in our scope.

[Zenodo callable asian pdf](https://zenodo.org/record/7682078/files/CallableAsian.pdf)

[Zenodo callable asian](https://zenodo.org/record/7682078)

[Github callable asian](https://github.com/cfrm17/callableAsian)


### Term Structure of CDS Curve

On the credit default swap market, a series of spreads with corresponding maturities can be obtained every business day. If the target default swap is forward starting, quarterly calibration payment dates will be generated from the first payment date of the target default swap backward to the value date.  If the target default swap finishes before the last maturity date in the term structure file, quarterly calibration payment dates will be generated from the maturity date of the target default swap forward to the last maturity date in the term structure file.  The payment dates used for calibration are therefore built.

[Zenodo cds curve pdf](https://zenodo.org/record/7729723/files/CdsTermStructure.pdf)

[Zenodo cds curve](https://zenodo.org/record/7729723)

[Github cds curve](https://github.com/cfrm17/CdsTermStructure)


### Credit Default Swap 

A credit default swap is actually an option, which protect the buyer against possible default of an entity, the so-called reference entity. To accomplish this, the buyer of the default swap pays the seller a premium periodically in exchange for a contingent payment in case the reference entity defaults. The contingent payment is the difference between the notional of the swap and the recovery value from the reference entity. 

[Zenodo cds pdf](https://zenodo.org/record/7729965/files/cds.pdf)

[Zenodo cds](https://zenodo.org/record/7729965)

[Github cds](https://github.com/cfrm17/cds)


### Hazard rate calibration

For each bond traded in the market, the credit premium is usually observable but the hazard rate is unobservable. The credit risk premium of a corporate bond can be observed by the difference of the bond yield from benchmark Treasury bond yield of similar duration. Credit risk premium can also be observed from traded credit default swaps. 

[Zenodo hazard pdf](https://zenodo.org/record/7729977/files/hazardRate.pdf)

[Zenodo hazard](https://zenodo.org/record/7729977)

[Github hazard](https://github.com/cfrm17/hazardRateCalibration)


### Quanto Himalayan Option

[More details](/quantoHimalayan.md)



### Callable Inverse Swap

[More details](/callableInverse.md)
