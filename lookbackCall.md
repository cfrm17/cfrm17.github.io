
### Lookback Call Option 

A model is presented for pricing a European lookback call option on a stock index with guaranteed exchange rate (LBCGER).  We define a lookback window  .  In addition a sampling frequency (e.g., daily, weekly, etc.) over the lookback window is specified.

Let delta  denote the value at time t for the underlying security.  The strike of the LBCGER, K ,  is set equal to the minimum price of the underlying security over a set of discrete points

The payoff at maturity is the value of a standard European call with strike   adjusted by the guaranteed exchange rate  

The method for pricing a lookback call option with guaranteed exchange rate is based on a single factor Monte Carlo approach.  The idea of the method is to  stochastically generate a large number of discrete sample paths for the underlying security.  

Risk neutral pricing formulas are presented for various types of cross-currency instruments, in particular, European call options with payoffs at maturity of the form




References:

[archive pdf](https://ia904703.us.archive.org/11/items/lookbackCall/lookbackCall.pdf)

[gitbook](https://finwhite.gitbook.io/lookbackcall/)

[core bond pdf](https://core.ac.uk/download/534868166.pdf)

[core bond](https://core.ac.uk/works/127930344)

