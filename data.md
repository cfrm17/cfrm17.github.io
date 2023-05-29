## Market Data

[Reference](https://derivatives.hcommons.org/2022/07/26/derivatives-modeling/)

### Yield Curve Introduction

The term structure of interest rates, also known as yield curve, is defined as the relationship between the yield-to-maturity on a zero 
coupon bond and the bond’s maturity. Zero yield curves play an essential role in the valuation of all financial products. 
			
Yield curves can be derived from government bonds or LIBOR/swap instruments. The LIBOR/swap term structure offers several advantages over government 
curves, and is a robust tool for pricing and hedging financial products.  Correlations among governments and other fixed-income products have declined, 
making the swap term structure a more efficient hedging and pricing vehicle.

Zero rate curves, also called spot rate curves, are special and dominant type of yield curves. By definition, a zero rate curve is the 
term structure of the yields-to-maturity of zero coupon bonds. Given a zero rate,

[More details](/IrCurveIntroduction-1.pdf)

[OSF curve](https://osf.io/dx584/download)

[OSF collateral](https://osf.io/preprints/inarxiv/dwz2m/download)

[Github digital](https://github.com/timxiao1203/DigitalOption)

[Zenodo swap curve](https://zenodo.org/record/6494992/files/Zenodo-IrCurveIntroduction.pdf)


### Yield Curve Construction

Zero curves are derived or bootstrapped from observed market instruments that represent the most liquid and dominant interest rate products for certain time horizons.
Normally the curve is divided into three parts. The short end of the term structure is determined using LIBOR rates. The middle part of the curve is constructed using 
Eurodollar futures or forward rate agreements (FRA). The far end is derived using mid swap rates. The objective of the bootstrap algorithm is to find the zero zero or 
discount factor for each maturity point and cash flow date sequentially so that all curve instruments can be priced back to the market quotes.
All bootstrapping methods build up the term structure from shorter maturities to longer ones.

Once we independently apply the above procedure for each of the three mod groups, we
end up with three series of discount factors at three disjoint series of offset dates. We also
have the discount factors at the cash dates. We form the final set of curve anchor dates
from all offset dates and all cash dates. So, we obtain discount factors at all anchor dates.
At any intermediate date we produce a discount factor by interpolating between the
discount factors at the nearest (left and right) neighboring anchor dates.


[OSF curve construction](https://osf.io/3xrs5/download)

[OSF cva](https://osf.io/preprints/inarxiv/9765p/download)

[Github short curve](https://github.com/timxiao1203/ShortTermCurve)

[Zenodo curve](https://zenodo.org/record/6498116/files/Zenodo-IrCurve.pdf)


### Basis Curve

Basis curves are used as the forecast curves for pricing interest rate products. The increase in basis spreads has resulted in large impacts on non-standard instruments.
The basis curve construction methodology is based on the most liquid market instruments. Normally a basis curve is divided into two parts. The short end of the term 
structure is determined using LIBOR rates and the remaining is derived using basis swaps.

[Zenodo basis swap](https://zenodo.org/record/6588375#.YpEh86gpDq4)

[OSF convertible](https://osf.io/preprints/inarxiv/zv2xe/download)

[Github fund](https://github.com/cfrm17/FundExposure-)

[FlipHtml5 basis](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamgTM2kzM2ITPkl0av9mY)

[Zenodo basis curve](https://zenodo.org/record/6498212/files/Zenodo-IrBasisCurve.pdf)


### OIS Curve

Overnight index swaps (OIS) curves became the market standard for discounting collateralized cashflows. The reason often given for using 
the OIS rate as the discount rate is that it is derived from the fed funds rate and the fed funds rate is the interest rate usually paid 
on collateral. As such the fed funds rate and OIS rate are the relevant funding rates for collateralized transactions.
			
Many banks now consider that overnight indexed swap (OIS) rates should be used for discounting when collateralized portfolios are valued and that 
LIBOR should be used for discounting when portfolios are not collateralized.

The reason often given for using the OIS rate as the discount rate is that it is derived from the fed funds rate and the fed funds rate 
is the interest rate usually paid on collateral. As such the fed funds rate and OIS rate are the relevant funding rates for collateralized 
transactions.

[More details](/IrOIS-4.pdf)

[FlipHtml5 ois](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamETN0MDN2ITPkl0av9mY)

[Github principal](https://github.com/cfrm17/PrincipalNote-)

[OSF diffution model](https://osf.io/preprints/inarxiv/zxk7w/download)

[Zenodo ois](https://zenodo.org/record/6498443/files/Zenodo-IrOIS.pdf)



### Forex Volatility

An implied volatility is the volatility implied by the market price of an option based on the Black-Scholes option pricing model. A volatility surface 
is derived from quoted volatilities that provides a way to interpolate an implied volatility at any strike and maturity. Unlike in other markets that 
quote volatility versus strike directly, the FX smile is given implicitly as a set of restrictions implied by market instruments and as such a calibration 
procedure to construct a volatility- delta or volatility-strike smile is used.

[Github collateralized swap](https://github.com/cfrm17/CollateralizedSwap)

[OSF test](https://osf.io/preprints/inarxiv/qh7vj/download)

[Zenodo fx vol](https://zenodo.org/record/6499323/files/Zenodo-FxVol.pdf)



### Swaption Volatility

An interest rate swaption volatility surface is a four-dimensional plot of the implied volatility of a swaption as a function of strike and expiry and tenor. 
The term structures of implied volatilities which provide indications of the market’s near- and long-term uncertainty about future short- and long-term swap rates. 
A crucial property of the implied volatility surface is the absence of arbitrage.

[Github HF VaR](https://github.com/cfrm17/HedgeFundVaR)

[OSF determination](https://osf.io/preprints/inarxiv/n29s7/download)

[Zenodo swaption vol](https://zenodo.org/record/6499360/files/Zenodo-IrSwnVol.pdf)


### Cap Implied Volatility

An implied volatility is the volatility implied by the market price of an option based on the Black-Scholes option pricing model. In cap market, 
a cap/floor is quoted by implied volatilities but not prices. An interest rate cap volatility surface is a three-dimensional plot of the implied 
volatility of a cap as a function of strike and maturity. 

In market, a cap/floor is quoted by implied volatilities rather than prices. An interest rate cap volatility surface is a three-dimensional 
plot of the implied volatility of a cap as a function of strike and maturity. 

ol skew or smile pattern is directly related to the conditional non-normality of the underlying returns. In particular, a smile reflects 
fat tails in the return distribution whereas a skew indicates asymmetry. A crucial property of the implied volatility surface is the 
absence of arbitrage.



[More details](/IrCapVol-7.pdf)

[FlipHtml5 cap vol](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamMzN0ITN2ITPkl0av9mY)

[Github barrier](https://github.com/cfrm17/HedgeFundBarrierOption)

[OSF irc](https://osf.io/preprints/inarxiv/f6v43/download)

[Zenodo cap vol](https://zenodo.org/record/6502573/files/Zenodo-IrCapVol.pdf)



### FX Foward Spreads

FX forward curve is also called FX implied forward curve or FX derived curve. It is derived from USD zero rate curve and FX forward spreads and used 
to value FX trades. Market standard is to use FX quoted forward spreads and USD zero rate curve to generate FX implied forward curve. In other words, 
FX curve construction generates an interest rate curve of the quoting currency from the interest rate curve of the base currency. The construction 
methodology is based on the arbitrage-free relationship between forward FX rates and the discount rates of the two currencies.


[Gitbook fx spreads](https://cfrm17.gitbook.io/fx-forward-curve-introduction/)

[OSF multiple](https://osf.io/preprints/inarxiv/3p7fy/download)

[Github Mortgage](https://github.com/cfrm17/AdjustableRateMortgages)

[Zenodo fx spreads](https://zenodo.org/record/6502685/files/Zenodo-FxForwardCurve.pdf)



### Inflation Curve

Inflation curve or inflation forward curve is also called Consumer Price Index (CPI) curve that is the term structures of CPI rates is defined as 
the relationship between CPI and different terms. The popular indices are Euro HICPxT, UK RPI, and US CPI. Inflation curves are used to price inflation 
securities and inflation derivatives, such as inflation linked bonds, inflation swaps and inflation caps/floors.


[Zenodo inflation curve](https://zenodo.org/record/6502757/files/Zenodo-IrInflationCurve.pdf)

[Gitbook inflation curve](https://cfrm17.gitbook.io/forward-inflation-curve/)

[OSF impact](https://osf.io/preprints/inarxiv/chjxe/download)

[Github Index](https://github.com/cfrm17/HedgeFundIndex)



### Inflation Linked Bond Curve

Inflation indexed bonds, also called inflation linked bonds or real return bonds, are bonds where the principal is indexed to inflation or deflation 
on a daily basis in terms of a reference index, such as Consumer Price Index (CPI). The primary purpose of these bonds is the transfer of inflation risk.

An inflation indexed bond is designed to hedge the inflation risk of the bond. Inflation bonds are an important vehicle for investors 
hose liabilities indexed to changes in inflation or wages. They have favorable performance and lower volatility relative to other risk 
assets. It is favorable to retirement planning and pension funds given its inflation protection. Inflation indexed bonds are less liquid 
than regular bonds.

Inflation linked bonds are mainly issued by government. There is also a small portion of inflation-linked bonds are issued by commercial 
financial institutions, that are usually treated as government-issued inflation-linked bonds.

[More details](/FiInflationBondCurve-10.pdf)

[Zenodo inflation bond curve](https://zenodo.org/record/6502866/files/Zenodo-FiInflationBondCurve.pdf)

[Github trust swap](https://github.com/cfrm17/TrustSwap)

[Gitbook inflation bond curve](https://cfrm17.gitbook.io/inflation-linked-bond-curve/)

[OSF swap](https://osf.io/preprints/inarxiv/f98aq/download)


### Treasury Benchmark Curve

Treasury curve or treasury benchmark curve is the term structures of treasury bill/bond prices vs maturities. The two major types of marketable s
ecurities issued by government are treasury bills and treasury bonds. Treasury bills, that do not pay coupons but rather are issued at a discount 
and mature at their par value, are issued at short terms. Issurance occurs through a competitive auction.

[Github asset](https://github.com/cfrm17/AssetsHedge)

[Zenodo treasury benchmark curve](https://zenodo.org/record/6505581/files/Zenodo-FiTreasuryCurve.pdf)

[OSF derivatives](https://osf.io/preprints/inarxiv/9765p/download)



### Treasury Yield Curve

Treasury yield curve or treasury zero coupon yield curve is the term structures of treasury yields-to-maturity. The yield is also called the zero coupon 
rate or the implied forward rate. Treasury yield curves are bootstrapped from treasury benchmark curves that contain the most actively traded treasury bills 
or bonds at some maturities. There are four elements in interest rate: zero coupon rates (or zero rates), discount factor, par yields, and forward rates. 
The derivation of one of these element is conveniently sufficient for the determination of the other three elements. Each interest rate definition is derived 
from specific representations of bond price.

[Github cash hedge](https://github.com/cfrm17/CashFlowHedge)

[Zenodo treasury yield](https://zenodo.org/record/6505850/files/Zenodo-FiTreasuryYieldCurve.pdf)



### SIFMA Curve

SIFMA (Securities Industry and Financial Markets Association) is a trading organization in US. The SIFMA Municipal Swap Index, formerly the Bond Market Association Index, 
is a market index composed of tax-exempt variable rate demand obligations (VRDOs). VRDOs are municipal bonds with floating interest rates. The SIFMA index is issued weekly. 
The SIFMA rate for each interest payment period is equal to the weighted average of the SIFMA index value. Both SIFMA and LIBOR are popular floating rate index. The SIFMA 
rate represents the average interest rate payable on tax-exempt variable rate demand obligations, while the LIBOR rate represents the interest rate payable on non-tax exempt 
demand obligations. In general, the SIFMA rate trades as a proportion of LIBOR rate.


[Github fair hedge](https://github.com/cfrm17/FairValueHedge)

[Zenodo sifma curve](https://zenodo.org/record/4313794/files/FiSifmaCurve-13.pdf)



### Cross Currency Basis Curve

Cross currency swap differs from single currency swaps in that the interest rate payments on the two legs are in different currencies. At inception 
of the trade, the notional principal amounts in the two currencies are usually set to be fair given the spot exchange rate. Contrary to single 
currency swap, there is an exchange of principals at inception and maturity, or even in each period of the swap.

Cross currency swaps are powerful instruments to transfer assets or liabilities from one currency to another. The market charges for 
this is a liquidity premium – the cross-currency basis spread. Thus, the market quoted cross-currency basis spreads usually relative 
to a liquidity benchmark. 

For a cross currency trade between one currency and another currency. If there is a higher demand for the currency, the party lending 
the dollar will ask for a premium. This premium is referred to as the cross currency basis. In general, the cross currency basis is 
a measure of the dollar shortage in the market. The more negative the basis is, the more severe the shortage.


[More details](/IrXccyBasisCurve-14.pdf)

[FlipHtml5 cross currency basis curve](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamUDMwEDMzMTPkl0av9mY)

[Github acquisation](https://github.com/cfrm17/PortfolioAcquisition)

[Zenodo xccy curve](https://zenodo.org/record/6506359/files/Zenodo-IrXccyBasisCurve.pdf)




### Precious Metal Volatility

Precious metals are trading commodities. But a precious metal quote is very similar to a Forex quote. The quote is represented in the same way 
as a quote for a currency pair. For instance, the spot gold traded against the US dollar is XAU/USD. An implied volatility is the volatility implied 
by the market price of an option based on the Black-Scholes option pricing model. A volatility surface is derived from quoted volatilities that provides 
a way to interpolate an implied volatility at any strike and maturity. Unlike in other markets that quote volatility versus strike directly, 
the precious metal or FX smile is given implicitly as a set of restrictions implied by market instruments and as such a calibration procedure to construct 
a volatility- delta or volatility-strike smile is used.


[Github mbs defer](https://github.com/cfrm17/MBSDeferredAsset)

[Zenodo precious metal volatility](https://zenodo.org/record/4407401/files/CmcPreciousMetalVol-15.pdf)




### Credit Spread Curve

There is only one base interest rate per currency, corresponding to the bank’s unsecured lending/borrowing rate (such as LIBOR). The interest rate used to discount 
cashflows may include a credit spread above or below the base rate. Credit spread can be derived by either structural model or reduced-form (intensity) model. 
The structural approach regards default as an endogenous event by focusing on the capital structure of the firm. Whereas the reduced-form approach does not explain 
the event of default endogenously, but characterizes it exogenously by a jump process.

[Github commitment](https://github.com/cfrm17/MortgageCommitment)

[Zenodo credit spread](https://zenodo.org/record/6506537/files/Zenodo-CrCreditSpread.pdf)



