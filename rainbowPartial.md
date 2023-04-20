
### Rainbow Partial Barrier Option

A rainbow partial barrier option is an option on two assets where one asset-the trigger asset-knocks in an European call or put on a second asset; such an option is therefore European. (Unless specified otherwise, all options are European style.) The adjective partial refers to the fact that the knock in or out period is shorter than the option tenor. 

The adjective rainbow describes the fact that the option is on two assets and cannot be priced as equivalent option on a single asset. Rainbow partial barrier options come in eight “colors”: the trigger asset initially may be above or below the barrier knocking in or out a call or put on the other asset.

We implemented analytic model for pricing rainbow partial barrier options where a trigger asset knocks in or out an European call or put on a different asset.

The current value of the option is obtained using the martingale representation for options. For example, the current value of a rainbow up-and-out partial barrier put option is given by taking the risk neutral expectation of XUOP using the money market account as numeraire:

The other option flavors are obtained by exchanging put payoffs for call payoffs and vice versa; the other barrier flavors are obtained from various parity relations. A plain vanilla put (call) can be replicated as long position in a rainbow partial barrier up-and-out put (call) and up-and-in put (call)


References:

[archive pdf](https://ia601606.us.archive.org/11/items/rainbow-partial/RainbowPartial.pdf)

[gitbook floor](https://finwhite.gitbook.io/amortizingfloor/)

[github epo](https://github.com/cfrm17/epoModel)

[core bond pdf](https://core.ac.uk/download/534868154.pdf)

[core bond](https://core.ac.uk/works/127933282)

