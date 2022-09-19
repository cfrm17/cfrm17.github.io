
### Three Factor Convertible Bond Model

The owner of a convertible bond (CB) receives periodic coupon payments from the issuer, but can also convert the CB into the issuer’s stock.  The convertible bond may also include call and put provisions, 
which respectively allow the issuer to buy back the convertible bond and the owner to put the convertible bond for respective preset amounts.  

We present a three factor trinomial tree based model for pricing the CB, where the three factors are the short interest rate corresponding to the bond’s coupon currency, the issuer’s stock price, and
the exchange rate from the issuer’s stock currency into the bond’s coupon currency.

Here the short interest rate process is assumed to be of Ho-Lee form under the bond’s coupon currency risk-neutral probability measure, and the stock price and foreign exchange rate processes are assumed 
to follow geometric Brownian motion with drift under their respective risk-neutral probability measures.  

The stock price process is then expressed under the bond’s coupon currency risk neutral probability measure by means of a quanto adjustment.   Under the bond’s coupon currency risk neutral probability 
measure, then, the short interest rate, stock price and foreign exchange rate processes respectively follow geometric Brownian motion with drift, but are driven by pair-wise correlated Brownian motions.  

We next define three related random variables, which are each taken to be particular linear combinations of the original short interest rate, stock price and foreign exchange rate random variables.  
Here the respective linear combinations are chosen such that the processes for the new random variables are now driven by pairwise uncorrelated Brownian motions.

We next construct respective trinomial trees to approximate the processes for each new random variable, but with each tree based on the same time slice partition of the CB tenor.  A new tree, 
which combines these respective trees, is then defined such that the set of nodes on a particular time slice of the combined tree equals the cross product of the set of nodes in each of the three respective 
trees at this time slice.  

Each node on the combined tree then has   children; and, since the processes for the new random variables are driven by pairwise independent Brownian motions, the probability of branching to 
any of these children nodes is given by the product of the corresponding probabilities on each of the individual trees.  The values for the original short interest rate, stock price and foreign 
exchange rate are now obtained, at each node on the combined tree, by inverting a related linear system of equations.

At each tree time slice we keep track of the call strike, put strike and stock conversion level at this time; we note, however, that FP does not include accrued interest in the respective call 
nd put strike levels at tree times where a coupon is not paid.  FP assumes that the CB owner can choose to hold, put or convert the bond into stock.  The CB issuer can then choose to call the bond.  
If the bond is called, however, the owner can then force the bond to be converted into stock.  

We use a three factor, trinomial tree based model for pricing the CB. Here FP constructs three independent trinomial trees, which are then combined into a three-factor tree. Upon review of this method 
we note that :

First, since the spreadsheet implementation limits the maximum number of trinomial tree time steps to be less than 47, it may not be possible to choose the time step sufficiently small such that branching 
probabilities on each respective trinomial tree are positive and less than one. The respective trinomial trees, and the combined multi-factor tree, may then not be stable in all cases.

Second, each respective trinomial tree is constructed by coalescing a related binomial tree. While this operation matches the mean of the random variable on a trinomial tree time slice, its variance is 
only approximately matched.



References:

[pdf](https://osf.io/pbjf8/download)

[wiki](https://osf.io/wvhpq/wiki/home/)





