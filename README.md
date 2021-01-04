# Deep Cox Mixtures

Code for the paper: Deep Cox Mixtures for Survival Regression

### Usage
```
from dcm import deep_cox_mixtures
results = deep_cox_mixture.experiment(dataset='SUPPORT', prot_att='race', groups=('white', 'other'))
deep_cox_mixtures.display_results(results)
```
### Requirements
`dcm` depends on `te` `scikit-survival`, 

Running baseline models for comparison requires `lifelines`, `pycox` and `dsm`
