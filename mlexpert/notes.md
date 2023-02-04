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

### Naive Bayes

- model - an appromixation of a relationship between an input and an output
- heuristic - an approach to finding a solution which is typically faster but less accurate than some optimal solution
- bernoulli distribution - a distribution which evaluates particular outcome as binary
    - example - a word was either in a message or not in a message (binary representation)
- prior - indicates the probability of a particular class regardless of the features of some examples
- likelihood - probability of some features given a particular class
- evidence - denominator of the naive bayes classifier
- posterior - probability of a class given some features
- vocabulary - list of words that naive bayes recognizes
- laplace smoothing - type of additive smoothing which mitigages the chance of encountering zero probabilities within the naive bayes classifier
- tokenization - splitting of some raw textual input into individual words or elements
- featurization - process of transforming raw inputs into something a model can perform training and predictions on
- vectorizer - used in a step of featurizing, transforms some input into something else
    - example - binary vectorizer which transforms tokenized messages into a binary vector indicating which items in the vocabulary appear in the message
- stop works - a word, typically discarded, which doesn't add much predictive value
- stemming - removing the ending modifiers of words, leaving the stem of the word
- lemmatization - a more calculated form of stemming which ensures the proper lemma results from removing the word modifiers

### Performance

- decision point - cut-off point in which anything below the cutoff is determined to be a certain class and anything above the cutoff is the other class
- accuracy - number of true positives plus the number of true negatives divided by the total number of examples
- unbalanced classes - when one class is far more frequently observed than another class
- model training - determining the model parameter values
- confusion matrix - in the binary case, a 2x2 matrix indicating the number of true positives, true negatives, and false negatives
- sensitivity - also recall, the proportion of true positives which are correctly classified
- specificity - proportion of true negatives which are correctly classified
- precision - number of true positives divided by the true positives plus the false positives
- f1 score - harmonic mean of the precision and recall
- validation - technique of holding out some portion of examples to be tested separately from the set of examples used to train the model
- generalize - ability of a model to perform well on the test set as well as examples beyond the test set
- receiver operator characteristic curve - ROC curve, is a plot of how the specificity and sensivity change as the decision threshold changes
    - area under the ROC curve is the probability that a randomly chosen positive example will have a higher prediction probability of being positive than a randomly chosen negative example
- hyperparameter - any parameter associated with a model which is not learned
