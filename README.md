# Credit_Risk_Analysis
## Overview
LendingClub, a peer-to-peer lending services company wants to use machine learning to predict credit risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Management believes machine learning will provide more accurate identification of good candidates for loans which will lead to lower default rates. The imbalanced-learn and scikit-learn libraries in Python are used to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, the performance of the following models is evaluated, and a recommendation is made whether they should be used to predict credit risk.

- Oversample the data using RandomOverSampler and SMOTE algorithms.
- Undersample the data using the ClusterCentroids algorithm.
- A combinatorial approach of Over and Undersampling using the SMOTEENN algorithm.
- Compare the BalancedRandomForestClassifier and EasyEnsembleClassifier machine learning models to predict credit risk.

## Results
- Using balance accuracy score from sklearn.metrics library, the accuracy score is calculated. 
- Using classification report imbalanced from imblearn.metrics library, the precision, and recall scores are calculated.

### RandomOverSampler Model
![image](https://user-images.githubusercontent.com/76491891/122673680-98e3c000-d19f-11eb-94f1-8686e023d857.png)
![image](https://user-images.githubusercontent.com/76491891/122673692-a6994580-d19f-11eb-826c-6688919030a5.png)
![image](https://user-images.githubusercontent.com/76491891/122673711-ba44ac00-d19f-11eb-8b9b-721a865f8797.png)

- The balanced accuracy score of the RandomOverSampler model is 68%.
- The high-risk precision is 1% and the recall score is 75% which makes an F1 score of 2%.
- The low-risk precision is 100% and the recall score is 61% which makes an F1 score of 75%.
