
### Shout Cap and Floor

A European shout cap is an option giving the holder the right to “shout” a European call strike level at spot at any time during the option tenor. That is, the holder receives an at-the-money European call when they shout. If they do not shout at any time during the option tenor the holder receives a European call struck at the initial strike level. Typically the initial strike level is set to the spot level when the contract is initiated. This instrument provides a protective cap on losses in short positions without requiring additional payments.

A European shout floor is similar to a shout cap. The shout floor is an option giving the holder the right to “shout” a European put strike level at spot at any time during the option tenor. That is, the holder receives an at-the-money European put when they shout. If they do not shout at any time during the option tenor the holder receives a European put struck at the initial strike level. This instrument provides a protective floor on losses in long positions without requiring additional payments 

It should be noted that shout caps and floors may be referred to as shout calls and puts although shout calls and puts originally referred to differently structured shout options

The price of European shout caps and floors are given by choosing a shouting strategies that maximize the present value of the expectation of their respective payoffs at expiry. The optimal shouting strategy amounts to specifying a stopping time which is knowing whether to shout or not at a given time in a given state of the world that takes values in the interval [0,T] since the option tenor is T . 

The prices are determined numerically using tree based methods. The option tenor is discretized and for each time in the discretization a discrete set of states for the underlying asset is constructed [2]. Given the tree of state prices, the shout cap and floor prices are obtained by backward inducting through the tree from expiration comparing the value of shouting to the shout option value and taking the maximum value.


References:

[archive pdf](https://ia904703.us.archive.org/12/items/shout-cap/ShoutCap.pdf)

[gitbook bermudan](https://finwhite.gitbook.io/singlebermudan/)

[github swap](https://github.com/cfrm17/equityForFloatSwap)

[core frtb pdf](https://core.ac.uk/download/534863938.pdf)

[core frtb](https://core.ac.uk/works/127932027)

