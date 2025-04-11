
### Commodity Simulation Translation


The goal of this work is to translate or convert simulated risk factors into market observables. There are three translations in commodity framework: price translation, volatility translation, and all-in translation.

Market instruments may be daily, for instance, but simulated risk factors may be monthly. Therefore, we need to convert monthly simulated risk factors into daily market instruments. Here we use linear interpolation within the range of risk factors and extrapolation beyond the range.

Since volatility is a surface, two-dimensional linear interpolation is required. We first do linear interpolation in quick delta (QD) direction converting 7QD to 11QD and then perform another linear interpolation in time direction. As seen in Figure 2, the cross-points of the grids are the risk factors  . The star dots denote the market instrument points whose volatility values are expected. The range of 7QDs is [1,99], which is the same as 11 QDs. This denotes no extrapolation but interpolation required in QD directions. However, extrapolation may be required in time direction.

In order to capture cross Gamma for pipelines that have spreads over bases, we need construct all-in scenarios. In our system, we simulate relative base and absolute spread.


References:

[archive bond abs](https://ia600703.us.archive.org/34/items/bond-abs-test/BondAbsTest.pdf)

[github double](https://github.com/cfrm17/doubleWindowBarrier)

[github swap](https://github.com/cfrm17/cmcFutureSwap)

[github swaption](https://github.com/cfrm17/cmcFutureSwaption)
