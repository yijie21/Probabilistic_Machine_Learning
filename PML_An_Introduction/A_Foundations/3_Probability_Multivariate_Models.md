# Probability: Multivariate Models

## 3.1 Joint distributions for multiple random variables

**Covariance** measures the degrees to which two random variables are (linearly) related

**Correlation** is a normalized measure to describe the relation between two random variables.

**Uncorrelated does not imply independent.**

**Correlation does not imply causation.** Because two unrelated variables might have similar distributions.

**Simpson's paradox.** A statistical trend may disappear or reverse 



## 3.2 The multivariate Gaussian (normal) distribution

A lot of properties and derivations according to multivariate variables.

The **Mahalanobis distance** formulation for two vectors.



## 3.3 Linear Gaussian systems

**Bayes rule for Gaussians.** The Gaussian prior $p(z)$, combined with the Gaussian likelihood $p(y|z)$, results in a Gaussian posterior $p(z|y)$.



## 3.4 The exponential family

Only a complicated form, but when to use it?

(**Explained in further Chapter 12**).

Derivatives of the log partition function can be used to generate all the cumulants of the sufficient statistics.



## 3.5 Mixture models

**Mixture/Hierarchical models.** Weighted-average of different probability models.

Any smooth distribution can be approximated using a number of Gaussian distributions.

**Bernoulli mixture models.** Mix binary-valued random variable distributions.



## 3.6 Probabilistic graphical models

**PGM** is a joint distribution that uses a graph structure to encode conditional independence assumptions.

If the graph is a **directed acyclic graph (DAG)**, the model is called a **Bayesian network**.

Each node is a **random variable**, each edge is a **direct dependency**, each lack of edge is a **conditional independency**.
