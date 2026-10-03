# PREDICTIVE MODELING USING MACHINE LEARNING

## 1. Project Title
**Customer Churn Prediction Using Random Forest**

## 2. Objective
The objective of this project is to build a supervised machine-learning model that predicts whether a customer is likely to churn based on customer and service information.

## 3. Dataset
No dataset was supplied for the task. Therefore, a realistic synthetic customer dataset containing **600 original records** was generated. The raw dataset intentionally contains missing values, duplicate records and extreme values so that the complete ML workflow can be demonstrated.

### Features
- Age
- Tenure in months
- Monthly charges
- Support calls
- Usage hours
- Late payments
- Contract type
- Satisfaction score
- Internet type

### Target
- **Churn**: 0 = No Churn, 1 = Churn

## 4. Data Preprocessing
The following preprocessing steps were performed:
1. Removed duplicate records.
2. Filled missing monthly charges using the median.
3. Filled missing satisfaction scores using the median.
4. Detected and capped extreme values using the IQR method.
5. Separated features and target variable.
6. Converted categorical variables using One-Hot Encoding.
7. Standardized numerical features.
8. Split the dataset into 80% training data and 20% testing data.

## 5. Algorithm Used
### Random Forest Classifier
Random Forest is an ensemble machine-learning algorithm that combines many decision trees. Each tree makes a prediction and the final prediction is obtained from the combined results.

Advantages:
- Handles nonlinear relationships.
- Works with many features.
- Less prone to overfitting than a single decision tree.
- Provides probability estimates.
- Suitable for classification tasks.

## 6. Model Evaluation
The model was evaluated using:

- **Accuracy:** 0.7417
- **Precision:** 0.6486
- **Recall:** 0.5714
- **F1 Score:** 0.6076
- **ROC-AUC:** 0.7353

A confusion matrix and ROC curve are included with the project files.

## 7. Interpretation
The model attempts to identify customers who are likely to leave the service. Features such as support calls, late payments, contract type, satisfaction and monthly charges provide useful predictive information in this synthetic dataset.

## 8. Conclusion
This project demonstrates a complete supervised machine-learning workflow:

**Dataset → Cleaning → Preprocessing → Train/Test Split → Random Forest → Prediction → Evaluation → Visualization**

The project provides practical experience with model training and evaluation using Python and Scikit-learn.
