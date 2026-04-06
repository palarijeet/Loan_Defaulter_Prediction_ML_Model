# Loan_Defaulter_Prediction_ML_Model
This project builds a Machine Learning model to predict loan default risk using customer financial data. It includes data cleaning, EDA, feature engineering, and model building. The model achieves high accuracy with strong precision and recall, helping identify high-risk applicants.
 Loan Default Prediction using Machine Learning
 Project Overview
This project aims to build a Machine Learning model to predict whether a customer is likely to default on a loan based on various financial and demographic features.
The goal is to help financial institutions make better lending decisions and reduce financial risk.

 Objective
Predict loan default (0 = No Default, 1 = Default)
Perform data cleaning and exploratory data analysis (EDA)
Apply feature engineering techniques
Train and evaluate machine learning models

 Dataset Features
Some key features used in the dataset:
person_age
person_income
person_home_ownership
loan_amnt
loan_int_rate
loan_percent_income
cb_person_cred_hist_length

Data Preprocessing
Handled missing values using median/mode
Removed or treated outliers (e.g., unrealistic age values > 100)
Converted categorical variables using encoding techniques
Cleaned numeric columns (removed commas, converted to float)
Feature engineering:
Created loan_with_interest using: loan_amnt × interest_rate × term_years


 Exploratory Data Analysis (EDA)
Checked data distributions using histograms
Identified outliers using boxplots
Analyzed relationships between variables
Visualized missing values using heatmaps

 Model Building
Split data into training and testing sets
Used machine learning algorithms (e.g., Random Forest / Logistic Regression)
Trained model on processed dataset

 Model Performance
 Accuracy
95.84%
 Confusion Matrix
[[5010  132]
 [ 139 1235]]
 Classification Report
              precision    recall  f1-score   support

           0       0.97      0.97      0.97      5142
           1       0.90      0.90      0.90      1374

    accuracy                           0.96      6516
   macro avg       0.94      0.94      0.94      6516
weighted avg       0.96      0.96      0.96      6516

Key Insights
The model achieved high accuracy and balanced performance
Significant improvement in detecting defaulters
Reduced false negatives, lowering financial risk
Both precision and recall are strong for both classes

 Challenges Faced
Handling missing and inconsistent data
Dealing with categorical variables
Managing outliers
Ensuring proper data type conversions

 Future Improvements
Apply advanced models (XGBoost, Gradient Boosting)
Perform hyperparameter tuning
Use cross-validation
Deploy model using Flask/Streamlit
Improve recall for high-risk customers

 Tech Stack
Python
Pandas
NumPy
Matplotlib / Seaborn
Scikit-learn

 Conclusion
This project demonstrates the complete machine learning workflow from data preprocessing to model evaluation. The model performs well in predicting loan defaults and can be further improved for real-world deployment.

 Author
Arijeet Pal
