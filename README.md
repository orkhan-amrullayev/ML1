# 2 Machine Learning Projects for ML1 course at University of Warsaw

## 1. Fraud Detection in Bank Transactions


In this paper, bank transactions will be used to predict fraudulent ones.

As per description of the dataset, it contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

add Codeadd Markdown
This paper will compare various data balancing techniques with powerful boosting models. Models used here are Random Forest, XGBoost and LGB. We will look at precision-recall curve and roc curve.


Content
1. Imports and reading dataset
2. Exploratory Data Analysis
3. Dealing with unbalanced dataset
- Without balancing
- Undersampling
- Oversampling

4. Building function for 3 models:

  - Random forest classifier

  - XGBoost

  - LightGBM

5. Comparison of result of the models with "Without balancing", "Undersampling", "Oversampling" options
6. Conclusion





## 2. Insurance Cost Prediction

A health insurance firms can make money if it collects more than it spends on the medical care of its beneficiaries. Even though some conditions are more prevalent for certain segments of the population, medical costs are difficult to predict since most money comes from rare conditions of the patients. The objective of this paper is to accurately predict insurance costs based on people’s data listed below.

age: age of primary beneficiary
sex: insurance contractor gender, female, male
bmi: Body mass index, providing an understanding of body, weights that are relatively high or low relative to height, objective index of body weight (kg / m ^ 2) using the ratio of height to weight, ideally 18.5 to 24.9
children: Number of children covered by health insurance / Number of dependents
smoker: Smoking
region: the beneficiary's residential area in the US, northeast, southeast, southwest, northwest.
charges: Individual medical costs billed by health insurance (dependent)

Content
1. Importing libraries and reading dataset
2. General exploratory Data Analysis
3. Relationship between features
4. Data Preparation
5. Conclusion of EDA
6. Label encoding
7. Modelling
8. DecisionTree
  - RandomForest
  - KNeighbors
  - AdaBoostRegressor
  - GradientBoosting
  - XGBRegressor
9. Cross Validation
10. Model Accuracy Comparison
