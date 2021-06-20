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

### SMOTE Model
![image](https://user-images.githubusercontent.com/76491891/122673774-07288280-d1a0-11eb-95f6-27ac3456337e.png)
![image](https://user-images.githubusercontent.com/76491891/122673782-127bae00-d1a0-11eb-8357-7e516d01d50e.png)
![image](https://user-images.githubusercontent.com/76491891/122673790-1e677000-d1a0-11eb-9b8f-3e3768c3cdb2.png)

- The balanced accuracy score of SMOTE model is 66%.
- The high-risk precision is 1% and the recall score is 63% which makes an F1 score of 2%.
- The low-risk precision is 100% and the recall score is 69% which makes an F1 score of 81%.

### ClusterCentroids Model
![image](https://user-images.githubusercontent.com/76491891/122673840-54a4ef80-d1a0-11eb-81fd-2d0a1fff57a5.png)
![image](https://user-images.githubusercontent.com/76491891/122673848-68e8ec80-d1a0-11eb-959a-d55440650bd2.png)
![image](https://user-images.githubusercontent.com/76491891/122673853-7b632600-d1a0-11eb-862d-b716d413a904.png)

- The balanced accuracy score of the ClusterCentroids model is 54%.
- The high-risk precision is 1% and the recall score is 68% which makes an F1 score of 1%.
- The low-risk precision is 100% and the recall score is 41% which makes an F1 score of 58%.
