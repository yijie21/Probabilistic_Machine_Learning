# Statistics

## 4.1 Introduction

Discuss how to estimating model parameters $\theta$ from data $D$.

Discuss how to model uncertainty or confidence in the estimate.



## 4.2 Maximum likelihood estimation (MLE)

**iid assumption**: Assume training examples are independent sampled from the same distribution and identically distributed.

Usually use **log likelihood** to compute the loss.

A standard way to measure the dissimilarity between probability distributions is the **KL divergence**.



## 4.3 Empirical risk minimization (ERM)

An empirical loss function by replacing the log loss term with any other loss function.



## 4.4 Other estimation methods

**Method of Moments (MOM)**: Use some discrete and limited number of minimization instead of minimizing the whole-range theoretical $E$.

**Online (recursive) estimation**: Perform online minimization or get the optimal parameters by leveraging the result from the last few time steps.



## 4.5 Regularization

The main solution to overfitting is to use **regularization**, which involves a regularization parameter and a complexity penalty.

The complexity penalty is usually a prior, for example, the probability distribution.

**MAP estimation**: Maximum a posterior estimation.

**How to pick the regularization parameter**: Pick one that minimizes the validation risk between the training set and the validation set.

**Cross validation**: Split the dataset in $k$ groups, train on $k-1$ groups and validate on the left group.

**One-standard error rule**: Measure the uncertainty of an estimate.



## 4.6 Bayesian statistics

**Inference**: Modeling uncertainty about parameters using a probability distribution.

(Many specialized concepts and formulas for practical problems.)

**Bayesian machine learning**: Computing the posterior using the bayesian principles.

Computational issues: Use some approximation methods to compute the posterior inference. (Grid approximation, Quadratic approximation, Variational approximation, Markov Chain Monte Carlo approximation)



## 4.7 Frequentist statistics

An alternative approach which avoids treating parameters like random variables, thus avoiding the use of priors and Bayes rule.

Here, uncertainty is not represented by the posterior distribution, but **by sampling distribution of an estimator**.

The key idea in frequentist statistics is to view the data $D$ as a random variable, and the parameters from which the data are drawn, as a fixed but unknown constant.

A most common estimator is the MLE.

**Confidence intervals**: We use the variability induced by the sampling distribution as a way to estimate uncertainty of a parameter estimate.

