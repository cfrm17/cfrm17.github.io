
### Credit Pricing Model Calibration 



A calibration procedures of the Default Correlation model is presented. There are two principal modifications.  The first is to change the manner in which asset correlations are converted into default correlations, the second is a small change in the algorithm by which the probability equations of the model are solved.  These changes are considered appropriate, and are necessary for the model to be considered robust enough to underpin the structuring and trading of complex credit contingent instruments.

The first modification involves the conversion of asset correlations into default correlations. Conversion of asset correlations into default correlations in the original model is carried out by equating the joint default probability of the bivariate normal copula between two names at a specific time horizon

The modified conversion procedure simply re-converts the (constant) asset correlation into a default correlation each time there is a change in the value of one of the credit curves.  This assures that the default correlations are always within the allowed range.  It also has the benefit of ensuring that the asset correlation is held constant over time.

This simple procedure has the effect of normalizing the solution, allowing the solution to recover.  This modification is accompanied by an error-checking condition.  If the solution obtained by the ostrich algorithm does not match the inputs to within a specified tolerance, a failure is reported.

The testing process was carried out in two stages.  First, the independent implementation of the model which was constructed for the testing of the original model outlined in was modified. 

The second phase of the process was carried out using the previous version of the model independently modified to conform to the new specifications by the author to make further tests.  These tests were conducted with both the new implementation of the model and the previous version of the model.

In order to further investigate the differences between the modified model and the original model, we have constructed our own modified version of the model.  This version is equipped with an error reporting facility, which reports the error between the inputs and the recomputation of those inputs from the solution to the probability equations.   The error is computed as the Frobenius norm of the differences in the inputs and the inputs as reconstructed from the solution as given by equation (6) with the ostrich algorithm.


References:

[zenodo pdf](https://zenodo.org/record/7378454/files/CreditModCorr.pdf)

[archive cppi](https://ia803406.us.archive.org/32/items/eq-cppi-19/EqCppi-archive.pdf)

[gitbook coupon](https://finwhite.gitbook.io/mortgagetranfercoupon/)

[github mbs](https://github.com/timxiao1203/MBS-Model)

[github mvf](https://github.com/timxiao1203/MVF-Swap)
