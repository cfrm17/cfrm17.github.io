
### Swap with Better-of Cliquet Option Model

A model is developed for pricing a swap with better of cliquet option. The floating amount payer makes semi-annual payments based on USD-LIBOR-BBA minus a spread. The fixed rate payer makes a single payment at swap maturity based on the arithmetic average of the S&P 500 Index price over certain pre-specified windows of ten consecutive trading days.

The swap’s fixed leg price is given by the value of a certain path-dependent European option. This option value is computed using Monte Carlo, by simulating the price of the S&P 500 Index at the point in each trading day window corresponding to the latest date. The price at each such point is then taken as the value of the S&P 500 Index average over the corresponding window of trading days.

The rate of return for each averaging day window is based on the relative change in the arithmetic average of the S&P 500 Index price over this window as compared against the average over the immediately preceding window, but bounded above and below by 13.5% and 0 respectively. The payoff at swap maturity is based on the notional USD amount multiplied by the better of 25.5% and the sum of the rate of return over each averaging day window.

FP represents the S&P 500 Index price based on a stochastic process, which follows geometric Brownian motion with piecewise constant drift and constant volatility, and a related stochastic process. Let the time t i correspond to the last day in the i th averaging window. 

we assume that the S&P 500 Index price, S , follows geometric Brownian motion with piecewise constant drift and volatility; furthermore the process S is driven by single Brownian motion. Here we simulate all points in the various averaging day windows

Entries under the Shift in Spot column represents a shift in the spot S&P 500 Index price relative to the base spot value , that is, new spot value = base spot value ´ (1+ shift) . Entries under the Shift in Volatility column are similarly defined, but with respect to a base volatility value. GA and FP option prices were both based on 100,000 Monte Carlo paths.


References:

[archive pdf](https://ia601605.us.archive.org/14/items/betterOfCliquet/betterOfCliquet.pdf)

[gitbook](https://finwhite.gitbook.io/swapbetterof/)

[github carc flexible](https://github.com/cfrm17/carcFlexibleReturn)

[core puttable pdf](https://core.ac.uk/download/534868202.pdf)

[core puttable](https://core.ac.uk/works/127930338)

