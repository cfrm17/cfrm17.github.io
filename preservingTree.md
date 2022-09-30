
### Martingale Preserving Tree 

An important feature of the popular three factor trinomial tree is that it uses a deterministic approximation of the interest rates for constructing the stock tree. The preservation of the martingale property of the stock price is thus not guaranteed.  and may potentially represent a problem.

We propose a two-factor tree model that implements the Hull-White and Black-Karasinski models. The new tree model does preserve the martingale property of the stock for sufficiently long terms (with accuracy better that 10-8 for terms of at least 10 years). 

The three factor model assumes that under the risk neutral probability measure the stock price follows the stochastic process


The coupon is the nominal annual rate of interest that is paid to the holder on a regular basis. It is usually expressed as a percentage of the face value (coupon rate: https://finpricing.com/lib/FiBondCoupon.html). The coupon rate is either fixed or variable. The coupon rate is given as an annualized percentage of the face value.

The probabilities of the joint Brownian motion on the combined tree are adjusted according to the correlation between W rt and W St. This approach produces an efficient implementation, since it uses only two one-dimensional trees. It has a significant drawback, however: the martingale property of the stock price is not preserved. 

The equation depends on two factors, and the equity tree is built as a genuine two-dimensional tree.  Its r-projection replicates the above interest rate tree, with the same values of r and transition probabilities at the corresponding nodes in the r-dimension. The distribution of the stock values is calculated and the overall transition probabilities are adjusted so as to preserve the martingale property and, if possible, to match the variance. The new trees allow variable time steps.

Given the limitations of the three-factor model that stem from the deterministic approximation of the interest rates, it performs remarkably well. Even for a bond’s term as long as 7 years the difference between the model and benchmark is within acceptable limits. The differences grow rapidly for longer terms, and the model is not recommended for terms exceeding 7 years.

As a more general observation, one should mind the limitations of the short term rates models such as the Hull-White model or the Black-Karasinski model. It is well known that in the Hull-White model the interest rate may become negative, which breaks the no-arbitrage condition.

On the Hull-White tree, the negative rates occur for sufficiently long terms, or even for medium terms when a fine time discretization is used. The problem is mitigated by the fact that the rates become negative in the lower part of the tree, whose contribution is small due to the low probability of reaching that part of tree. However, the experience shows that the Hull-White model is not very good for terms exceeding 10 years.

Another kind of problem arises when one uses a log-normal models of the short rates, such as the Black-Karasinski model, in conjunction with log-normal stock models. The stock price grows exponentially with the rate which, in turn, is an exponential function of the random factor.

As a result, there is a non-zero probability that the stock price turns infinite within a finite time. One may argue that when those large stock prices are discounted back with the appropriate rates they should give reasonable contribution to the present value.

References:

[pdf](https://osf.io/6eyrv/download)

[list](https://osf.io/u95g2/wiki/home/)





