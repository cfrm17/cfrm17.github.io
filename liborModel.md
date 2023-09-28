
### LIBOR Rate Model 

LIBOR Rate Model is used for pricing Libor-rate based derivative securities. The model is applied, primarily, to value instruments that settle at a Libor-rate reset point.  In order to value instruments that settle at points intermediate to Libor resets, we calculate the numeraire value at the settlement time by interpolating the numeraire at bracketing Libor reset points. 

Libor rate model is very useful to price callable exotics. Many derivatives have callable features. Callable exotics are among the most challenging derivatives to price. These products are loosely defined by the provision that gives the holder or issuer the right to call the product after a lock-out period (more details at https://finpricing.com/lib/EqCallable.html).

Although referred to as a BGM model, the model is actually based on Jamshidian’s approach towards Libor rate modeling (i.e., where Libor rates are modeled simultaneously under the spot Libor measure).

To generate a sample path of Libor rates, we discretize the SDEs above based on Euler’s method. Let each Libor accrual interval be discretized based on evenly spaced points. Then the crude Monte Carlo algorithm, for generating a single Libor rate sample path, has running time of O(n3m).

For example, if quarterly Libor rates must be generated over a period of ten years, and if each accrual period is partitioned using two points, then n=40 and m=1 ; in order to generate a single Libor rate path, we then require on the order of n3m = 64,000 operations! Over a typical number of Monte Carlo sample paths, say 5,000, we then require approximately 32 million operations.

We see that, while Jamshidian’s approach provides for direct simulation of Libor rates and the spot Libor numeraire process, its Monte Carlo implementation may be impractical depending on the accrual period discretization and number of Monte Carlo sample paths.

References:

[osf pdf](https://osf.io/wra62/download)


[zenodo multi carc](https://zenodo.org/record/7480124)

[zenodo multi carc pdf](https://zenodo.org/record/7480124/files/MultiCarc.pdf)

[zenodo carc lockin](https://zenodo.org/record/7487196)

[zenodo carc lockin pdf](https://zenodo.org/record/7487196/files/CARCLockIn.pdf)


