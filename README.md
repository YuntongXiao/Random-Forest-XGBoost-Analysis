### Random-Forest-XGBoost-Analysis
###### According to the two model the Mean Absolute Error, Mean Squared Error and Root Mean Squared Error for XGboost are all smaller than ramdon forest model, the prediction accuarcy for XGboost is higher than ramdon forest one. But for the cross validation score of XGboost is less than the random forest model.  When compared with random forest, boosting is highly efficient on both classification and regression tasks and should be more accurate predictions compared to random forests. Also it can handle mixed type of features and no pre-processing is neede. 

###### However, too large number of n_estimators might cause overfitting which results in the less predict power for out of sample data.Compared with random forest, xboost is hard to parallelize / slower and requires careful tuning of hyperparameters.It also may overfit if too many trees are used (n_estimators) and sensitive to outlier

###### Random forest conbined simple decision trees to improve accuracy, it create bootstraps from the orginal dataset. Then is creats decsion trees based on the bootstrap dataset but based on subset of some randomly chosen variables. Then it goes through all the decision trees to collect the classification result of the test varibale. It draws conclusion based on the persentage of results in every trees. Then we can identfy the accuracy of the random forest model based on the out-of-bag smaples prediction. By changing the number of variables used in each step and choose the most accuracte one.

###### XGBoost similary use decision trees to predict the target, however, it calculates the similarity scores based on the residuals of prediction and the gain score to determinate how to split the data. And then purnes the tree by comparing the difference between the gain and gamma (tree complexity parameter). And it use lambda as the regularization parameter to shrinkage the similarity score to decrease the difference between output values. Then it repeat calculating the residuals to make the prediction closer to the ture value. XGBoost minimizes a regularized (L1 and L2) objective function that combines a convex loss function (based on the difference between the predicted and target outputs) and a penalty term for model complexity.
