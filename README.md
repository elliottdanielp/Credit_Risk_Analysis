# Credit_Risk_Analysis

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

# Results:

- Naive Random Oversampling results: Our balanced accuracy test is 65%,
![image](https://user-images.githubusercontent.com/106495422/194461005-383cb7b1-253d-4c99-98b1-9578948332da.png)

- SMOTE oversampling results: the accuracy score is 66%, the precision for the high_risk loans has a low positvity again at 1% and recall is 68% overall
- 
![image](https://user-images.githubusercontent.com/106495422/194461436-d4592890-4786-4191-89dd-98a1878129c2.png)

- Undersampling results: balanced accuracy score is 66% overall, the precision is at 99% and the recall is 40%
![image](https://user-images.githubusercontent.com/106495422/194461653-7cbfcdcb-2807-4559-bf77-db82f97bfc63.png)

- Combination(over and undersampling) results: balanced accuracy score is 55% the precision is 99% and the recall is 57% overall
![image](https://user-images.githubusercontent.com/106495422/194461782-ffb28956-d9d2-475f-b172-698e6d9a1b41.png)

- Balanced Random Forest Classifier results: the accuracy score is 78% the precision is 99% and the recall is 88%
![image](https://user-images.githubusercontent.com/106495422/194461892-350bbd87-fe7b-4bb2-8133-a8609db6ec2d.png)

- Easy Ensemble AdaBoost Classifier results: the accuracy score is 92% the precision is 99% and the recall is 94%
![image](https://user-images.githubusercontent.com/106495422/194461985-071d0f96-55ff-4600-ab4c-d746ff9867be.png)

# Summary: 

In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. The next two models we resampled the data using ensemble classifiers to try and predict what loans are high or low risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is also low. Typically we look for a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.




