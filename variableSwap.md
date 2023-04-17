
### Variable Rate Swap Valuation

Variable rate swap is a special type of interest rate swap in which one leg of the swap corresponds to fixed rate payments while the other involves fixed rate payments for an initial period of time and a floating rate for the rest. The floating rate on that portion is defined as a minimum of two index rates.

The fixed rate leg is similar to a fixed rate bond. The bond price is computed by discounting each coupon descripted at https://finpricing.com/lib/FiBond.html

We treat the two index rates as assets whose values are lognormally distributed random variable. Their pricing procedure uses discount factors retrieved from the EURIBOR curve.

One example of variable rate swap is shown belows:

• Payment period: March 1, 2010 through March 1, 2026

• Payment frequency annual

• Notional DEM 49,500,000

• R&V payments rate: 8.875 %

• Payments rate: min(EURCMS10, GBPCMS10)

The tests were focused on the following set of parameters:

• Diffusion, T = 30 years,

• CMS rate 1, r1 = 5%

• CMS rate 2, r2 = 6%

• volatility 1, 1 =10%

• volatility 2, 2 =10%

• correlation,  = 95%

References:

[osf pdf](https://osf.io/np5bw/download)

[zenodo bond option pdf](https://zenodo.org/record/7681904/files/BondOption.pdf)

[zenodo bond option](https://zenodo.org/record/7681904)

[zenodo bond futures option pdf](https://zenodo.org/record/7682025/files/BondFuturesOption.pdf)

[zenodo bond futures option](https://zenodo.org/record/7682025)

