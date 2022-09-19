
### Bond Bootstrapping Approach

We discuss a method for bootstrapping a set of zero rates from an input set of US government money market securities and bonds. The government bond bootstrapping procedure requires to input a set of financial instruments, of the type below, sorted by order of increasing time to maturity:

	Short term money market instruments (i.e., USD T-Bills with maturity not more than one year),
	Medium to long term “on the run” US government bonds,
	Medium to long term “off the run” US government bonds.

To determine discount factors at times intermediate to control points, we can apply a particular interpolation technique. There are three available:

	LINEAR
	LOG_LINEAR
	TIME_WEIGHTED_LINEAR

The LINEAR scheme interpolates zero rates linearly between successive control points on the zero curve; that is, if r(t_1) and r(t_2) are bootstrapped continuously compounded zero rates at successive control points

Government Bond Bootstrapping proceeds in two phases. The first phase uses short term instruments, which typically mature in one year or less. Consider, for example, a US government money market instrument 

We present a method for bootstrapping a set of zero rates from an input set of US government money market securities and bonds. We detail the calculations used to convert ACT/365 continuously compounded 
zero rates to the rates. We assume semi-annual compounding and, respectively, 30/360 and ACT/360 day-count fraction.

References:

[pdf](https://osf.io/4nhyb/download)

[wiki](https://osf.io/5sgx7/wiki/home/)





