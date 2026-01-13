# Task 2: End-to-End ML Pipeline (Telco Churn)

## 🎯 Objective
To build a production-ready machine learning pipeline using the **Scikit-learn Pipeline API**. The project focuses on predicting customer churn for a telecommunications company.

## 🛠️ Technical Implementation
* **Data Preprocessing:** Used `ColumnTransformer` to handle different data types:
    * **Numerical Features:** Scaled using `StandardScaler`.
    * **Categorical Features:** Encoded using `OneHotEncoder`.
* **Model Selection:** Implemented `GridSearchCV` to compare and tune **Logistic Regression** and **Random Forest** algorithms.
* **Persistence:** The entire pipeline (preprocessing + model) was exported as a `.joblib` file for deployment.



## 🚀 Key Insights
* **Pipeline Integrity:** Using the Pipeline API prevents "Data Leakage" during training and ensures the model is robust for production.
* **Automation:** The use of `GridSearchCV` ensures that we are always using the most optimal version of the model.
* **Scalability:** The exported model can handle raw, uncleaned data inputs because the preprocessing is built directly into the pipeline file.
