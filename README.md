# Deep Cox Mixtures

This repository contains code for the NeurIPS 2020, ML4H paper: 
[Deep Cox Mixtures for Survival Regression](https://arxiv.org/abs/2101.06536)

### Usage
```
from dcm import deep_cox_mixtures
results = deep_cox_mixture.experiment(dataset='SUPPORT', prot_att='race', groups=('white', 'other'))
deep_cox_mixtures.display_results(results)
```
### Requirements
`dcm` depends on `tensorflow2` and `scikit-survival`, 

Running baseline models for comparison requires `lifelines`, `pycox` and `dsm`
