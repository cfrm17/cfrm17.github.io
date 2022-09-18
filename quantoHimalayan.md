
### Quanto Himalayan Option Valuation

Himalayan options are a form of European-style, path-dependent, exotic option on a basket of equity underliers, in which intermediate returns on selected equities enter the payoff, while the
equities are subsequently removed from the basket.

Like other exotic option, Quanto Himalayan may also have cap floor constraints and barrier conditions. The barrier option may knock out the trade before maturity.

In other words, k(i) is the index of the equity with the highest return, at the fixing
date ti, among those equities, whose returns at the previous fixing dates were not the
highest2. Given a strike level, K, the Himalayan option payoff is given.

This definition is consistent with the one in the case of domestic equities, that is, in the absence of a quanto adjustment. In the quanto case, the effect of the change in the quanto adjustment 
resulting from a change in the volatility is ignored. 

With the exception of the theta, the hedge ratios are computed using Malliavin weights.
The presence of the volatility calibration step requires an adjustment in the calculated
Malliavin hedge ratios, according to the chain rule.


Let the known dividend schedule for equity i consist of payments _i,1, . . . , _i,mi made at
times _i,1, . . . , _i,mi , all of which lie between the valuation date t and the last relevant
fixing tn. Furthermore, let the discount curve in the native currency of equity i be di,
that is, for any time s greater than the valuation time t, let the discount factor be
di(s − t).For times t _ s1, t _ s2, let us define di(s1, s2) = di(s2)/di(s1). 

We employ the definitions of the respective hedge ratios, as stated in the section on
the WM pricing method. With the exception of the theta, calculated through the
finite difference technique, all hedge ratios are computed using the Malliavin weight
approach. Additional considerations arise from the impact of the calibration procedure
on the sensitivity ratios, as describe in the next section.

Moreover, as can be seen from the test results below, the relative error in the gamma
hedge ratios can be quite large. These quantities are generally very small, making the
relative error a poor indicator of agreement. Moreover, it appears that the Monte Carlo
sampling error is quite large for the gamma hedge ratio. 

For a large number of paths, this ratio should be approximately normally distributed with mean zero and unit variance, if the means in the two models are equal. We believe that this is a more
meaningful way of comparing results whose Monte Carlo sampling error is large relative
to the size of their expectation.




References:

[pdf](https://osf.io/cg5x4/download)

[wiki](https://osf.io/ucqk6/wiki/home/)





