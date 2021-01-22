# Motivation

In the heterogenous-agent neoclassical growth model with stochastic income:
- the representative household solves its utility maximization problem subject to budget constraint (households solve the same problem ex-ante, but face different realizations of income which causes heterogeneity when simulating over many individuals)
- the representative firm solves its profit maximization problem
- the market clears

Due to this being a heterogenous  agent model, we can achieve a non-degenerate stationary wealth distribution in the long run (after simulating for many periods). 
We calibrate this model to have a mean asset to mean income ratio of about 3 to 4 to reflect [real-world data](https://en.wikipedia.org/wiki/Affluence_in_the_United_States#:~:text=In%20the%20United%20States%2C%20as,household%20net%20worth%20is%20%24692%2C100.). 
See [calibrated model results here](https://github.com/tyrneh/sample_python_code/blob/main/WIP_neoclassical_growth_model/vfi_stochastic_income.ipynb). This initial code is credited to [Professor Ben Moll](https://benjaminmoll.com/).

However, we see that this standard growth model fails to replicate the large amount of wealth concentration at the top of the wealth distribution in the United States, United Kingdom, and other developed countries. In particular it fails to match statistics like the top 1% wealth sahres. In the US for example, we find that the top 1% of wealth share holds 37% of total wealth, while our model predicts top 1% should hold 2.3% of total wealth. 

One possible extension of this heterogenous-agent growth model that researchers have proposed to explain top wealth inequality is to allow for stochastic rates of return ([Benhabib & al, 2014](https://www.researchgate.net/publication/301891020_Wealth_Distribution_and_Social_Mobility_in_the_US_A_Quantitative_Approach)). 
In [vfi_stochastic_income_and_returns](https://github.com/tyrneh/sample_python_code/blob/main/WIP_neoclassical_growth_model/vfi_stochastic_income_and_returns.ipynb), I attempt to extend this standard model to have stochastic returns. 
