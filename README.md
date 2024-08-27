# Credit Card Transaction Fraud Analysis

#### Project Overview
This project focuses on detecting fraudulent credit card transactions using a dataset originally sourced from a US government organization in Tennessee. The dataset, provided by Mark Nigrini, a renowned expert in forensic accounting, comprises approximately 100,000 real card transaction records.

#### Data Preparation and Feature Engineering
- **Data Cleaning**: Addressed missing values, outliers, and data inconsistencies. Categorical variables were transformed into numerical ones using one-hot encoding. Variables deemed irrelevant or exhibiting high multicollinearity were excluded.
- **Feature Engineering**: Developed 184 distinct variables that captured various aspects of the transaction data, including date-related, geographic, and time-based features like Day Since, Velocity, and Cross-entity uniqueness, enhancing the model’s ability to discern patterns indicative of fraud.

#### Model Development and Selection
- **Feature Selection**: Implemented feature selection using LGBM and Random Forest classifiers, applying forward and backward selection methods to distill the most impactful predictors.
- **Model Testing**: Evaluated multiple machine learning models such as Logistic Regression, Decision Trees, Neural Networks, LightGBM, and XGBoost. XGBoost was selected based on its superior performance and scalability.

#### Model Validation and Performance
- **Validation Strategy**: The model was rigorously validated across training, testing, and out-of-time (OOT) datasets to ensure robustness and reliability.
- **Performance Metrics**:
  - **Training Dataset**: Achieved a Fraud Detection Rate (FDR) at 3% of 76.40%, demonstrating strong predictive capabilities.
  - **Testing Dataset**: Recorded a FDR at 3% of 76.26%, confirming the model's effectiveness in controlled scenarios.
  - **Out-of-Time (OOT) Dataset**: Secured a FDR at 3% of 56.98%, showcasing the model’s performance in predicting future, unseen data scenarios.
- **Financial Impact**: The implementation of this model is projected to save approximately $21.22 million annually by reducing fraud-related financial losses.

## Impact
In business terms, the model's financial impact was analyzed to estimate the potential savings that could be achieved by implementing the XGBoost model with a recommended score cutoff at 3%. The analysis revealed an anticipated savings of about $21.22 million per year, showcasing the model's effectiveness in detecting and preventing fraudulent transactions.  
