
### Exchangeable Convertible Bond Model

A convertible bond issuer pays periodic coupons to the convertible bond holder. The bond holder can convert the bond into the underlying stock within the period(s) of time specified by the conversion schedule. 
The bond issuer can call the bond and the holder can put it according to the call and put provisions. For pricing a regular convertible bond, you can find a reference at https://finpricing.com/lib/EqConvertible.html

The Exchangeable feature assumes that the convertible bond and the underlying stock are issued by different parties. There are two possible cases with respect to stock conversion:

Assume that the stock conversion is vulnerable. If the bond-issuer has defaulted by a time, t , then the stock price is zero. If, on the other hand, the bond-issuer has not defaulted by time t , then the stock 
price is given by St or 0.

We discretize the stock-price process based on a trinomial tree approach, and the respective default-time processes based on a two-state (i.e., default or no-default) tree. In order to discretize the processes 
above simultaneously, we then combine the respective trees into a three-factor tree.

Each node on the combined tree has 12 = 3´ 2´ 2 children; moreover, since the individual processes above are independent, the branching probability associated with each child is given by the product of the 
corresponding probabilities on each respective tree.


References:

[osf pdf](https://osf.io/zgx8c/download)

[zenodo ccds pdf](https://zenodo.org/record/7362947/files/ccds.pdf)

[zenodo ccds](https://zenodo.org/record/7362947)

[zenodo cdo mapping pdf](https://zenodo.org/record/7363084/files/CDOnMapping.pdf)

[zenodo cdo mapping](https://zenodo.org/record/7363084)
