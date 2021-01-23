*WIP*

# Motivation

In the heterogenous-agent neoclassical growth model with stochastic income:
- the representative household solves its utility maximization problem subject to budget constraint (households solve the same problem ex-ante, but face different realizations of income which causes heterogeneity when simulating over many individuals)
- the representative firm solves its profit maximization problem
- the market clears

Due to this being a heterogenous  agent model, we can achieve a non-degenerate stationary wealth distribution in the long run (after simulating for many periods). 
We calibrate this model to have a mean asset to mean income ratio of about 3 to 4 to reflect [what we see in the real world](https://en.wikipedia.org/wiki/Affluence_in_the_United_States#:~:text=In%20the%20United%20States%2C%20as,household%20net%20worth%20is%20%24692%2C100.). 
See [calibrated model results here](https://github.com/tyrneh/Macro--hetereo_growth_model_stochastic_returns/blob/main/VFI_StochasticIncome-Calibrated.ipynb). This initial code is credited to [Professor Ben Moll](https://benjaminmoll.com/).

However, we see that this standard growth model fails to replicate the large amount of wealth concentration at the top of the wealth distribution in the United States, United Kingdom, and other developed countries. In particular it fails to match statistics like the top 1% wealth sahres. In the US for example, we find that the top 1% of wealth share holds 37% of total wealth, while our model predicts top 1% should hold 2.3% of total wealth. This standard model predicts that the savings function is decreasing in wealth, in both percentage and absolute terms. This is completely wrong compared to what we know from the real world - the wealthiest people save the most. 
<p align="center">
<img src="https://github.com/tyrneh/Macro--hetereo_growth_model_stochastic_returns/blob/main/Stochastic%20Income%20Savings%20Policy%20Function.JPG" width="300" height="200">

One possible extension of this heterogenous-agent growth model that researchers have proposed to explain top wealth inequality is to allow for stochastic rates of return ([Benhabib & al, 2014](https://www.researchgate.net/publication/301891020_Wealth_Distribution_and_Social_Mobility_in_the_US_A_Quantitative_Approach)). 
In [vfi_stochastic_income_and_returns](https://github.com/tyrneh/Macro--hetereo_growth_model_stochastic_returns/blob/main/vfi_stochastic_income_and_returns_Calibrated-B9707.ipynb), I attempt to extend this standard model to have stochastic returns. 

After calibrating this new stochastic returns model, we find that the savings is linear in wealth, which is the same result that research has shown *(citation needed)*. That is, for high-income type individuals, they will always save a positive portion of their wealth. This would be a cause for income inequality, as there will be those in the economy who always have realizations of high-income and will accumulate wealth forever. 
<p align="center">
<img src="https://github.com/tyrneh/Macro--hetereo_growth_model_stochastic_returns/blob/main/Stochastic%20Returns%20Savings%20Policy%20Function.JPG" width="300" height="200">

*To do:*
- *figure out why low-income savings rate does not become positive after some sufficient level of wealth*
- *figure out why asset distribution statistics imply lower 90th percentile wealth despite savings function implying higher inequality*


