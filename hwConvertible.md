
### Pricing Convertible Bond via Hull White Model

A convertible bond pays the holder periodic coupon payments from the issuer, but can also convert it into the issuer’s stock.  The model uses a two-factor trinomial tree for pricing the convertible bond, 
where the two factors are the short term interest rate and the issuer’s stock price.

Here we assume that the short term interest rate process follows a stochastic differential equation (SDE) of the Hull-White form, and that the stock’s price follows geometric Brownian motion with drift.  
For tractability, however, the stock’s price SDE is modified so that its drift does not depend on the stochastic short-term interest rate.

Based on the Hull-White single-factor tree building approach, respective trinomial trees are constructed for the short-term interest rate and stock’s price processes.  Using the Hull-White two-factor tree 
building procedure, a combined tree is constructed by matching the mean, variance and correlation corresponding to each combined tree node.  The convertible bond price is given from the combined tree by 
backward induction.  

Here the issue time refers to the coupon payment immediately prior to, or including, the valuation time; otherwise it corresponds to the bond’s issuance.  Since the valuation time is taken to be zero, 
the issue time must be less than or equal to zero.

The Brownian motions respectively driving the short-term interest rate and stock’s price processes have constant instantaneous correlation coefficient.  A drawback, here, is that the SDE above for the 
stock’s price admits only a  zero dividend yield.

We build respective trinomial trees for the approximate stock’s price and short-term interest rate processes above.  This construction is based on Hull and White’s single factor tree-building technique, 
but is generalized to accommodate non-uniformly spaced partitions of the interval to bond maturity.  The separate trinomial trees are then combined into a joint tree using Hull and White’s two-factor 
tree building procedure.  

Here the set of nodes at a particular time slice on the combined tree is given by the cross product of the nodes on each respective tree at this time slice.  From each node on the combined tree emanate 
nine children; the branching probabilities are given by the product of the corresponding probabilities on the respective trees, but shifted by a certain amount so to match the correlation between the 
random variables associated with the combined tree node.

The Hull-White convertible bond pricing model assumes that the short-term interest rate process follows a SDE of the Hull-White form, and that the stock’s price process follows geometric Brownian motion 
with drift. The derivation of the stock’s price process assumes that the initial term structure of risk-free rates is sufficiently smooth, while in practice it is generally only piecewise smooth.
The two-factor tree building procedure appears from testing to be numerically stable and convergent, provided that the correlation between the short-term interest rate is sufficiently small

References:

[osf pdf](https://osf.io/eyb8c/download)

[zenodo xccy option](https://zenodo.org/record/7474447)

[zenodo xccy option pdf](https://zenodo.org/record/7474447/files/CrossCcyOption.pdf)

[zenodo xccy option](https://zenodo.org/record/7478480)

[zenodo average option pdf](https://zenodo.org/record/7478480/files/AverageRateOption.pdf)



