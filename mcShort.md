
### Monte Carlo Multi-factor Short Rate Model

The Monte Carlo Multi-factor Short Rate Mode has been used extensively in pricing a variety of interest rate derivative securities. The model assumes that short rates at reset times are lognormally distributed.

Caplets were specified based on the following parameters :

·  short rate equal to three month LIBOR,
·  tenor equal to three months, one year and three years,
·  initial forward rate term structure set
·  constant at 7%, 7.5% and 8%, and
·  linearly upward rising , initially at 7% , with .0025 increments every three months,
·  strike equal to 7%, 8% and 9%,
·  LIBOR rate volatility set constant at 10%, 25% and 50%, and
·  adjacent LIBOR rate correlation constant in the range of 90% to 99% inclusive.


Caplets were benchmarked using Black’s model, that is, with constant volatility and with fixed discounting based on the initial term structure of forward rates; FP prices were based on 10,000 Monte Carlo paths. Numerical test results showed relative differences between the benchmark and FP model


·  not greater than 1% for high (50%) volatility,
·  not greater than .1% for low (10%) and medium (25%)volatility.




References:

[archive pdf](https://ia904708.us.archive.org/12/items/monte-carlo-short-rate/MonteCarloShortRate.pdf)

[gitbook](https://finwhite.gitbook.io/mcshortrate/)

[github carc volatility](https://github.com/cfrm17/carcVol)

[core arn pdf](https://core.ac.uk/download/534866797.pdf)

[core worst](https://core.ac.uk/works/127932808)

