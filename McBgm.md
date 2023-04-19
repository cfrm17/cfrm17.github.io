
### Monte Carlo Simulation for LMM

Brace-Gatarek-Musiela (BGM) model, also called LIBOR Market Model (LMM), is a multi-factor log-normal model for pricing interest rate derivatives. The model is usually solved by Monte Carlo simulation.

The model is aimed to calibrate its parameters on the market price of a list of at-the-money FX options, with increasing maturities 

Diffusion dates are set in such a way that all calibration dates are diffusion dates. Then the diffusion step is specified on each slice. Diffusion dates are business days, approximately spaced by the diffusion step (except the last step that can be shorter). 

Generally speaking, all diffusions will be considered between diffusion dates, whereas discounting will be performed between spot dates.

It is important to notice that these dates should be absolutely the same in both currencies. In particular, the spot dates are computed in the same way as those of an FX option.

When computed at a diffusion date other than  , these rates and discount factors are random variables that are materialized as Monte-Carlo arrays. Each index corresponds to a path and expectations will be replaced by averages over all paths.

At each diffusion date, only a certain number of discount factors are provided. For the purpose of rate diffusion, one may need other discount factors. An interpolation procedure is thus necessary. Currently, we have implemented a linear interpolation of the logarithm of encompassing available maturities. Assume for instance that these maturities are in the following order:

This interpolation, which is very commonly used, means that forward spot rates are piecewise constant. It is similar to, but not quite the same as making a linear interpolation of the yields to maturity. It has been chosen because accuracy is the same and formulas are simpler.


References:

[archive pdf](https://ia904702.us.archive.org/7/items/monte-carlo-bgm/MonteCarloBgm.pdf)

[gitbook inverse](https://finwhite.gitbook.io/callableInverse/)

[github bb](https://github.com/timxiao1203/BrownianBridge)

[core cva pdf](https://core.ac.uk/download/232916600.pdf)

[core cva](https://core.ac.uk/works/8871669)

