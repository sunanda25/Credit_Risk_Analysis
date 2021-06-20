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

### SMOTEENN Model
![image](https://user-images.githubusercontent.com/76491891/122673875-a0f02f80-d1a0-11eb-812f-6f1e9cec6af5.png)
![image](https://user-images.githubusercontent.com/76491891/122673889-b2393c00-d1a0-11eb-8f7a-a424027bf79e.png)
![image](https://user-images.githubusercontent.com/76491891/122673911-c41adf00-d1a0-11eb-93a6-f015dde06af5.png)

- The balanced accuracy score of the SMOTEENN model is 63%.
- The high-risk precision is 1% and the recall score is 70% which makes an F1 score of 2%.
- The low-risk precision is 100% and the recall score is 57% which makes an F1 score of 72%.

### BalancedRandomForestClassifier Model
![image](https://user-images.githubusercontent.com/76491891/122673944-f7f60480-d1a0-11eb-8686-8b7a5fdad1b8.png)
![image](https://user-images.githubusercontent.com/76491891/122673959-080de400-d1a1-11eb-84fa-22fb78e47a44.png)
![image](https://user-images.githubusercontent.com/76491891/122673966-178d2d00-d1a1-11eb-9cb3-34d6c3b04bf4.png)

- The balanced accuracy score of the BalancedRandomForestClassifier model is 79%.
- The high-risk precision is 3% and the recall score is 70% which makes an F1 score of 6%.
- The low-risk precision is 100% and the recall score is 87% which makes an F1 score of 93%.

### EasyEnsembleClassifier Model
![image](https://user-images.githubusercontent.com/76491891/122673986-34c1fb80-d1a1-11eb-8527-373bb61c7fb9.png)
![image](https://user-images.githubusercontent.com/76491891/122674004-4c997f80-d1a1-11eb-9604-4287abf0da09.png)
![image](https://user-images.githubusercontent.com/76491891/122674019-5e7b2280-d1a1-11eb-9b3c-f6fcb0abb363.png)

- The balanced accuracy score of the EasyEsembleClassifier model is 93%.
- The high-risk precision is 9% and the recall score is 92% which makes an F1 score of 16%.
- The low-risk precision is 100% and the recall score is 94% which makes an F1 score of 97%.

## Summary
The Oversampled, Undersampled, combination of both, Ensemble models have been used to determine which model is best in predicting credit risk. The accuracy scores for both Ensemble classifier models (79%, 93%) are high compared to the remaining models (68%, 66%, 54%, 63%). The EasyEnsembleClassifier model has a high accuracy score of 93% and a recall of 92% which detects almost all high-risk credit. Based on the accuracy, precision, and recall scores, the Ensemble classifiers models are recommended over the remaining models to predict credit risk.
