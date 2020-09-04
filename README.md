# Credit-card-fraud
In this project I build machine learning models to identify fraud in European credit card transactions. I also make several data visualizations to reveal patterns and structure in the data.

The dataset, hosted on Kaggle, includes credit card transactions made in September 2013 by European cardholders. The data contains 284,807 transactions that occurred over a two-day period, of which 492 (0.17%) are fraudulent. Each transaction has 30 features, all of which are numerical. The features V1, V2, ..., V28 are the result of a PCA transformation. To protect confidentiality, background information on these features is not available. The Time feature contains the time elapsed since the first transaction, and the Amount feature contains the transaction amount. The response variable, Class, is 1 in the case of fraud, and 0 otherwise.

I was able to accurately identify fraudulent transactions using a random forest model. I also calculated mutual information values to identify the variables most correlated with fraud. On a test set consisting of 20% of the original data, the predictions from the random forest model had an F1 score of 0.869 and a Matthews correlation coefficient (MCC) of 0.869. I also trained logistic regression and linear support vector classifier models, but these models underperformed the random forest. To improve a particular model, I optimized hyperparameters via a grid search with 5-fold cross-validation.


https://www.kaggle.com/mlg-ulb/creditcardfraud
