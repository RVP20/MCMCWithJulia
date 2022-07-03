# Markov Chain Monte Carlo With Julia

## Overview
This project mainly focuses on Markov Chain Monte Carlo techniques. Markov Chain Monte Carlo sampling provides a class of algorithms for systematic random sampling from high-dimensional probability distributions. MCMC techniques often solve integration and optimization problems in large dimensional spaces. These two types of problems play a fundamental role in machine learning. Just going over the theory is boring. This project involved a substantial computational aspect, and we were asked to implement various algorithms, preferably in Julia. 

The list of topics that were covered is as follows:
1. Sampling Methods and general Monte Carlo methods
2. Rejection Sampling and Importance Sampling
3. Markov Chain and Measure Theory basics
4. Metropolis-Hastings Algorithm
5. Accelerating MCMC Algorithms
6. MCMC Algorithms for Intractable Posteriors

## Assignment 1:
1. Implement a Discrete Inverse Transform sampler for Poisson distribution.
2. Implement a Discrete Accept Reject Sampler to simulate draws from Binomial(n, p) using a Poisson proposal.

## Assignment 2
1. Prove that Barker's algorithm generates a Bern(cy\*py/cx\*px + cy\*py) event. 
Also, find the probability distribution of the number of iterations it takes to give an output.
2. Sample uniformly from a p-dimensional sphere (a circle is p=2). Consider a p-vector x = (x1, x2, ... , xp) and let  .  denote the Euclidean norm. The pdf of this distribution is given.
Use a uniform p-dimensional hypercube to sample uniformly from this sphere. Implement this for p = 2, 3, 4, 5, and 6. 
What happens as p increases?
3. Using accept-reject and a standard normal proposal, obtain samples from a truncated standard normal distribution. Run for a=4 and a=1. 
What are the differences between the two settings?

## Assignment 3

1. Suppose X1, X2, , Xn (iid draws) and Y1, Y2, , Yn is a Markov chain with F as the stationary distribution. Consider two estimates of the mean, calculated as the average of Xis and Yis.
Which estimator is better? In other words, which estimator has smaller variance? Support your answer with formal mathematical arguments.
2. Suppose Y1, Y2, ..., Yn|𝜇 ~ N(𝜇, 1). Assume the prior on 𝜇 ~ t, where  is the degrees of freedom. Assume the prior on  ~ Truncated Gamma(a0, b0,(2,∞)), where (2,∞) is the support of Truncated Gamma.
What is the joint posterior distribution of (𝜇, )?
Write an MH algorithm to sample from the above posterior distribution.
Generate n=100 data points. Set a0=2, b0=0.1, and run the MH algorithm described above. 
3. Consider the Bayesian linear regression model. The likelihood is 
y1, y2, , yn|𝛽, 𝜎2 ~ Nn(X𝛽, 𝜎2In)
The parameters of interest are 𝛽, 𝜎2 , just like regular MLE. We assume priors:
𝛽 ~ Np(𝜇, 𝜎2Ip)  and  𝜎2~ Inverse Gamma(a, b).
Np is the p-dimensional multivariate normal distribution.
Here a, b and 𝜇 are hyper-parameters, which need to be chosen according to the dataset.
What is the posterior distribution of  (𝛽, 𝜎2)?
Implement an MH algorithm to sample from the posterior distribution for any suitable dataset (for example, Boston-housing dataset, etc.)

## Assignment 4
Research Paper: https://www.tandfonline.com/doi/full/10.1080/01621459.2020.1847120 
Summarize sections 2 and 3 in your own words (with all mathematical details and rigor). Do NOT copy. Write in your own words.

## Assignment 5
Research Paper: https://arxiv.org/abs/2004.07471

1.Summarize sections 2, 3 and 4 in your own words (with all mathematical details and rigor). Do NOT copy. Write in your own words.
2.Implement the example 5.1, play with the parameter 𝛽 and create different plots to judge the quality of your samples








