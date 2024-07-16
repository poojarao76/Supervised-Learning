# Rain Prediction in Australia

## Introduction

This project uses Logistic Regression with Python and Scikit-Learn to predict whether it will rain tomorrow in Australia. The model is trained using the Rain in Australia dataset from Kaggle.


## The problem statement

Ever wondered if you should carry an umbrella tomorrow? With this dataset, you can predict next-day rain by training classification models on the target variable RainTomorrow.

This dataset comprises about 10 years of daily weather observations from numerous locations across Australia.

This dataset contains daily weather observations from numerous Australian weather stations

## Dataset 

I have downloaded this data set from the Kaggle - Rain in Australia

This dataset comprises about 10 years of daily weather observations from numerous locations across Australia.

RainTomorrow is the target variable to predict. It answers the crucial question: will it rain the next day? (Yes or No).

## Conclusion

1. The logistic regression model accuracy score is 0.8484. So, the model does a very good job in predicting whether or not it will rain tomorrow in Australia.
2. The model shows no signs of overfitting.
3. ROC AUC of our model approaches towards 1. So, we can conclude that our classifier does a good job in predicting whether it will rain tomorrow or not.
4. Original model accuracy score is 0.8484 whereas accuracy score after RFECV is 0.8485. So, we can obtain approximately similar accuracy but with reduced or optimal set of features.
5. In the original model, we have FP = 1204 whereas FP1 = 1194. So, we get approximately same number of false positives. Also, FN = 3207 whereas FN1 = 3213. So, we get slighly higher false negatives.
6. Original model score is found to be 0.8486. The average cross-validation score is 0.8482. So, we can conclude that cross-validation does not result in performance improvement.
7. Original model test accuracy is 0.8484 while GridSearch CV accuracy is 0.8488. We can see that GridSearch CV improve the performance for this particular model.