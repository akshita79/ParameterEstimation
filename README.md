# Parameter Estimation using Maximum Likelihood Estimation (MLE)

## Introduction:

Maximum Likelihood Estimation (MLE) is a method used for estimating the parameters of a statistical model. It is a widely used technique in statistics and machine learning for parameter estimation. The basic idea behind MLE is to find the parameter values that maximize the likelihood function, which measures how well the model explains the observed data.

## Theory:

### Likelihood Function:

Given a statistical model with parameters \( \theta \) and observed data \( x_1, x_2, ..., x_n \), the likelihood function \( L(\theta | x_1, x_2, ..., x_n) \) measures the likelihood of observing the given data under the given model and parameter values. It is often expressed as the probability density function (pdf) or probability mass function (pmf) evaluated at the observed data points, considered as a function of the parameters.

### Log-Likelihood Function:

To simplify calculations and maximize numerical stability, the logarithm of the likelihood function, called the log-likelihood function \( \ell(\theta | x_1, x_2, ..., x_n) \), is often used instead. Maximizing the log-likelihood function is equivalent to maximizing the likelihood function, as the logarithm is a monotonically increasing function.

### Maximum Likelihood Estimation (MLE):

The goal of MLE is to find the parameter values \( \hat{\theta} \) that maximize the likelihood (or equivalently, the log-likelihood) function:

\[ \hat{\theta} = \arg \max_{\theta} L(\theta | x_1, x_2, ..., x_n) \]

or

\[ \hat{\theta} = \arg \max_{\theta} \ell(\theta | x_1, x_2, ..., x_n) \]

In other words, MLE seeks the parameter values that make the observed data most probable under the assumed statistical model.

### Properties of MLE:

1. **Consistency**: As the sample size \( n \) approaches infinity, the MLE converges in probability to the true parameter value.
2. **Asymptotic Normality**: Under certain regularity conditions, the MLE follows an approximately normal distribution with mean equal to the true parameter value and variance equal to the inverse of the Fisher information.
3. **Efficiency**: Among all unbiased estimators, the MLE achieves the minimum variance asymptotically, making it asymptotically efficient.
4. **Invariance**: MLE is invariant under reparameterization. That is, if \( \hat{\theta} \) is the MLE of \( \theta \), then \( g(\hat{\theta}) \) is the MLE of \( g(\theta) \) for any function \( g \).

### Computational Considerations:

In practice, maximizing the likelihood function (or log-likelihood function) may involve solving optimization problems, often using numerical optimization algorithms such as gradient descent, Newton's method, or the EM algorithm.

## Conclusion:

Maximum Likelihood Estimation (MLE) is a powerful method for estimating the parameters of statistical models. By maximizing the likelihood function, MLE provides parameter estimates that are theoretically sound and possess desirable statistical properties. It is widely used across various fields, including statistics, machine learning, econometrics, and biology, among others.
