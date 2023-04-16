
### Mutual Fund Securitization Model

The purpose of the model is to determine, from a projected stream of future cashflows, whether all Commercial Paper used to fund the commissions to brokers for the sale of mutual funds will be repaid within a period. 
 Here a broker charges the Partnership a commission on the net asset value of the mutual funds sold.  The buyer of the mutual funds, however, pays nothing up front; instead, a deferred sales charge, which depends on 
 when the mutual funds are redeemed, is assessed.

The model assumes that the monthly net asset value of the mutual funds follows a deterministic process.  Administration and program fees, as well as mutual fund redemptions are then based on the monthly net asset value.  
Issued Commercial Paper is amortized into equal monthly payments over a period of six years.  Here the cashflows generated from the administration and redemption fees are paid monthly to the Partnership, to be used 
for the payment of outstanding Commercial Paper and accrued interest.  Furthermore, the model includes a test to determine whether a collateral infusion is required to aid in re-paying the Commercial Paper.

Based on the net value of all cashflows collected and paid by the Partnership, but without any discounting, the model yields a Boolean answer to the question of whether the Commercial Paper and accrued interest are repaid.

Commissions to brokers from the sale of mutual fund units are funded on a monthly basis.  Each new funded amount is amortized into 72 equal monthly payments over six years.  Monthly interest is based on the remaining 
funded amount at the beginning of the month, multiplied by the monthly cost of Commercial Paper, and is paid from money in the General Account.  If the interest owed exceeds the General Account balance, then the 
unpaid interest is added to the remaining funded amount at the end of the month (i.e., unpaid interest is capitalized).

After the monthly interest obligations have been met, any remaining money in the General account, plus money in the Retention Account, is used to pay the required amortized amount.  Furthermore, in the event of a 
Lock-up, all money in the Retention Account is used immediately to pay down the remaining funded amount.  The Retention Account, is a collateral account, which is funded by the mutual funds.

The Retention Account holds collateral towards the repayment of Commercial Paper principal.  The Retention Account balance, at the beginning of a month, accrues based on a monthly reinvestment rate.  The balance 
at the end of the month includes this accrued amount plus the balance in the General Account (which may be negative if amortized principal obligations could not be met).  The month’s ending Retention Account balance 
is, however, compared against an upper bound for required collateral; if the month’s ending Retention Account balance exceeds the upper bound, then the positive difference from the upper bound is returned.

he net asset value of the mutual funds follows a deterministic process, and that one party's capital contributions to fund sales commissions are amortized on a straight-line basis over a period of six years. 
The purpose of the model is to determine, from a projected stream of future principal and interest payments, whether all Commercial Paper will be repaid within a maximum period of thirteen years.


References:

[osf pdf](https://osf.io/vzfaw/download)

[zenodo epo pdf](https://zenodo.org/record/7526459/files/EpoModel.pdf)

[zenodo epo](https://zenodo.org/record/7526459)

[zenodo swap pdf](https://zenodo.org/record/7526526/files/equityForFloatSwap.pdf)

[zenodo swap](https://zenodo.org/record/7526526)

