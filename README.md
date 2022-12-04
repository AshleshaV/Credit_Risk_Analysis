# Credit_Risk_Analysis

### Overview
The main purpose of this analysis was to evaluate machine learning models to determine which is best for predicting credit risk. Numerous techniques are employed to evaluate and train models with unbalanced classes.

The machine learning models used in this challenge
Random Over Sampler,
SMOTE algorithms to oversample the dataset and
Cluster Centroids algorithm to undersample the dataset.
SMOTEENN algorithm will be utilized to over and under-sample.
Thereafter we compared Easy Ensemble Classifier both Balanced Random Forest Classfier to predict credit risk and then assess the performance of these models.
Different unbanlanced machine learning models were applied and compared the results. This was executed by observing variables, viewing the count of the target classes, then train the logistic regression classifier, and calculated the balanced accuracy score, generated a confusion matrix and thus finally we generated a classification report.

In this challenge the main purpose of analysis is to Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms. and then Compared the pros and cons of each supervised learning algorithm.
we can Determine which supervised learning algorithm is more appropriate for a given data.
Improve model performance by ensemble and resampling techniques.

### Results:
##### Naive Random Oversampling

This method handles class imbalances by duplicating the data in the minor class. For this dataset the minor class represents the high-risk loan applications and the major class the low-risk applications.

![](https://github.com/AshleshaV/Credit_Risk_Analysis/blob/main/Naive%20Random%20Oversampling.png?raw=true)

balanced accuracy test it 64%, the precision for the high_risk has a very low positivity at 1% and the recall is 60%

##### SMOTE Oversampling

This model matches the size of the major class with the minor class dataset. This is done by interpolating data from k-nearest neighbors rather than duplicating data like the Random Oversampling model.

![](https://github.com/AshleshaV/Credit_Risk_Analysis/blob/main/SMOTE%20Oversampling.png?raw=true)

the accuracy score is 66.2%, the precision for the high_risk loans has a low positvity again at 1% and recall is 69% overall

##### Undersampling

This model only employs existing data in the dataset rather than creating duplicates like the above models. But this approach may have a limitation of removing some data to ensure that the dataset is even.

![](https://github.com/AshleshaV/Credit_Risk_Analysis/blob/main/Undersampling.png?raw=true)

. Undersampling results: balanced accuracy score is 54% overall, the precision is at 99% and the recall is 40%

##### Combination (Over and Under) Sampling

-As the name suggest this model includes both over and under sampling methods

![](https://github.com/AshleshaV/Credit_Risk_Analysis/blob/main/Combination%20(Over%20and%20Under)%20Sampling.png?raw=true)

balanced accuracy score is 64% the precision is 99% and the recall is 57% overall

##### Balanced Random Forest Classifier

This model uses a mix of classification and regression technique to address imbalance data.

![](https://github.com/AshleshaV/Credit_Risk_Analysis/blob/main/Balanced%20Random%20Forest%20Classifier.png?raw=true)

Balanced Random Forest Classifier results: the accuracy score is 74.2% the precision is 99% and the recall is 85%

##### Easy Ensemble AdaBoost Classifier

![](https://github.com/AshleshaV/Credit_Risk_Analysis/blob/main/Easy%20Ensemble%20AdaBoost%20Classifier.png?raw=true)

. Easy Ensemble AdaBoost Classifier results: the accuracy score is 93% the precision is 99% and the recall is 94%

### Summary
In the first four models we undersampled, oversampled and did a combination of both to determine which model is best at predicting which loans are the highest risk.

The next two models we resampled the data using ensemble classifiers to try and predict which loans are high or low risk.

In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/combination models is low as well.

Ideally, we want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models.

It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.
