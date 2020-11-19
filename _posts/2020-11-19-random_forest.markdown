---
layout: post
title:      "Random Forest"
date:       2020-11-19 19:09:38 +0000
permalink:  random_forest
---


**Random forests** are an ensemble learning method for classification and regression that operate by constructing a multitude of decision trees at training time and outputting the class that is the mode of the classes (classification) or mean/average prediction (regression) of the individual trees.

Random forest is a flexible, easy to use  algorithm that produces (even without hyper-parameter tuning) a great result most of the time. It is also one of the most used algorithms, because of its simplicity and diversity (it can be used for classification and regression tasks).

The random forest consists of many decisions trees. It uses bagging and feature randomness when building each individual tree trying to create uncorrelated forest of trees whose prediction by committee is more accurate than that of any individual tree. It fits a number of decision tree classifiers on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting. The sub-sample size is controlled with the parameter max_samples, if bootstrap=True (default), otherwise the whole dataset is used to build each tree.

Let's take a look at some of the commonly used parameters in Random Forest :

* **n_estimators** - defines the number of trees in the forest.  default value is 100.                                 
																 
* **max_depth** - It defines maximum depth of the tree. If None( which is the value by 'default' ), then nodes are expanded      until all leaves are pure or until all leaves contain less than min_samples_split samples.						

* **criterion** -It measures the quality of a split. the 2 criteria are “gini” for the Gini impurity and “entropy” for the information gain. The default value is gini.

* **bootstrap** - if bootstrap samples are used when building trees. If False, the whole dataset is used to build each tree. The default value is True.  



