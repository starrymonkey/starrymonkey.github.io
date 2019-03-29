---
layout: post
title: "Occam's Razor in Machine Learning Approaches"
description: "brief post on simplicity in problem solving approaches"
comments: true
keywords: "Occam's Razor, Problem Solving, Simplicity"
---
Occam's Razor is a law of succinctness that in problem solving - "other things being equal, simpler explanations are generally better than the complex ones".

Applying the law to an Artificial Intelligence system, when facing multiple hypothesis, choose the simplest one consistent with the data (one with the fewest assumptions), given the simplest explanation is the most plausible till evidence is presented to prove it false.

The principle is certainly refutable, but the preference for simplicity is reasoned with that the solution, hypothesis or explanation to a problem is not singular; rather there exist number of possible and more complex alternatives, each has the potential to be falsified, and simpler ones are more testable, and lay closer to a basic statement.

In Machine Learning, many problems can be approached by a simple line function (degree-1 polynomial), generating prediction based on historical data (linear regression), binary or multivariate (using one-vs-all approach) classifications on input data that are linearly separable etc. When linear model cannot be adapted, the increase in degree of polynomial usually isn't drastic; one reason is to avoid model from overfitting to training set and not generalizing well to new data (low prediction accuracy). This underlines the tradeoff between complex hypothesis that fits the training set well and simpler hypothesis may generalize better and achieve higher computation efficiency.

When a problem gets too complex, a suggested approach is to break into smaller pieces, thus simplifying the task. For example, in the process of training AlphaStar to play real-time strategy game StarCraft II, the Deepmind team created multiple mini-games to train the Agent on specific tactics than try to tackle everything at once.

Another example would be adapting Feature Reduction, when fitting a Machine Learning model to a dataset that contains too many features, approaches such as Principle Component Analysis (PCA), or other statistical modelings are adapted to reduce the number of features as input. In multivariate datasets, there're usually a substantial number of correlated variables, increasing the complexity of analysis. PCA transforms a number of possibly correlated variables into a smaller set of uncorrelated variables (Principle Components), simplifies the analysis following.

The key idea behind all is to approach problems from first principles, try from the simplest approach and gradually build up. One good way to assess the simplicity of an approach would be to see the components involved in the solution, for example, when dealing with an image recognition task, it can be solved with a Convolutional Neural Network with multiple hidden layers, but it might also be possible with a single layered Neural Network adapting Logistic Regression. The latter is less involved and "easier" to train and tune, as it has less components, and for the ones used, they adapt simpler mathematical concepts.

Personally I also assess the simplicity of an approach based on when I acquired the knowledge to adapt such approach. For example, I learnt algebra, then calculus, then can use the math to implement logistic regression, then single hidden layer neural net, then more complex ones with varied activation functions etc.

One semi-counter example would be algorithm optimization, sometimes the brute force ones are the "simplest" (easy to implement, most apparent), but not optimized in time complexity. The most efficient approach might require a few tries, but none the less, they often don't involve crazy stacking of data structures or functions, but more of a condensation process reaching simplicity in the end.
