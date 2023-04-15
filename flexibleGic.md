
### Flexible GIC Valuation

A flexible GIC is an investment with an embedded option to redeem the principal and accrued interest at any time after 30 days from the date of purchase. In other words, the holder of GIC has an option to redeem the principal and accrued interest at any time after 30 days of from the date of purchase. No interest is paid if the investment is redeemed within first 30 days from the purchase date.

We price the option of a flexible GIC with a one factor Hull-White model via a trinomial tree. The Hull-White model assumes a normal distribution for the rates. Our solution constructs a Hull-White tree. The calibration procedures take an interest rate curve as input (ignoring volatility surfaces) and assume volatility and mean reversion parameters as constants. 

We also apply the bootstrapping algorithm to produce the zero-coupon bond yields from the quoted bond yields. The linear interpolation is further used to obtain the zero-coupon yield term structure. Bond yield can be computed as https://finpricing.com/lib/FiZeroBond.html

The width of the tree increases as a square root of time rather than linearly as in the Hull-White algorithm. The tree wings that are away from the mean by more than  t1/2 are cut off. The resulting error is of the order of 10-8, which is much less than the error resulting from discretization of the random walk component of the interest rate. This modification gives a noticeable acceleration of the calculations at a large number of time slices (the calculation time scales then as n2.5 rather than n3 of the Hull-White tree, where n stands for the number of the tree time slices).

The initial approximation of the short rate in the middle node of a time slice is taken as a forward rate for the time interval between the given and next slices, without using the Hull-White analytical approximation, The initial value is subsequently improved by the Newton-Raphson formula.

To facilitate the theta calculations, the time slice immediately following the root is separated from the root by a much smaller time interval than the intervals between the other time slices (typically it was taken as 10-4 of a regular time interval). The transition probabilities from the nodes of this, irregular time slice is calculated by the perturbation method.

In the case of exercise a penalty is applied: the accrued interest is recalculated according to a lower rate than that set for the deal till maturity. The interest adjustments are typically different for the two exercise periods: the adjusted interest rate for the first exercise period is lower than that for the second one.

There are two types of the Premium GIC, GIC and RSP. They differ by the way the first and second coupons are treated. In the GIC type, the coupons are handed over to the holder and cannot be reinvested into the same deal. In the RSP type, the coupons are automatically reinvested into the same deal and cannot be redeemed before the maturity unless the option is exercised.


References:

[osf pdf](https://osf.io/q6ut7/download)

[Zenodo CDS Curve pdf](https://zenodo.org/record/7373680/files/creditCurveAdjustment.pdf)

[Zenodo CDS Curve](https://zenodo.org/record/7373680)

[Zenodo default sensitivity pdf](https://zenodo.org/record/7373904/files/DefaultSensitivity.pdf)

[Zenodo default sensitivity](https://zenodo.org/record/7373904)

