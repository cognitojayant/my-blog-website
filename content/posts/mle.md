---
title: "Maximum Likelihood Estimate"
date: 2020-07-18T19:59:42+05:30
draft: true
katex: true
categories: ["Mathematics", "Statistics"]
tags: ["Machine Learning", "Mathematics"]
---
Consider a model parametrised by a vector  $\theta$, and let $X = (x_1,\cdots x_n)$ be observed data samples from the model. Then the function $p(X|\theta)$ is called the ***likelihood function*** if viewed as a function of the parameter vector $\theta$. It gives how probable the observed data $X$ is for different value of $\theta$.
Likelihood is not  a probability distribution over $\theta$ i.e. its integral with respect to $\theta$ may not always equal to one. 

For example, in case of Normal Distribution the set $X$ is independently drawn sample from normal distribution with unknown parameters $\theta = (\mu, \sigma^2)$ and therefore the likelihood function is given by following is treated as function of $\mu, \sigma$.

$$p(X|\theta) = \mathcal{N}(X|\mu, \sigma) = \prod_{i=1}^{N}\mathcal{N}(x_i|\mu,\sigma^2) = (\frac{1}{2\pi\sigma^2})^\frac{N}{2}\hspace{1mm}\exp(-\frac{1}{2\sigma}\sum_{i=1}^{N}(x_i - \mu)^2$$

The Maximum Likelihood Estimate (MLE) for parameter is the value of θ which maximises the likelihood. It is a very common way in statistics to estimate the unknown parameters for the model after observing the data.
