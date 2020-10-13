## Market Data

### Yield Curve Introduction
Yield curves can be derived from government bonds or LIBOR/swap instruments. The LIBOR/swap term structure offers several advantages over government 
curves, and is a robust tool for pricing and hedging financial products.  Correlations among governments and other fixed-income products have declined, 
making the swap term structure a more efficient hedging and pricing vehicle.

[More details](/IrCurveIntroduction-1.pdf)

[FlipHtml5 yield curve](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamUTNyITM2ITPkl0av9mY)

[Github yield curve](https://github.com/cfrm17/YieldCurve/raw/main/IrCurveIntroduction-1.pdf)

[Pubpub yield curve](https://david.pubpub.org/pub/c7n9gnqy/download/pdf)

[Zenodo yield curve](https://zenodo.org/record/3928440/files/IrCurveIntroduction-1.pdf)


### Yield Curve Construction
Yield curves are derived or bootstrapped from observed market instruments that represent the most liquid and dominant interest rate products for 
certain time horizons. 	The objective of the bootstrap algorithm is to find the zero rate or discount factor for each maturity point and cash 
flow date sequentially so that all curve instruments can be priced back to the market quotes.

[More details](/IrCurve-2.pdf)

[FlipHtml5 yield curve construction](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamkDO1kzM2ITPkl0av9mY)

[Github yield curve construction](https://github.com/cfrm17/YieldCurveConstruction/raw/main/IrCurve-2.pdf)

[Pubpub yield curve construction](https://david.pubpub.org/pub/pmwcp6ah/download/pdf)

[Zenodo yield curve construction](https://zenodo.org/record/3928459/files/IrCurve-2.pdf)


### Basis Curve
The basis curve construction methodology is based on the most liquid market instruments. Normally a basis curve is divided into two parts. The short 
end of the term structure is determined using LIBOR rates and the remaining is derived using basis swaps.

[More details](/IrBasisCurve-3.pdf)

[FlipHtml5 basis curve](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamgTM2kzM2ITPkl0av9mY)

[Github basis curve](https://github.com/cfrm17/BasisCurve/raw/main/IrBasisCurve-3.pdf)

[Pubpub basis curve](https://david.pubpub.org/pub/j9ol7gvf/download/pdf)

[Zenodo basis curve](https://zenodo.org/record/3928459/files/IrCurve-2.pdf)


### OIS Curve
Many banks now consider that overnight indexed swap (OIS) rates should be used for discounting when collateralized portfolios are valued and that 
LIBOR should be used for discounting when portfolios are not collateralized.

[More details](/IrOIS-4.pdf)

[FlipHtml5 ois](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamETN0MDN2ITPkl0av9mY)

[Github ois](https://github.com/cfrm17/OisCurve/raw/main/IrOIS-4.pdf)

[Pubpub ois](https://david.pubpub.org/pub/x9tb74np/download/pdf)

[Zenodo ois](https://zenodo.org/record/3928515/files/IrOIS-4.pdf)


### FX Implied Volatility
Unlike in other markets that quote volatility versus strike directly, the FX smile is given implicitly as a set of restrictions implied by market 
instruments and as such a calibration procedure to construct a volatility- delta or volatility-strike smile is used.

[More details](/FxVol-5.pdf)

[FlipHtml5 fx vol](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamIjMyYDN2ITPkl0av9mY)

[Github fx vol](https://github.com/cfrm17/fxVol/raw/main/FxVol-5.pdf)

[Pubpub fx vol](https://david.pubpub.org/pub/q1ujtvfx/download/pdf)

[Zenodo fx vol](https://zenodo.org/record/3928657/files/FxVol-5.pdf)


### Swaption Implied Volatility
The term structures of implied volatilities which provide indications of the market’s near- and long-term uncertainty about future short- and 
long-term swap rates. A crucial property of the implied volatility surface is the absence of arbitrage.

[More details](/IrSwnVol-6.pdf)

[FlipHtml5 swaption vol](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamYTNyYDN2ITPkl0av9mY)

[Github swaption vol](https://github.com/cfrm17/swaptionVol/raw/main/IrSwnVol-6.pdf)

[Pubpub swaption vol](https://david.pubpub.org/pub/r83v30ev/download/pdf)

[Zenodo swaption vol](https://zenodo.org/record/3928662/files/IrSwnVol-6.pdf)


### Cap Implied Volatility
An implied volatility is the volatility implied by the market price of an option based on the Black-Scholes option pricing model. In cap market, 
a cap/floor is quoted by implied volatilities but not prices. An interest rate cap volatility surface is a three-dimensional plot of the implied 
volatility of a cap as a function of strike and maturity. 

[More details](/IrCapVol-7.pdf)

[FlipHtml5 cap vol](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamMzN0ITN2ITPkl0av9mY)

[Github cap vol](https://github.com/cfrm17/capVol/raw/main/IrCapVol-7.pdf)

[Pubpub cap vol](https://david.pubpub.org/pub/d1mdbxkw/download/pdf)

[Zenodo cap vol](https://zenodo.org/record/3928669/files/IrCapVol-7.pdf)


### FX Forward Points
Market standard is to use FX quoted forward spreads and USD zero rate curve to generate FX implied forward curve. In other words, FX curve 
construction generates an interest rate curve of the quoting currency from the interest rate curve of the base currency. The construction methodology 
is based on the arbitrage-free relationship between forward FX rates and the discount rates of the two currencies.

[More details](/FxForwardCurve-8.pdf)

[FlipHtml5 fx forward](https://fliphtml5.com/download/download-pdf-file.php?str=x0DZh9GTud3bENXamQDO0ITN2ITPkl0av9mY)

[Github fx forward](https://github.com/cfrm17/fxForwardPoints/raw/main/FxForwardCurve-8.pdf)

[Pubpub fx forward](https://david.pubpub.org/pub/6utrh10z/download/pdf)

[Zenodo fx forward](https://zenodo.org/record/3928681/files/FxForwardCurve-8.pdf)
