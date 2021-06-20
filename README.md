# Credit_Risk_Analysis
## Overview
LendingClub, a peer-to-peer lending services company wants to use machine learning to predict credit risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Management believes machine learning will provide more accurate identification of good candidates for loans which will lead to lower default rates. The imbalanced-learn and scikit-learn libraries in Python are used to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, the performance of the following models is evaluated, and a recommendation is made whether they should be used to predict credit risk.

- Oversample the data using RandomOverSampler and SMOTE algorithms.
- Undersample the data using the ClusterCentroids algorithm.
- A combinatorial approach of Over and Undersampling using the SMOTEENN algorithm.
- Compare the BalancedRandomForestClassifier and EasyEnsembleClassifier machine learning models to predict credit risk.
