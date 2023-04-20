
### Asian Commodity Swap

A commodity swap is a deal where counter-parties exchange fixed payments for floating payments monthly based on a specific commodity, for example, West Texas Intermediate (WTI) crude oil. The fixed payments are specified as a given quantity times a fixed price; the floating payments are specified as a given quantity times the spot value of the commodity on the payment date. The floating payments may also be based on the arithmetic average of spot commodity price (Asian commodity-price) over the payment period or LIBOR plus a spread.

The commodities swaps are based on crude and refined oil products and these swaps are typically Asian commodity-price swaps. A typical deal where one party pays fixed and receives floating is specified as follows:

The present value of the floating rate payment for the current payment period and paid at T is the sum of the risk-neutral expectation of the floating rate payment over the remainder of the current period plus the floating rate payment over the current period that has already passed. The required expectation is approximated similarly as to what is described above so that the present value of the floating payment for the current period is given 

V is given by equation (1) with WF and WB calculated using the unaccrued time in the current period but with NB as the sum of the accrued and unaccrued business days

It should be noted that futures contracts are not traded on the entire range of crude and refined oil products for which one party does commodity swaps. For example, one party has done commodity swaps based on fuel oils such as New York Harbor (NYH) 1% for which there are no futures contracts. In such cases, the price of floating payments for forward months are generated from swap prices obtained from various brokers. These prices may be given as a spread to value of floating payments for commodities on which futures contracts are written; for instance, this would be the case for TAPIS-Malaysian crude oil-which is given as spread to WTI.


References:

[archive pdf](https://ia601608.us.archive.org/22/items/asian-commodity/AsianCommodity.pdf)

[gitbook](https://finwhite.gitbook.io/asianswap/)

[github fair](https://github.com/cfrm17/fairValueAdjustment)

[core asian pdf](https://core.ac.uk/download/534868701.pdf)

[core asian](https://core.ac.uk/works/127933067)

