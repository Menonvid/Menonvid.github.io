---
layout: post
title:      "Gradient Boost and XG Boost"
date:       2020-11-25 21:04:25 +0000
permalink:  gradient_boost_and_xg_boost
---


**Gradient boost** is a machine learning technique for regression and classification problems, which produces a prediction model in the form of an ensemble of weak prediction models, typically decision trees. It builds the model in a stage-wise fashion like other boosting methods do, and it generalizes them by allowing optimization of an arbitrary differentiable loss function.

It builds an additive model in a forward stage-wise fashion i.e it allows for the optimization of arbitrary differentiable loss functions. In each stage a regression tree is fit on the negative gradient of the given loss function.

Gradient boost is one of the most powerful concepts in machine learning. The term gradient boost refers to a class of algorithms, rather than a single one. The version with the highest performance is **XGBoost**, which is short term for **Extreme Gradient Boosting.**

Let's take a look at some of the parameters for Gradient Boost :

* **n_estimators** : It is the number of boosting stages to perform. GB is fairly robust to over-fitting so a large number usually results in better performance. The default value is 100

*  **learning_rate** : shrinks the contribution of each tree by the learning rate(value). There is a trade-off between learning_rate and n_estimators. The default value is 0.1

*  **n_estimators** : The number of boosting stages to perform. The default value is 100

*  **loss** - It is the loss function to be optimized. The different loss functions are - ls, lad, huber, quantile, The default being 'ls'.  ‘ls’ refers to least squares regression. ‘lad’ (least absolute deviation) is a highly robust loss function solely based on order information of the input variables. ‘huber’ is a combination of the two. ‘quantile’ allows quantile regression (use alpha to specify the quantile).

*  **criterion** - It is the function to measure the quality of a split. It is {‘friedman_mse’, ‘mse’, ‘mae’}, 
 The criteria are 'friedman_mse' for the mean squared error with improvement score by Friedman, 'mse' for mean squared error and 'mae' for the mean absolute error. The default value is ’friedman_mse’
 
*  **max_depth** - It is the maximum depth of the individual regression estimators. it limits the number of nodes in the tree. We can tune this parameter for best performance; the best value depends on the interaction of the input variables. The default value being 3.
 






