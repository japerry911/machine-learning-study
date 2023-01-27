# Notes

### Introduction

- ranking - optimizing machine learning models to rank candidates, such as music, articles, or products
    - typically the goal is to order the candidates such that the candidates which are most likely to be interacted with (purchased, viewed, liked, etc...) are above other candidates that aren't likely to be interacted with
- supervised learning - optimizing machine learning models based on previously observed features and labels
    - typically the goal is to attach the most likely label to some provided features
    - requires data labels labels
- unsupervised learning - an approach within machine learning that takes in unlabeled examples and produces patterns from the provided data
    - typically the goal is to discover something previously unknown about the unlabeled examples
    - no labels
- deep learning - optimizing neural networks, often with many hidden layers, to perform supervised or unsupervised learning
- recommendation systems - systems with the goal of presenting an item to a user such that the user will most likely purchase, view, or like the recommended item
    - items can take many forms, such as music, movies, or products
    - also called recommender systems

### Prerequisites

- features - a set of quantities or properties describing an observation
    - can be binary like 'day' and 'night'; categorical like 'morning', 'afternoon', and 'evening'; continuous like '3.141'; or ordinal like 'threatened', 'endangered', 'extinct', where the categories can be ordered
- labels - usually paired with a set of features for use in supervised learning
    - can be discrete or continous
- examples - pairs of features and labels
- dimensions - here, the number of features associated with a particular example
- vector - here, a feature vector, which is a list of features representing a particular example
- matrix - an array of values, usually consisting of multiple rows and columns
- matrix transpose - an operator that flips a matrix over its diagonal
- polynomial - a feature with more than one variable/coefficient pair
- derivative - indicates how much the output of a function will change with respect to a change in its input
- probability - how likely something is to occur
    - this can be independent, such as the roll of the dice, or conditional, such as drawing two cards subsequently out of a deck with replacement
- probability distribution - a function that takes in an outcome and outputs the probaility of that particular outcome occuring
- gaussian distribution - very common type of probability distribution which fits many real world observations; also called a normal distribution
- uniform distribution - probability distribution in which each outcome is equally likely; for example, rolling a normal six-sided die
