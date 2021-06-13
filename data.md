## Market Data

### Yield Curve Introduction

The term structure of interest rates, also known as yield curve, is defined as the relationship between the yield-to-maturity on a zero 
coupon bond and the bond’s maturity. Zero yield curves play an essential role in the valuation of all financial products. 
			
Yield curves can be derived from government bonds or LIBOR/swap instruments. The LIBOR/swap term structure offers several advantages over government 
curves, and is a robust tool for pricing and hedging financial products.  Correlations among governments and other fixed-income products have declined, 
making the swap term structure a more efficient hedging and pricing vehicle.

Zero rate curves, also called spot rate curves, are special and dominant type of yield curves. By definition, a zero rate curve is the 
term structure of the yields-to-maturity of zero coupon bonds. Given a zero rate,

[More details](/IrCurveIntroduction-1.pdf)

[OSF curve](https://osf.io/ut5gw/download)

[FlipHtml5 swap curve](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamUTNyITM2ITPkl0av9mY)

[Github swap curve](https://github.com/timxiao1203/SwapCurve)


### Yield Curve Construction

Zero curves are derived or bootstrapped from observed market instruments that represent the most liquid and dominant interest rate products for certain time horizons.
Normally the curve is divided into three parts. The short end of the term structure is determined using LIBOR rates. The middle part of the curve is constructed using 
Eurodollar futures or forward rate agreements (FRA). The far end is derived using mid swap rates. The objective of the bootstrap algorithm is to find the zero zero or 
discount factor for each maturity point and cash flow date sequentially so that all curve instruments can be priced back to the market quotes.
All bootstrapping methods build up the term structure from shorter maturities to longer ones.

[OSF curve construction](https://osf.io/yf2rj/download)

[FlipHtml5 curve construction](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamkDO1kzM2ITPkl0av9mY)

[Hcommons curve construction](https://hcommons.org/deposits/download/hc:34016/CONTENT/ircurve-2.pdf)

[Github curve construction](https://github.com/cfrm17/YieldCurveConstruction)


### Basis Curve

Basis curves are used as the forecast curves for pricing interest rate products. The increase in basis spreads has resulted in large impacts on non-standard instruments.
The basis curve construction methodology is based on the most liquid market instruments. Normally a basis curve is divided into two parts. The short end of the term 
structure is determined using LIBOR rates and the remaining is derived using basis swaps.

[Github basis curve](https://github.com/cfrm17/BasisCurve/raw/main/IrBasisCurve-3.pdf)




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

[OSF ois](https://osf.io/68sc9/download)

[Hcommons ois](https://hcommons.org/deposits/download/hc:34720/CONTENT/irois-4.pdf)


### Forex Volatility

An implied volatility is the volatility implied by the market price of an option based on the Black-Scholes option pricing model. A volatility surface 
is derived from quoted volatilities that provides a way to interpolate an implied volatility at any strike and maturity. Unlike in other markets that 
quote volatility versus strike directly, the FX smile is given implicitly as a set of restrictions implied by market instruments and as such a calibration 
procedure to construct a volatility- delta or volatility-strike smile is used.

[OSF fx vol](https://osf.io/nd4tx/download)

[FlipHtml5 fx vol](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamIjMyYDN2ITPkl0av9mY)



### SwapCurve Volatility

An interest rate swaption volatility surface is a four-dimensional plot of the implied volatility of a swaption as a function of strike and expiry and tenor. 
The term structures of implied volatilities which provide indications of the market’s near- and long-term uncertainty about future short- and long-term swap rates. 
A crucial property of the implied volatility surface is the absence of arbitrage.

[OSF swaption volatilities](https://osf.io/73qk2/download)

[FlipHtml5 swaption volatility](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamYTNyYDN2ITPkl0av9mY)

[Hcommons swaption volatility](https://hcommons.org/deposits/download/hc:35170/CONTENT/irswnvol-6.pdf)




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

[OSF cap vol](https://osf.io/gav3c/download)



### FX Foward Spreads

FX forward curve is also called FX implied forward curve or FX derived curve. It is derived from USD zero rate curve and FX forward spreads and used 
to value FX trades. Market standard is to use FX quoted forward spreads and USD zero rate curve to generate FX implied forward curve. In other words, 
FX curve construction generates an interest rate curve of the quoting currency from the interest rate curve of the base currency. The construction 
methodology is based on the arbitrage-free relationship between forward FX rates and the discount rates of the two currencies.


[Gitbook fx spreads](https://cfrm17.gitbook.io/fx-forward-curve-introduction/)

[Github fx spreads](https://github.com/cfrm17/fxForwardPoints)



### Inflation Curve

Inflation curve or inflation forward curve is also called Consumer Price Index (CPI) curve that is the term structures of CPI rates is defined as 
the relationship between CPI and different terms. The popular indices are Euro HICPxT, UK RPI, and US CPI. Inflation curves are used to price inflation 
securities and inflation derivatives, such as inflation linked bonds, inflation swaps and inflation caps/floors.


[Zenodo inflation curve](https://zenodo.org/record/4299095/files/IrInflationCurve-9.pdf)

[Gitbook inflation curve](https://cfrm17.gitbook.io/forward-inflation-curve/)

[FlipHtml5 inflation curve](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamMzN3gDNyMTPkl0av9mY)

[Github inflation curve](https://github.com/timxiao1203/inflationCurve)




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

[Zenodo inflation bond curve](https://zenodo.org/record/4299106/files/FiInflationBondCurve-10.pdf)

[FlipHtml5 inflation bond curve](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamUTO3gDNyMTPkl0av9mY)

[OSF inflation bond curve](https://osf.io/7ukym/download)

[Gitbook inflation bond curve](https://cfrm17.gitbook.io/inflation-linked-bond-curve/)

[Github inflation bond curve](https://github.com/timxiao1203/inflationBondCurve)


### Treasury Benchmark Curve

Treasury curve or treasury benchmark curve is the term structures of treasury bill/bond prices vs maturities. The two major types of marketable s
ecurities issued by government are treasury bills and treasury bonds. Treasury bills, that do not pay coupons but rather are issued at a discount 
and mature at their par value, are issued at short terms. Issurance occurs through a competitive auction.

[OSF treasury benchmark curve](https://osf.io/umy36/download)

[Zenodo treasury benchmark curve](https://zenodo.org/record/4299113/files/FiTreasuryCurve-11.pdf)

[FlipHtml5 treasury benchmark curve](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamQTM4gDNyMTPkl0av9mY)

[Github treasury benchmark curve](https://github.com/timxiao1203/treasuryBenchmarkCurve)



### Treasury Yield Curve

Treasury yield curve or treasury zero coupon yield curve is the term structures of treasury yields-to-maturity. The yield is also called the zero coupon 
rate or the implied forward rate. Treasury yield curves are bootstrapped from treasury benchmark curves that contain the most actively traded treasury bills 
or bonds at some maturities. There are four elements in interest rate: zero coupon rates (or zero rates), discount factor, par yields, and forward rates. 
The derivation of one of these element is conveniently sufficient for the determination of the other three elements. Each interest rate definition is derived 
from specific representations of bond price.

[OSF treasury yield](https://osf.io/kxrzg/download)

[Zenodo treasury yield](https://zenodo.org/record/4299119/files/FiTreasuryYieldCurve-12.pdf)

[FlipHtml5 treasury yield](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamIjM4gDNyMTPkl0av9mY)

[Github treasury yield](https://github.com/timxiao1203/treasuryYieldCurve)



### SIFMA Curve

SIFMA (Securities Industry and Financial Markets Association) is a trading organization in US. The SIFMA Municipal Swap Index, formerly the Bond Market Association Index, 
is a market index composed of tax-exempt variable rate demand obligations (VRDOs). VRDOs are municipal bonds with floating interest rates. The SIFMA index is issued weekly. 
The SIFMA rate for each interest payment period is equal to the weighted average of the SIFMA index value. Both SIFMA and LIBOR are popular floating rate index. The SIFMA 
rate represents the average interest rate payable on tax-exempt variable rate demand obligations, while the LIBOR rate represents the interest rate payable on non-tax exempt 
demand obligations. In general, the SIFMA rate trades as a proportion of LIBOR rate.


[OSF sifma curve](https://osf.io/x3ygn/download)

[Zenodo sifma curve](https://zenodo.org/record/4313794/files/FiSifmaCurve-13.pdf)

[FlipHtml5 sifma curve](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamcTO5ADMzMTPkl0av9mY)

[Github sifma curve](https://github.com/timxiao1203/sifmaCurve)




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

[OSF xccy curve](https://osf.io/pxu9z/download)

[Zenodo xccy curve](https://zenodo.org/record/4313815/files/IrXccyBasisCurve-14.pdf)

[Github xccy curve](https://github.com/timxiao1203/crossCurrencyBasis)



### Precious Metal Volatility

Precious metals are trading commodities. But a precious metal quote is very similar to a Forex quote. The quote is represented in the same way 
as a quote for a currency pair. For instance, the spot gold traded against the US dollar is XAU/USD. An implied volatility is the volatility implied 
by the market price of an option based on the Black-Scholes option pricing model. A volatility surface is derived from quoted volatilities that provides 
a way to interpolate an implied volatility at any strike and maturity. Unlike in other markets that quote volatility versus strike directly, 
the precious metal or FX smile is given implicitly as a set of restrictions implied by market instruments and as such a calibration procedure to construct 
a volatility- delta or volatility-strike smile is used.


[OSF precious metal volatility](https://osf.io/zdk3g/download)

[Zenodo precious metal volatility](https://zenodo.org/record/4407401/files/CmcPreciousMetalVol-15.pdf)

[FlipHtml5 precious metal volatility](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamIjN3ATOzMTPkl0av9mY)

[Github precious metal volatility](https://github.com/timxiao1203/preciousMetalVol)



### Credit Spread Curve

There is only one base interest rate per currency, corresponding to the bank’s unsecured lending/borrowing rate (such as LIBOR). The interest rate used to discount 
cashflows may include a credit spread above or below the base rate. Credit spread can be derived by either structural model or reduced-form (intensity) model. 
The structural approach regards default as an endogenous event by focusing on the capital structure of the firm. Whereas the reduced-form approach does not explain 
the event of default endogenously, but characterizes it exogenously by a jump process.

[OSF credit spread](https://osf.io/gfjkm/download)

[Zenodo credit spread](https://zenodo.org/record/4429184/files/CrCreditSpread-16.pdf)

[FlipHtml5 credit spread](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamAzNykTM0MTPkl0av9mY)

[Github credit spread](https://github.com/timxiao1203/creditSpreadCurve)

