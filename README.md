# SC1015_MiniProject_FDDC_Team6_TanTanTer
## About
This is a Mini-Project for SC1015 course (Introduction to Data Science and Artificial Intelligence) which focuses on Credit card Fraud from a dataset in Kaggle

## Dataset
https://www.kaggle.com/datasets/kelvinkelue/credit-card-fraud-prediction

This dataset offers a variety of attributes valuable for comprehensive analysis. It contains 555,719 instances and 22 attributes, a mix of categorical and numerical data types. More importantly, the dataset is complete with no null values.

## Project Aim and Motivation
Our project aim and motivation is to enhance credit card fraud detection by developing reliable and accurate fraudulent transaction detection mechanisms using Classification and Machine Learning algorithms to minimise financial losses for financial institutions and individuals.

## Contributors
- Tan Dan Feng - Problem Statement and Motivation, Sample Collection, AUROC evaluation, K-Nearest Neighbour, Slides
- Ter Wei Lin - Scaling, Data Cleaning, Data Visualisation, Logistic Regression Model, Presentation
- Tan Shi Qi - Data Balancing, Random Forest Classifier  Model, Multilayer Perceptron Model

## Project Overview
### 1. Practical Motivation and Problem Formulation
- Are we able to predict if a credit card transaction is fraudulent?
- What are some of the variables that can help in the prediction of credit card fraud?
- Which model would be the best to predict credit card fraud?

### 2. Sample Collection
**Exploring the Dataset**
- There are 11 numerical variables and 12 categorical variables
- The dataset has 23 columns and 555719 rows.
- Check for Unique Values for each variable
- There is no null value or duplicate value in the dataset

**Examining the Relationship Between Different Variables and Fraudulent Transactions**
- Utilised heatmap, barplot, and histogram for data visualisation
- Explored variables like gender and category and the general relation to 'is_fraud'

### 3. Data Cleaning
**Feature Engineering**
- We created a new variable, age from date of birth and the date of transaction.
- We undersampled the data to resolve the imbalanced data.
- We categorised the time of purchasing into time categories with one-hour interval
- We performed one-hot encoding on gender, category of purchases (category), and time (time_category).
- We cleaned the dataset to obtain a reliable gender ratio for fraudulent and non-fraudulent transactions.

**Correlation of Variables with Fraudulent Transactions**
- The chi-squared test is used for categorical variables
- Correlation coefficient and heat map is used for numerical variables
- Mann-Whitney U Test is used to examine the relationship between age and fraudulent transactions
- Explored variables like gender and category and the general relation to 'is_fraud'

**Feature Selection**

We select Category of Products (category), Time of Transaction (time_category), Transaction Amount (amt), Gender (gender) and Age (age) as these variables can significantly influence an individual's susceptibility to fraudulent transactions

**Feature Scaling**

We tested three scaling methods on the dataset, robust scaling, min-max scaling, and standard scaling. We choose standard scaling to scale our dataset.

### 4. Development of Fraud Detection Mechanism
We built and tested the accuracy, TPR, FNR, TNR, FPR, and AUC value for Random Forest Classifier model, Logistic Regression model, Multi-layer Perceptron model, and K-Nearest Neighbour model.

###  5.Evaluation of the Different Models Used
- We looked at different metrics in evaluating the best model.
- Random Forest Classifier Model has the highest accuracy of 0.97, highest TPR of 0.95, lowest FPR of 0.02, and highest AUC value of 0.99.

### 6. Final Analysis
- Amount of transaction, category of objects, gender, time of transaction, and age greatly influence the credit card fraud prediction
- The random forest classifier model is the most suitable model for credit card fraud prediction.

### 7. Outcome of Project
- By implementing robust and relevant machine learning models and techniques, the system can effectively identify suspicious activities and minimise false positives and false negatives
- Effective fraud detection prevents unauthorised transactions, reducing the risk of financial losses
- Using machine learning algorithms can reduce the manual effort needed for monitoring transactions
- Insights gained from data can be incorporated into fraud prevention strategies

### 8. New insights
- Solve the issue of imbalance data using undersampling
- Machine learning models, including Random Forest Classifier model, Logistic Regression model, Multi-layer Perceptron model, and K-Nearest Neighbour model
- Concepts of AUROC
- Feature engineering techniques such as creating new variables and scaling to tackle poor correlation between variables

### 9. Recommendations
- Implementing greater surveillance and scrutiny during high-risk periods and on high-risk platforms
- Collaborate with Industry Partners
- Raise Awareness

### 10. Conclusion

Further research and innovation is needed to stay ahead of emerging and sophisticated credit card frauds  and ensure the integrity and security of financial systems
