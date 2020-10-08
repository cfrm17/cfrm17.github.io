## Market Data

### Yield Curve Introduction
Yield curves can be derived from government bonds or LIBOR/swap instruments. The LIBOR/swap term structure offers several advantages over government 
curves, and is a robust tool for pricing and hedging financial products.  Correlations among governments and other fixed-income products have declined, 
making the swap term structure a more efficient hedging and pricing vehicle.

[More details](/IrCurveIntroduction-1.pdf)


### Yield Curve Construction
Yield curves are derived or bootstrapped from observed market instruments that represent the most liquid and dominant interest rate products for 
certain time horizons. 	The objective of the bootstrap algorithm is to find the zero rate or discount factor for each maturity point and cash 
flow date sequentially so that all curve instruments can be priced back to the market quotes.

[More details](/IrCurve-2.pdf)


### Basis Curve
The basis curve construction methodology is based on the most liquid market instruments. Normally a basis curve is divided into two parts. The short 
end of the term structure is determined using LIBOR rates and the remaining is derived using basis swaps.

[More details](/IrBasisCurve-3.pdf)


### OIS Curve
Many banks now consider that overnight indexed swap (OIS) rates should be used for discounting when collateralized portfolios are valued and that 
LIBOR should be used for discounting when portfolios are not collateralized.

[More details](/IrOIS-4.pdf)

### FX Implied Volatility
Unlike in other markets that quote volatility versus strike directly, the FX smile is given implicitly as a set of restrictions implied by market 
instruments and as such a calibration procedure to construct a volatility- delta or volatility-strike smile is used.

[More details](/FxVol-5.pdf)

### Swaption Implied Volatility
The term structures of implied volatilities which provide indications of the market’s near- and long-term uncertainty about future short- and 
long-term swap rates. A crucial property of the implied volatility surface is the absence of arbitrage.

[More details](/IrSwnVol-6.pdf)

### Cap Implied Volatility
An implied volatility is the volatility implied by the market price of an option based on the Black-Scholes option pricing model. In cap market, 
a cap/floor is quoted by implied volatilities but not prices. An interest rate cap volatility surface is a three-dimensional plot of the implied 
volatility of a cap as a function of strike and maturity. 

[More details](/IrCapVol-7.pdf)

### FX Forward Points
Market standard is to use FX quoted forward spreads and USD zero rate curve to generate FX implied forward curve. In other words, FX curve 
construction generates an interest rate curve of the quoting currency from the interest rate curve of the base currency. The construction methodology 
is based on the arbitrage-free relationship between forward FX rates and the discount rates of the two currencies.

[More details](/FxForwardCurve-8.pdf)
