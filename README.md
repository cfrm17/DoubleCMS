# Double CMS

A double CMS derivatives represents a European type derivatives whose matured payoff depends on two CMS rates.1 For most important products in the fixed income market, the payoff function can be an affine-linear with respect to two CMS rates and may be possibly capped and/or floored. Another typical derivative is accumulator.

There are three basic types of payoffs: (a) an affine-linear on two CMS rates, (b) a call on a linear combination of the two and (c) a put on the combination. For the first type payoff (a), the present value can be calculated by using single CMS cap/floor model. 

Further, if the weighting-coefficients in the affine linear function, which are also called index gearing factors, have same signs, then it is also called (double-) CMS average; otherwise, it is called (double-) CMS spread. 

Conventionally, for the second and third types of payoffs, they may be called CMS average/spread call and put, respectively. One may also notice that a vanilla digital call (put) can be well approximated by two calls (puts). Hence a CMS average/spread digital call/put can be replicated by CMS average/spread calls/puts. In this vetting report, we only consider double-CMS derivatives with payoffs of type (b) and (c).

Special examples are CMS spread calls (or cap or caplets), puts (or floor or floorlets) and swaps. A double-CMS (structured) swap is a swap contract with a regular funding leg and a structured (or CMS) leg in which coupons are functions of two CMS rates as mentioned above. Particularly, each (structured) coupon rate can be a sum of an affine-linear function with respect to two CMS rates and a linear combination of CMS average/spread calls and puts. 

With this structure, we have the following special cases: (a) simple CMS average/spread swaps in which coupon rates in the CMS leg are not capped nor floored, (b) CMS average/spread cap-floor swaps and (c) CMS average/spread digital swaps. The double-CMS swaps, which are considered in this vetting report, are not callable.

Let us consider non-callable double-CMS rate swap called “CMS Spread or Average Swap and Option”. The swap is composed of a so-called double-index leg, or more specific “CMS leg”, and a vanilla funding leg. Clearly, evaluating the vanilla funding leg is trivial and we will not cover that here. Corresponding to each accrual period of the CMS leg, the coupon rate is a function of the two CMS rates, also denoted as S1 an S2. This coupon rate, denoted as C, can be further decomposed into a linear part and two vanilla option parts.

The value of a (non-callable) swap is the sum of values of two swap legs. In all our swap products, one of swap legs is always a vanilla funding leg. The calculation of the value of the funding leg is trivial. Hence we only need to consider the pricing of the other one, the structured leg, or the CMS average/spread leg. Since the swap is non-callable, the present value of a CMS average/spread leg is the sum of values of all structured coupons. 

Under an appropriate forward measure, the value of each structured coupon is equal to the discounted expectation of the coupon. For some trivial cases when the coupon rate is just a linear combination of two CMS rates, then the expectation can be calculated by using single CMS rate European vanilla option pricing model. Therefore, it suffices to consider the calculation of the expectation of CMS average/spread call-payoff

The expectation of CMS average/spread call-payoff is calculated. In the function, two market implied (i.e., SABRNmodel implied) marginal PDFs and CDFs are calculated. For a given European vanilla option tenor and a current expectation of a underlying index rate, SABRN European option pricing model is completely determined by four SABRN-model parameters. 

For a given swaption market, all SABRN-model parameters are calibrated to the market. Hence, for a given option tenor, a pair of CMS rates and the current expectations of the two CMS rates together with the two sets of corresponding SABRN-model parameters, then the market implied PDFs/CDFs of the two CMS rates are also completely determined.


References:

https://finpricing.com/lib/FxAccumulator.html

https://derivatives.hcommons.org/fixed-income-derivatives/
