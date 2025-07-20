# BankMarketingDataset
This project builds and evaluates machine learning models to predict whether a customer will subscribe to a term deposit using the Bank Marketing dataset. It includes full preprocessing, model training (Logistic Regression, Random Forest, XGBoost), hyperparameter tuning.

##  Problem Statement

The goal is to help a bank target potential customers more effectively by predicting which customers are likely to say **"yes"** to a term deposit offer.

##  Dataset

- **Target Variable**: `y` (binary - "yes" or "no")
- **Features**: Includes job, marital status, education, contact type, campaign info, etc.

##  ML Pipeline

1. **Data Preprocessing**
   - Handled missing values
   - One-hot encoded categorical features
   - Label-encoded target variable

2. **Model Training**
   - Logistic Regression
   - Random Forest
   - XGBoost Classifier

3. **Model Tuning**
   - Hyperparameter tuning using `RandomizedSearchCV` for XGBoost

4. **Evaluation**
   - Accuracy, Precision, Recall, F1-score, Confusion Matrix
   - Focused on **recall and F1-score** for the minority class ("yes")

##  Results

| Model               | Accuracy | Recall (yes) | F1-score (yes) |
|---------------------|----------|--------------|----------------|
| Logistic Regression | 90.1%    | 0.35         | 0.45           |
| Random Forest       | 90.7%    | 0.40         | 0.50           |
| **XGBoost (Tuned)** | 88.6%    | **0.80**     | **0.62**       |

 **Final Model:** Tuned XGBoost  
 **Best for business impact due to high recall and lower false negatives**

##  Business Value

- Helps reduce customer acquisition costs by focusing on high-probability leads
- Increases marketing efficiency and ROI
- Supports data-driven targeting strategies



