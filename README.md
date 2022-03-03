# Deep Cox Mixtures
#### _Chirag Nagpal<sup>1,2</sup> Steve Yadlowsky<sup>1</sup>, Negar Rostamzadeh<sup>1</sup> and Katherine Heller<sup>1</sup>_

#### _<sup>1</sup>Google Brain Team_, _<sup>2</sup>Carnegie Mellon University_


---
> **❗⚠️❗⚠️❗⚠️❗⚠️❗ IMPORTANT NOTE ❗⚠️❗⚠️❗⚠️❗⚠️❗⚠️❗**
>
> ***Deep Cox Mixtures*** **now has a more stable `pytorch` implementation here**:
>
## https://autonlab.github.io/auton-survival/models/dcm/
>
> **`tensorflow` version is no longer supported.** ***Please use the version above.*** 

---


<img width=100% align="center" src=https://ndownloader.figshare.com/files/28316535>

This repository contains code for the MLHC 2021 paper: 

[Deep Cox Mixtures for Survival Regression](https://arxiv.org/abs/2101.06536)


### Installation

To download and run Deep Cox Mixtures:

```console
foo@bar:~$ git clone https://github.com/chiragnagpal/deep_cox_mixtures.git
foo@bar:~$ cd deep_cox_mixtures
foo@bar:~$ pip install -r requirements.txt
```


### Usage

To run DCM on a standard survival analysis dataset like SUPPORT, please see the following
example notebook:

1. [Deep Cox Mixtures on the SUPPORT Dataset](https://nbviewer.jupyter.org/github/chiragnagpal/deep_cox_mixtures/blob/master/DCM%20on%20SUPPORT%20Dataset.ipynb)


To run the original experiments from the paper, please use: 
```python
from dcm import deep_cox_mixture
results = deep_cox_mixture.experiment(dataset='SUPPORT', prot_att='race', groups=('white', 'other'))
deep_cox_mixture.display_results(results)
```
### Requirements
`dcm` depends on `tensorflow2` and `scikit-survival`, 

Running baseline models for comparison requires `lifelines`, `pycox` and `dsm`


### Citing

Please cite using the following bib-entry:

```python
@article{nagpal2021dcm,
  title={Deep Cox mixtures for survival regression},
  author={Nagpal, Chirag and Yadlowsky, Steve and Rostamzadeh, Negar and Heller, Katherine},
  journal={Machine Learning for Healthcare Conference},
  year={2021}
  organization={PMLR}
}
```
