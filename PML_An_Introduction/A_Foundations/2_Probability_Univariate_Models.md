# Probability: Univariate Models

## 2.1 Introduction

Some basic types of probability models.



## 2.2 Random Variables

**Probability mass function (pmf)**: Describe the probability of an event happening in a finite, discrete set of events.

**Cumulative distribution function (cdf)**: The probability of a variable less than a specific value. (non-decreasing)

**Probability density function (pdf)**: The derivative of the cdf.

**Quantile:** If the cdf is strictly monotonically increasing, it has an inverse, it has an inverse called quantile function. (given a cdf value, find the specific value satisfying the given cdf)

**Chain rule of probability**: Provides a way to create a high dimensional joint distribution from a set of conditional distributions.



### 2.3 Bayes' rule

**Definition:** The posterior probability is proportional to the product of prior probability and likelihood.

A good example: Page 77 The Monty Hall problem



## 2.4 Bernoulli and binomial distributions

**Logistic regression**: Regress the data distribution of a 1-D, 2-class dataset.



## 2.5 Categorical and multinomial distributions

**Softmax function**: Deal with multi-class classification problems.

**Log-sum-exp trick**: Avoid overflow when use indexed $e$



## 2.6 Univariate Gaussian (normal) distribution

**Why is gaussian distribution so widely used:**

1. Only two easily interpretable parameters.
2. The sums of independent random variables have an approximately Gaussian distribution, making it a good choice for modeling residual error and noise.
3. It has maximum entropy, so it contains the least number of assumptions.
4. A simple mathematical form.



## 2.7 Some other common univariate distributions*

**Student t-distribution**: The Gaussian distribution is quite sensitive to **outliers**. A **robust** alternative to the Gaussian is the Student t-distribution.

**Cauchy distribution**: Heavy tails compared to a Gaussian.

(Some other distributions left for future references...)



## 2.8 Transformations of random variables*

How to compute $p(y)$ given different input data format.



