
## Market Risk

References:

[Hcommons](https://derivatives.hcommons.org/2023/03/24/market-risk/)


### Market Risk Flow

In the Risk Measurement Data Flow, positions are valued using models and market inputs. The valuation process is enhanced via Independent Price Valuation (IPV), Valuation Adjustments (VA) and proxy bookings. The valuation process then feeds profit and loss (P&L) and Risk which can be connected through the P&L Attribution (PAA). Market risk measures and diagnostics, such as VaR, are an outcome from the risk measures. This forms the cornerstones of the Market Risk Measurement Management and Data Review Process.

The Market Risk Measurement Management and Data Review Process establishes the linkages which are required in an effective risk management system. All data composing these linkages can theoretically trace dependencies back to market inputs and position inputs. Market inputs are defined as the inputs required in the valuation model that are dynamic in nature and are sourced from markets. As an input to the risk process, the positions require thorough review and validation processes to ensure completeness and consistency. The set of inputs required for valuation should also be employed for other calculations such as P&L attribution (PAA) and should be simulated when computing Value at Risk (VaR).


References: 

[More details](riskFlow.md)

[Studylib flow](https://studylib.net/flashcards/set/market-risk-data-flow_255525)

[Readkong flow](https://www.readkong.com/page/aabd2bbe43e94b494f6b7de3f61c2c77-4897149)

[Bitbucket flow](https://bitbucket.org/timxiao1203/market-risk-data-flow/downloads/MarketRiskDataFlow.pdf)



### Profit and Loss Explanation

Market data accuracy will also improve significantly with the common set of pricing models which allows for direct re-use of official valuation market data (sourcing from the Front Office and Global Middle Office databases, and Valuation Product Control group). This will significantly reduce the complexity of managing multiple market data sources. All market data required for daily valuation is to be saved in databases which are accessible to the relevant Market Risk teams. Data used to compute P&L, PAA,  BT and shocks used in VaR should be the same.

The identification and selection of market risk factors to be captured in a risk model, such as VaR, are critical to building strong risk measurement platform. The Risk Management Completeness Review Stream will be responsible for regular validation of the risk factors. Risk factors are market variables which are expected to impact valuation P&L. In VaR, “risk factors” also define the returns which are simulated and subsequently mapped to market instruments. 


References: 

[More details](pnl.md)

[Studylib PnL](https://studylib.net/flashcards/set/profit-and-loss-explanation_255531)

[Readkong PnL](https://www.readkong.com/page/profit-and-loss-explanation-6423884)

[Bitbucket PnL](https://bitbucket.org/timxiao1203/profit-and-loss-explanation/downloads/PnLExplain.pdf)



### Backtest Exception

The backtest P&L calculations are based on the actual day-over-day changes in market inputs observed.  The market inputs must be the same as those used for official valuation thereby establishing a direct linkage to P&L. 

Root cause investigations are required to validate instances of backtest exceptions. Investigation documentation should be prepared, including the root cause, the analysis performed to find the root cause, and the follow-up actions to be taken, if any. 

Exceptions may be classified as legitimate, or false. For instances where the exceptions are deemed as false, such as spurious market data input, and IT system issues, appropriate operational procedures need to be followed for issue resolution including reruns, market data 


References: 

[More details](backtestEx.md)

[Studylib backtest exception](https://studylib.net/flashcards/set/backtest-exception_255532)

[Readkong backtest exception](https://www.readkong.com/page/862c0ea2b888a978f7149403f1fef68f-8915848)

[Bitbucket backtest exception](https://bitbucket.org/timxiao1203/backtest-exception/downloads/BacktestException.pdf)



### Independent Price Verification

VPC holds a month-end meeting to review all IPV/VA with representatives from the line of business (LOB), Capital Markets Finance, Chief Accountant’s Group, and Risk Oversight. A report is distributed outlining the IPV and VA balances and month over month changes. Detailed reports for each LOB are also available.

VPC will identify material IPV and VA balance for each portfolio (as defined by a unique limit letter) that have a potential impact on VaR. Materiality will be set at total IPV adjustment or total VA greater than $1MM per portfolio. Note that individual rather than net IPV and VA balances should be reviewed as there may be offsetting effects within a portfolio.

References: 

[Studylib vpc](https://studylib.net/flashcards/set/independent-price-verification_255533)

[Readkong vpc](https://www.readkong.com/page/independent-price-verification-3995317)

[Bitbucket vpc](https://bitbucket.org/timxiao1203/price-verification/downloads/IndependentValidation.pdf)




### All-In Gamma Shocks

Generate scenarios for the market instruments corresponding to the base and spread curves

Given the base and spread scenarios, those for the all-in curve can be generated and should be mapped according to spread name and contract date.  For instance, in the example above the AECOM: 201404 AllIn point would take absolute change from the AECOM: 201404 contract, and the base relative change and closing-rate from the NG: 201404

Using these scenarios, the absolute change for the all-in curve is constructed 

References: 

[Studylib gamma shock](https://studylib.net/flashcards/set/constructing-all-in-gamma-shocks_255534)

[Readkong gamma shock](https://www.readkong.com/page/11bc376ef34263cc95154937c512ed8e-2460064)

[Bitbucket gamma shock](https://bitbucket.org/timxiao1203/constructing-all-in-gamma-shocks/downloads/GammaShock.pdf)



### Commodity Risk Factor Translation

The goal of this work is to translate or convert simulated risk factors into market observables. There are three translations in commodity framework: price translation, volatility translation, and all-in translation.

References:

[Studylib commodity translation](https://studylib.net/flashcards/set/commodity-simulation-translation_256082)

[Readkong commodity translation](https://www.readkong.com/page/d68646898b227610dd91dc66cd6cf4bd-8643543)

[Bitbucket commodity translation](https://bitbucket.org/timxiao1203/commoditytranslation/downloads/CommodityTranslation.pdf)



### Commodity Volatility Closing Rate

We use the Omega type models to model the implied volatility skew for commodity derivatives.  These surfaces are incorporate moneyness and time to maturity into the skew definition and are a function of calibrated parameters (skew, wing, boost etc).

References:

[Studylib commodity vol](https://studylib.net/flashcards/set/commodity-volatility-closing-rate-calculation_256102)

[Readkong commodity vol](https://www.readkong.com/page/f3e7fc493b351fb59e863391afeda09e-5813799)

[Bitbucket commodity vol](https://bitbucket.org/timxiao1203/volrate/downloads/CommodityVol.pdf)



### Precious Metal Futures Basis

Futures contracts are typically valued as a spread to the forwards curves.  This spread is the EFP (Exchange of Futures for Physical).  This function spec outlines the introduction of this spread as a basis risk factor into system and the transformation of sensitivities with respect to futures contracts to those with respect the spot contract, forward offered rates, and basis.

References:

[Studylib PM basis](https://studylib.net/flashcards/set/precious-metal-futures_256119)

[Readkong PM basis](https://www.readkong.com/page/ddd68d14959f38d5317e09c5be9e4d30-4962003)

[Bitbucket PM basis](https://bitbucket.org/timxiao1203/pmfutures/downloads/PreciousMetalFutures.pdf)



### Dividend Risk

OSFI recommended that dividend risk should be captured in market risk framework. To achieve that, a dividend risk model is developed by Market Risk (MR) and will be implemented in system. The model calls for the introduction of new dividend risk factors as the expected dividend amount of an equity asset, either a stock, or a basket of stocks, or an equity index. 

References:

[Studylib dividend risk](https://studylib.net/flashcards/set/dividend-risk_256120)

[Readkong dividend risk](https://www.readkong.com/page/44229fa074278a10cf9dfc6d638efd1f-9446385)

[Bitbucket dividend risk](https://bitbucket.org/timxiao1203/dividendrisk/downloads/DividendRisk.pdf)



### Dividend Exposure Measurement 

The proposal is to capture the dividend risk under normal market conditions. Stress test is considered a more appropriate approach to capture the risk of severe cutting or eliminating dividend of large blue chip stocks during financial crisis.

References:

[Studylib dividend exposure](https://studylib.net/flashcards/set/dividend-exposure-measurement-and-management_256121)

[Readkong dividend exposure](https://www.readkong.com/create/preview/e66f03a99516814b5ac50b8d9777f4f9-7267783)

[Bitbucket dividend exposure](https://bitbucket.org/timxiao1203/dividendexposure/downloads/DividendExposure.pdf)



### Dividend Risk Modeling 

In practice, most traders treated dividend amount as “known” and risk managers do not monitor the price sensitivity to dividend amount as long as the total price sensitivity to underlying asset price is properly captured in case the dividend yield is used in pricing. If they think there is any dividend risk, that is only associated with the big negative jumps described above. Stress test, rather than daily VaR, is a proper way to capture that kind of risk.

References:

[Studylib dividend model](https://studylib.net/flashcards/set/dividend-risk-modeling-and-methodology_256122)

[Readkong dividend model](https://www.readkong.com/create/preview/46b214dd09912278e2a2be4a6a5e5e26-4427754)

[Bitbucket dividend model](https://bitbucket.org/timxiao1203/dividendmodel/downloads/DividendModel.pdf)



### Dividend Risk Model Calibration

As described in model description and calibration of the model, the daily innovation to expected dividend of an index is simulated from double exponential distribution with specified correlation with all other risk factors. The daily innovation to expected dividend of a single stock is simulated on the fly without correlation with other risk factors. 

References:

[Studylib dividend Calibration](https://studylib.net/flashcards/set/dividend-risk-model-calibration_256123)

[Readkong dividend Calibration](https://www.readkong.com/page/37d55160d761971bfc351a91a735edab-1838459)

[Bitbucket dividend Calibration](https://bitbucket.org/timxiao1203/dividendcalibration/downloads/dividendCalibration.pdf)

