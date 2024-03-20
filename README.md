# Bank Customers Behavior Prediction

## Introduction
This project aims to predict the behavior of bank customers regarding their deposit subscription. It involves building predictive models using various machine learning algorithms and evaluating their performance.

## Dataset
The dataset contains information about bank customers, including demographic features, financial status, and previous marketing interactions. It consists of 11,162 entries and 15 columns.

## Data Preprocessing
- Modified the target variable to have binary values (0/1).
- Assessed categorical variables and visualized their distributions.
- Conducted feature engineering and handled categorical variables by creating dummy features.
- Scaled numerical features using MinMax scaling.

## Model Building
- Divided the data into train and test sets.
- Built logistic regression and random forest models.
- Evaluated the models' performance on both training and test sets.
- Conducted cross-validation to assess the models' generalization performance.

## Feature Selection
- Utilized Recursive Feature Elimination (RFE) and Recursive Feature Elimination with Cross-Validation (RFECV) for feature selection.
- Identified important features based on model performance and cross-validation scores.

## Hyperparameter Tuning
- Performed hyperparameter tuning using RandomizedSearchCV for the Random Forest model.
- Evaluated various combinations of hyperparameters to optimize the model's performance.

## Results
- Logistic Regression:
  - Training Accuracy: 70.98%
  - Test Accuracy: 69.32%

- Random Forest:
  - Training Accuracy: 99.85%
  - Test Accuracy: 69.32%

- Cross-Validation:
  - Logistic Regression Mean CV Score: 70.24%
  - Random Forest Mean CV Score: 69.24%
  - LeaveOneOut Mean SV Score: 66.90%

- Hyperparameter Tuning:
  - Best Random Forest Model:
    - Max Depth: 15
    - Max Features: 15
    - Min Samples Leaf: 20
    - N Estimators: 100
    - Mean CV Score: 71.86%

## Conclusion
- Logistic Regression and Random Forest models were built to predict bank customers' deposit subscription behavior.
- Feature selection techniques such as RFE and RFECV were employed to identify important features.
- Hyperparameter tuning was performed to optimize the Random Forest model's performance.
- The best-performing model achieved an accuracy of 71.86% on cross-validation.
- Further improvements could be made by exploring other machine learning algorithms and conducting more extensive feature engineering.
