# Customer_Churn
Classification modeling project to predict churn

# Client / Background
- Connex is a fictitous communications company that provides phone, internet, and streaming services. In addition, they offer supportive services like online security, device protection, etc. 

- Connex would like to utilize machine learning methodologies to create a model that gives them the ability to get ahead of customer churn.

# Business Questions
- What model can best predict churn?
- Which features (inputs) are more likely to predict churn?

# Data to Answer the Question
- 7032 Observations (rows)
- 30 Features (columns)
- [Kaggle dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) 

# Solution Path
#### EDA + Benchmark
- [Cleaned data and Get Dummies](https://github.com/Jenni-Hawk/Customer_Churn/blob/main/01_Clean_GetDummies.ipynb)
- [Used Logistic Regression to explore the data and create a benchmark model](https://github.com/Jenni-Hawk/Customer_Churn/blob/main/03_Logistic_Reg_Explore.ipynb)
1. Created a model without oversampling
2. Created model with oversampling
    - Class imbalance just on edge of potentially being problematic. Negative class represents 72% of the data. Typically problematic at 80%
    - Addressed Class Imbalance with oversampling using imblearn to gain experience with the process.
3. Compared the Key Metrics for each model: ROC AUC, Recall
4. Reviwed Confusion matrix for each model. 
    - With oversampling recall score greatly improved 
    - With oversampling more customers were being correctly identified as churnin

#### Tested More Models
- [Decision Trees, Random Forest and XGBoost](https://github.com/Jenni-Hawk/Customer_Churn/blob/main/04_Tree_vs_Forest_vs_LogReg.ipynb)

#### Tuned Hyperparamters
- [Tune hyperparameters using Gridsearch](https://github.com/Jenni-Hawk/Customer_Churn/blob/main/05_Tuning_GridSearch.ipynb)

#### Determine Winner
- Best performing model
- Most important features

#### Identify Further Optimizations
- Identify further tuning opportunities

# Findings
Check out the [presentation](https://github.com/Jenni-Hawk/Customer_Churn/blob/main/CustomerChurn_Presentation.pdf)

# Tech Tools Used
- Pandas
- Sklearn
- Imblearn
- Numpy
