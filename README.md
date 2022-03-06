# Credit_Risk_Analysis
Overview: After learning and building up skills in data preparation, statistical reasoning and machine learning . We are tasked to  apply machine learning to sove a real=world challenge: credit card risk using credit card dataset from  Lending Club, a peer to peer lending services company.

To build and evaluate models, we use **imbalanced-learn** and **scikit-learn libraries** for resampling.The following are used to employ different techniques to train and evaluate models with unbalanced classes to predict credit risk:

  -  Oversample the data using the **RandomOverSampler** and **SMOTE algorithms**
  - Undersample the data using the **ClusterCentroids** algorithm
  - Use a combinatorial approach of over and undersampling using the **SMOTEENN** algorithm
  -  Compare two new machine learning models that reduce bias, **BalancedRandomForestClassifier** and **EasyEnsembleClassifier**, to predict credit risk.

# **Results:**
Below are the results of the balanced accuracy scores, precision and recall scores of all six machine learning models:

1. **Naive Random Oversampling**
Balanced accuracy scores: 0.6293939430565123
Precision: low at .01 for high risk, and high for at 1.0 for low risk
Recall scores:high risk at .57,  low risk at .68
F1: high risk at .02 , low risk at .81
![Naive Random Oversampling](https://user-images.githubusercontent.com/92903447/156906030-83f939a7-214e-4f38-9d04-599fe516a417.png)


2. **SMOTE Oversampling**
Balanced accuracy scores: 0.6277008271188627
Precision: low at .01 for high risk, and high for at 1.0 for low risk
Recall scores:high risk at .62,  low risk at .63
F1: high risk at .02 , low risk at .78
![Smote Oversampling](https://user-images.githubusercontent.com/92903447/156906033-3e23dd08-56bd-46ea-b29d-4d4e3f163649.png)

3. **Undersampling**
Balanced accuracy scores: 0.5296239892671961
Precision: low at .01 for high risk, and high for at 1.0 for low risk
Recall scores:high risk at .61,  low risk at .45
F1: high risk at .01 , low risk at .62
![Undersampling](https://user-images.githubusercontent.com/92903447/156906046-dd7fe8eb-a68d-4456-a58e-e6c1461d04c3.png)

4. **Combination (Over and Under) Sampling**
Balanced accuracy scores:0.5296239892671961
Precision: low at .01 for high risk, and high for at 1.0 for low risk
Recall scores:high risk at .70,  low risk at .61
F1: high risk at .02 , low risk at .76
![Combination_over_under_sampling](https://user-images.githubusercontent.com/92903447/156906065-34b28cca-ddc4-4971-869f-538ea32fa2bc.png)

5. **Balanced Random Forest Classifier**
Balanced accuracy scores:0.7877672625306695
Precision: low at .04 for high risk loans, and high for at 1.0 for low risk loans
Recall scores:high risk at .67,  low risk at .91
F1: high risk at .07 , low risk at .95
![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/92903447/156906102-973e407b-7609-4227-8a50-a5bffa69460e.png)

6. **Easy Ensemble AdaBoost Classifier**
Balanced accuracy scores:0.925427358175101
Precision: low at .07 for high risk loans, and high for at 1.0 for low risk loans
Recall scores:high risk at .91,  low risk at .94
F1: high risk at .14 , low risk at .97
![Easy Ensemble Adaboost Classifier](https://user-images.githubusercontent.com/92903447/156906112-93becbc8-35f0-4e52-a35e-ce77a0b73348.png)

# **Summary:** 
After running all the different evaluation techniques and models to predict credit risk, when working with the dataset the highest compared accuracy is between 0 to 1, and closest to 1 is the best machine learning model for balanced accuracy. Easy Ensemble AdaBoost Classifier was the best-performing model and gave a balanced accuracy score of .925, that could mean it could accurately predict a rate closer to 93% of the appropriate levels of credit risk, however its F1 score for high risk was no better for .16. which makes it too risky being unable to predict who the high risk debtors would be.


