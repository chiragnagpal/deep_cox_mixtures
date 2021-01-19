# Deep Cox Mixtures
#### _Chirag Nagpal<sup>1,2</sup> Steve Yadlowsky<sup>1</sup>, Negar Rostamzadeh<sup>1</sup> and Katherine Heller<sup>1</sup>_

#### _<sup>1</sup>Google Brain Team_, _<sup>2</sup>Carnegie Mellon University_

This repository contains code for the NeurIPS 2020, ML4H paper: 
[Deep Cox Mixtures for Survival Regression](https://arxiv.org/abs/2101.06536)

### Poster

![ML4H 2020 Poster](http://www.cs.cmu.edu/~chiragn/papers/Deep_Cox_mixtures_poster.png)


### Usage
```
from dcm import deep_cox_mixtures
results = deep_cox_mixture.experiment(dataset='SUPPORT', prot_att='race', groups=('white', 'other'))
deep_cox_mixtures.display_results(results)
```
### Requirements
`dcm` depends on `tensorflow2` and `scikit-survival`, 

Running baseline models for comparison requires `lifelines`, `pycox` and `dsm`
