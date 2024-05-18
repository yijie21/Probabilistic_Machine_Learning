# Introduction

## 1.1 What is machine learning

**Definition:** A computer program for task **T**, that learns and improves from experience **E**. And the metric for performance evaluation is **P**.

**Key:** Explain all ML methods from a **probabilistic perspective**.

**Two core concepts:**

1. Treat all quantities as **random variables**.
2. Describe them as **probability distributions**.

**Reasons for probabilistic descriptions:**

1. It is the optimal method to make decision under uncertainty.
2. It is commonly-used by other science areas.



## 1.2 Supervised Learning

**Definition:** Learn from given ground truth.

**Two main branches:**

Classification:

- Tricks before tackling an ML problem:
  - Exploratory data analysis. This means preprocess the raw data to find some **obvious data patterns** to simplify the problem.
  - Dimensionality reduction. Reduce the higher-dimensional data to 2d or 3d for better visialuzation.
- How to learn a classifier:
  - Construct different rules to separate data of different classes.
- How to measure the performance of the classification model:
  - Empirical risk minimization. Set **asymmetric/empirical** loss values for different wrong classification results, and weighted-sum them all as the total loss. Then we explore the optimal model parameters to minimize the total loss.
- How to deal with uncertainty in an ML problem:
  - Definitions of uncertainty:
    - Epistemic/Model Uncertainty: Inability to predict the exact output from the input due to lack of knowledge.
    - Aleatoric/Data Uncertainty: Intrinsic/irreducible/unavoidable stochasticity in the input-output mapping.
  - Capture uncertainty with **conditional probability distribution**.
  - **Softmax function:** Avoid the restriction that the sum of predicted probability values for all classes must be added up to 1.
    - Specific operation: refer to Page 37 for the exact formula.
- What is the loss function for fitting the probabilistic model:
  - Negative log likelihood: refer to Page 38 for the exact formula.


Regression:

(Difference from classification: Predict a real-valued quantity instead of discrete class labels.)

- The loss used:
  - Quadratic loss: Evaluate the difference between the predicted values and the ground truth values.
  - Mean squared error: Weighted average of quadratic loss for all predicted values.
- Classifications of regression models:
  - Linear regression: Estimate the weights and bias of a affine transform function
  - Polynomial regression: The same form of linear regression but with different index for $x$ (manually specify the transformation of the input features)
  - Deep neural networks: Use neural networks for nonlinear feature extraction

**Two phenomenons of models:**

Overfitting: Trained to only fit well to the training dataset.

Generalization: Trained to also work well for the unseen dataset.



## 1.3 Unsupervised Learning

**Definition:**  Learn without ground truth.
