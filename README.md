**Bank Churn Prediction Using Machine Learning**

**Project Overview**

Customer churn is a major challenge in the banking industry, as retaining existing customers is often more cost-effective than acquiring new ones. This project applies machine learning techniques to predict customer churn and identify the key factors that influence customer attrition.

Using customer demographic and banking behavior data, multiple classification models were developed and evaluated to determine the most effective approach for predicting whether a customer is likely to leave the bank.

**Objectives**

The main objectives of this project were to:

* Explore and understand customer characteristics associated with churn.
* Perform data cleaning and preprocessing.
* Conduct exploratory data analysis (EDA).
* Build and evaluate machine learning models for churn prediction.
* Compare model performance.
* Identify the most important features driving customer churn.

**Dataset**

The dataset contains customer information including:

* Credit Score
* Geography
* Gender
* Age
* Tenure
* Account Balance
* Number of Products
* Credit Card Ownership
* Active Membership Status
* Estimated Salary
* Churn Status (Exited)

Target Variable:

**Exited**
* 0 = Customer Retained
* 1 = Customer Churned

**Methodology**

**1. Data Preprocessing**

The following preprocessing steps were performed:

* Removed irrelevant identifiers:
    * RowNumber
    * CustomerId
    * Surname
* Checked for missing values and duplicates.
* Encoded categorical variables.
* Split data into training and testing sets.
* Applied feature scaling where necessary.
  
**2. Exploratory Data Analysis (EDA)**

EDA was conducted using:

* Descriptive statistics
* Histograms
* Boxplots
* Count plots
* Correlation heatmaps
* Pair plots

The analysis helped identify patterns and potential relationships between customer characteristics and churn behavior.

**3. Machine Learning Models**

Three classification models were implemented:

1. Logistic Regression
2. Random Forest
3. XGBoost

Model performance was evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

**Model Performance**

| Model               | Accuracy | Recall (Churn) | F1-Score (Churn) |
| ------------------- | -------- | -------------- | ---------------- |
| Logistic Regression | 81.0%    | 14%            | 23%              |
| Random Forest       | 85.6%    | 43%            | 55%              |
| XGBoost             | 86.75%   | 47%            | 59%              |

**Best Model**

XGBoost achieved the highest performance across the evaluated metrics and was selected as the final model for customer churn prediction.

**Feature Importance**

Feature importance analysis using XGBoost identified the following key predictors of customer churn:

1. Number of Products
2. Active Membership Status
3. Age
4. Geography
5. Gender

These findings suggest that customer engagement and product usage play a significant role in customer retention.

Key Findings
* Customers with different product ownership patterns exhibit varying churn behavior.
* Active members are less likely to leave the bank.
* Age is a significant predictor of churn.
* Geographic location influences customer retention.
* XGBoost outperformed both Logistic Regression and Random Forest models.

**Conclusion**

The project demonstrates the effectiveness of machine learning in predicting customer churn. Among the evaluated models, XGBoost provided the best predictive performance, achieving an accuracy of 87%.

The analysis further revealed that customer engagement indicators such as product ownership and active membership status are among the strongest drivers of churn. These insights can support targeted retention strategies and help financial institutions reduce customer attrition.

**Technologies Used**

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Google Colab

**Future Improvements**

1. Hyperparameter tuning for XGBoost.
2. Address class imbalance using advanced sampling techniques.
3. Deploy the model as a web application.
4. Incorporate customer transaction and behavioral data.
5. Implement real-time churn prediction pipelines.
