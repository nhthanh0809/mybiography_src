---
# title: SISE

# View.
#   1 = List
#   2 = Compact
#   3 = Card
view: 2

# Optional header image (relative to `static/img/` folder).
header:
  caption: ""
  image: ""


layout: post
title: "Hyperopt: A tool for parameter tuning"
date: 2020-06-01 12:38:00 -0700
comments: true
tags: technical
---

In deep learning, it is not easy to tune hyperparameters for optimal results. If we have 2 parameters (each with 3 prior desirable values), it is an easier problem. We will have possible combinations to try. However, with more parameters, the possible combinations will increase exponentially. For example, for 5 parameters, each with 4 desired values, we will have possible combinations. Manually trying each of them is not a very practical approach.

hence, the question usually is "Which way should I update my hyper-parameter to reduce the loss (i.e. gradients) in order to find the optimal model architecture?

Idealy, we should come up with an approach : 

* where we can search for hyperparameters (hyper-parameter search space) using a distributed compute on the cloud.
* intelligently optimize which of the possible combinations from the search space will give us the best results.
* Supports exisitng optimization techniques like Grid Search, Random Search, Bayesian Optmization etc.

Some of the exisiting tools for hyperparamter tuning are:
1. RayTune (https://ray.readthedocs.io/en/latest/tune.html)
2. Talos (https://autonomio.github.io/talos)
3. NNI (https://nni.readthedocs.io/en/latest/index.html)
4. Orion (https://orion.readthedocs.io/en/latest/user/pytorch.html#adapting-the-code-for-orion)
5. Sherpa (https://parameter-sherpa.readthedocs.io/en/latest/parallel/parallel-guide.html)
6. TPOT (https://github.com/EpistasisLab/tpot)
7. Hyperopt (https://github.com/hyperopt/hyperopt)
8. AWS Sagemaker Hyperparameter tuning (https://aws.amazon.com/sagemaker/?hp=tile&so-exp=below)
9. Botorch (https://botorch.org/)

Here, we will discuss hyperopt!

Hyperopt is an open-source hyperparameter tuning library written for Python. Hyperopt provides a general API for searching over hyperparameters and model types. Hyperopt offers two tuning algorithms: Random Search and the Bayesian method Tree of Parzen Estimators (TPE). To run hyperopt you define:
* the objective function
* the parameter space
* the number of experiments 

There are both continuous and categorical methods to describe the parameters.

<img src="/img/hyperopt.png " width="600" height="800" />

**Limitation**:
Hyper-parameter takes a lot of time to tune the parameters if number of trials and number of epocs (iteration of the neural network) are higher (which is desired). Hence, it would be good to explore how to parallelize the tuning work.


