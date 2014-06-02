Day 1
=====

Weka and scikit

buncha quotes and cv stuff

explanation of different terminology of data mining

face detection algorithms

ML learning definition. 

explanation of training sets

a method to learn from data, train, predict.

You don't need to know how classifier works, magic lightbox that does. 
What you really need to know is evaluation (unit testing?)

evaluating classifiers for, e.g. spam detection. Bayesian?

eval should be suspect if it passes majority at the beginning, but it is not *exactly* like unit testing because we don't intentionally want to write failing tests ad the beginning.

unit testing is bad-ish because it is binary. either it passes or it doesn't pass. Machine learning is fuzzier.

How much data do you use for training versus how much do you use for testing?

more training data resulst in better models but more data increases confidence in generalization capability.

K-fold cros-validation

* shuffle
* partition data into k folds, each fold same # of instances
* one fold for testing adn k-1 folds for training. prediction for 1 fold.
* repeat k times resulting in predictions for k folds
* calculate the classification metrics you need base on ground truth and predictions
* bias-variance tradoeff: k large, loewr bias, higher variance.
* one initial shuffle
* when number of folds = number of instances k-fold cross-validation is called leave-one-out eval.
