#  Task 2: Credit Risk Prediction for Loan Applications

## Overview
This project focuses on predicting the likelihood of loan approval using historical financial and demographic data. The goal is to build a classification model that helps financial institutions assess **credit risk** and make informed loan approval decisions.

## Objective
- Clean and preprocess the loan applicant dataset.
- Perform exploratory data analysis (EDA) to understand relationships between features.
- Build and evaluate a **Logistic Regression** model for credit risk prediction.
- Identify key features that influence loan approval outcomes.

##  Dataset Description
- Features include: Gender, Married, Education, Self_Employed, ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term, Credit_History, Property_Area
- Target variable: `Loan_Status` (Y: Approved, N: Rejected)
- Dataset contains a mix of **numerical** and **categorical** features.
- Missing values and duplicates are addressed.

##  Data Preprocessing
- Null values handled using appropriate imputations.
- Categorical features encoded using **Ordinal Mapping** and **One-Hot Encoding**.
- Numerical features scaled using **StandardScaler**.
- Dataset split into training and testing sets for model evaluation.

##  Exploratory Data Analysis (EDA)

### ➤ Univariate Analysis
- Used count plots, histograms, and KDE plots to understand feature distributions.

### ➤ Bivariate and Multivariate Analysis
- Explored relationships between input features and `Loan_Status`.
- Boxplots and countplots used for visual insights.
- Correlation heatmaps helped identify redundant features.

##  Modeling

### Model Used: **Logistic Regression**
- Chosen for its simplicity, interpretability, and good performance on binary classification tasks.

### Evaluation Metrics:
- Accuracy Score
- Confusion Matrix
- Precision, Recall, F1-score (via Classification Report)

###  Performance:
- **Accuracy:** ~76%
- Model performs well with acceptable recall and precision, especially in identifying approved loans.

##  Key Insights
1. **Credit History** is the most decisive factor in loan approval.
2. Applicants with **higher income** and **lower loan amounts** are more likely to be approved.
3. Education and property area show moderate influence, while gender and marital status have less impact.
4. The dataset had class imbalance, but logistic regression still handled it effectively.

##  Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

## skills
- Data cleaning and handling missing values
- Exploratory Data Analysis (EDA)
- Binary classification using machine learning
- Model evaluation using confusion matrix and accuracy
