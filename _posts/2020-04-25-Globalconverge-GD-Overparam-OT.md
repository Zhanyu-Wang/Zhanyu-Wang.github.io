---
layout: post
title:  "Review of 'On the Global Convergence of Gradient Descent for Over-parameterized Models using Optimal Transport'"
date:   2020-04-26 01:15:01
categories: post
---
# Title

1. Global Convergence (Property: e.g. generalization)
2. Gradient Descent (Method: e.g. SGD)
3. Over-parameterized (Model: e.g. NTK)
4. Optimal Transport (Tools: e.g. ?)

# Abstract

1. Problem
    1. sparse spikes deconvolution
    2. neural network with a single hidden layer
2. Setting
    1. discretized into a mixture of particles
    2. continuous-time gradient descent on weights and positions
    3. (Reason behind idea) idealization of the usual way to train neural networks
4. Results
    1. gradient flow converge to global minimizers (non-convex)
        1. initialized correctly
        2. many-particle limit (asymptotic)
5. Tools
    1. Wasserstein gradient flows
6. Experiments
    1. reasonable number of particles are good 
    2. even in high dimension

# Introduction
1. classical task in machine learning
    1. loss function R is smooth and convex
    2. find element being a linear combination of features $\phi(\theta)$
    3. => signed measure $\mu$ on $\theta$
    4. $G(\mu)$ is an convex regularizer, e.g. TV norm for sparsity
    5. in this paper consider $\phi(\theta)$ differentiable and $\theta\in\Theta\subset\ \mathbb{R}^d$
    6. e.g. NN with a single hidden layer, sparse spikes deconvolution, Low-rank tensor decomposition
2. related work
    1. conditional gradient  {% sidenote 1 'Martin Jaggi. Revisiting Frank-Wolfe: Projection-free sparse convex optimization. In Proceedings ofthe International Conference on Machine Learning (ICML), 2013.' %}






# Questions

1. Do we have generalization error results by all this analysis? (Title 1)
2. Do we have SGD results? (Title 2, Abs 2.3)
3. Can we analysis more than one hidden layer? (Title 3)
4. Why is optimal transport necessary? (Title 4, Abs 5.1)

5. Any other problem fitting in this? (Abs 1)
6. Can we reduce the case to be weights in 0/1? (Abs 2.2)
7. Is global minimizers unique? (Abs 4.1)
8. How should we initialize? (Abs 4.1.1)
9. Do we have non-aymptotic result? (Abs 4.1.2, Abs 6.1)
10. How large dimension can it handle? (Abs 6.2)













