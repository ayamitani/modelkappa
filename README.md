# ModelKappa
Calculate model-based kappa of agreement and association and their standard errors as seen in:
- Mitani, A. A., & Nelson, K. P. (2017). Modeling Agreement between Binary Classifications of Multiple Raters in R and SAS. Journal of Modern Applied Statistical Methods, 16(2), 277-309. doi: [10.22237/jmasm/1509495300](https://digitalcommons.wayne.edu/jmasm/vol16/iss2/15/)
- Mitani, A. A., Freer, P. E. & Nelson, K. P. (2017) Summary measures of agreement and association between many raters' ordinal classifications. Annals of Epidemiology, 27(10), 677-685. doi: [10.1016/j.annepidem.2017.09.001](http://www.sciencedirect.com/science/article/pii/S1047279717303447)
- Nelson, K. P., and Edwards, D. (2015) Measures of agreement between many raters for ordinal classifications. Statistics in Medicine, 34: 3116–3132. doi: [10.1002/sim.6546](https://onlinelibrary.wiley.com/doi/abs/10.1002/sim.6546) 
- Nelson, K. P. and Edwards, D. (2008), On population‐based measures of agreement for binary classifications. Canadian Journal of Statistics, 36: 411-426. doi: [10.1002/cjs.5550360306](https://onlinelibrary.wiley.com/action/showCitFormats?doi=10.1002%2Fcjs.5550360306)

### R installation Instructions
Copy and paste the following code to install modelkappa package in R.
```
install.packages("devtools")
library(devtools)
devtools::install_github("AyaMitani/ModelKappa")
library(ModelKappa)
```
### Use ModelKappa function to calculate model-based agreement (and association) for multiple raters each assessing multiple cases
```
?ModelKappa 
data(holmdata)
ModelKappa(data=holmdata, cat=Cat, item=Item, rater=Rater)
```
