# Decision Theory

## 5.1 Bayesian decision theory

**Bayesian decision theory**: Decide the best action according to the computed posterior.

**F-scores**: An evaluation metric combining precision and recall values.

**Probabilistic prediction problems**: Pick a probability distribution over some value of interest instead of an exact action.

**KL divergence**: A common form of loss functions for comparing two distributions.

**Proper scoring rules**: A loss function measuring the similarity of two distributions. And such loss function can be a cross-entropy loss or Brier score.



## 5.2 Choosing the "right" model

**Hypothesis testing**: Use a **Bayes factor** to evaluate the likelihood of two hypothesis.

**Model selection**: Compute the **marginal likelihood**, or evidence of each model $m$

**Occam's razor**: If two models have equally high marginal likelihood, we should prefer the model which is simpler and has fewer parameters.

**Information criteria**: Since marginal likelihood is difficult to compute, we use some other related metrics for model selection. (The bayesian information criterion, Akaike information criterion, Minimum description length)



## 5.3 Frequentist decision theory

**Definition**: Treat the unknown state of nature as a fixed but unknown quantity, and treat the data $x$ as random. Thus instead of conditioning on $x$, we average over it, to compute the loss we expect to incur if we apply our decision procedure to many different datasets.

**The risk of an estimator**: Bayes risk/Maximum risk

**Consistent estimators**: A procedure that recovers the true parameters. An example of this is the maximum likelihood estimator.

**Admissible estimators**: An estimator is said to be admissible if it is not strictly dominated by any other estimator.



## 5.4 Empirical risk minimization

Focus on **how to apply frequentist decision theory in the context of supervised learning**.

**Approximation error**: Measuring how closely the hypothesis space can model the true optimal function.

**Estimation error**: Measuring the difference in estimated risks due to having a finite training set.

**Regularized empirical risk**: To avoid the chance of overfitting, we need to add a complexity penalty.

**Cross-validation**: A simple way of estimating the population risk for a supervised learning setup. 

**Statistical learning theory**: Since cross-validation is slow, this is needed.



## 5.5 Frequentist hypothesis testing

Focus on ways to determining id a hypothesis model is plausible or not.

To be more specific, suppose we have two hypothesis, known as the null hypothesis $H_0$ and an alternative hypothesis $H_1$, and we want to choose one we think is more likely.

