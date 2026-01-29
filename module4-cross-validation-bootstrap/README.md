Problem 1
In Module 3, we used logistic regression to predict the probability of default using income and balance on the Default data set. We will now estimate the test error of this logistic regression model using the validation set approach. Do not forget to set a random seed before beginning your analysis.

A) Fit a logistic regression model that uses income and balance to predict default.

B) Using the validation set approach, estimate the test error of model in (a). In order to do this, you must perform the following steps:
1. Split the sample set into a training set and a validation set.
2. Fit a multiple logistic regression model using only the training observations.
3. Obtain a prediction of default status for each individual in the validation set by computing the posterior probability of default for that individual, and classifying the individual to the default category if the posterior probability is greater than 0.5.
4. Compute the validation set error, which is the fraction of the observations in the validation set that are misclassified.

C) Repeat the process in (b) using LOOCV to split of the observations into a training set and a validation set. Comment on the results obtained.

D) Repeat the process in (b) using k-fold (with k=5) to split of the observations into a training set and a validation set. Comment on the results obtained.

Problem 2
We continue to consider the use of a logistic regression model to predict the probability of default using income and balance on the Default data set. In particular, we will now compute estimates for the standard errors of the income and balance logistic regression coefficients using the bootstrap. Do not forget to set a random seed before beginning your analysis.

1. Write a function, boot.fn(), that takes as input the Default data set as well as an index of the observations, and that outputs the coefficient estimates for income and balance in the multiple logistic regression model.
2. Use the boot() function together with your boot.fn() function to estimate the standard errors of the logistic regression coefficients for income and balance.
3. Comment on the estimated standard errors obtained using the using your bootstrap function.
