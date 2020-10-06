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
