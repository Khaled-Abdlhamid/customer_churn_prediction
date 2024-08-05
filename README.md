# Telecomm Customer Churn Prediction

### Objective
The objective of this project is to predict customer churn for a telecommunications company using a dataset from Kaggle. The dataset contains various customer attributes, and the goal is to develop a machine learning model to identify customers likely to churn.


### Column Dictionary:
- customerID: Unique ID for each customer
- gender: Gender of the customer
- SeniorCitizen: Whether the customer is a senior citizen (1) or not (0)
- Partner: Whether the customer has a partner (Yes, No)
- Dependents: Whether the customer has dependents (Yes, No)
- tenure: Number of months the customer has stayed with the company
- PhoneService: Whether the customer has phone service (Yes, No)
- MultipleLines: Whether the customer has multiple lines (Yes, No, No phone service)
- InternetService: Customer’s internet service provider (DSL, Fiber optic, No)
- OnlineSecurity: Whether the customer has online security (Yes, No, No internet service)
- OnlineBackup: Whether the customer has online backup (Yes, No, No Internet Service)
- DeviceProtection: Whether the customer has device protection (Yes, No, No Internet Service)
- TechSupport: Whether the customer has tech support (Yes, No, No Internet Service)
- StreamingTV: Whether the customer has streaming TV (Yes, No, No Internet Service)
- StreamingMovies: Whether the customer has streaming movies (Yes, No, No Internet Service)
- Contract: The type of contract the customer has (Month-to-Month, One year, Two years)
- PaperlessBilling: Whether the customer has paperless billing (Yes, No)
- PaymentMethod: Payment method used by the customer (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))
- MonthlyCharges: Amount charged to the customer monthly
- TotalCharges: The total amount charged to the customer
- Churn: Whether the customer churned (Yes) or not (No)
 

### Preprocessing and EDA:
- Binary encoded relevant categorical features.
- One-hot encoded other categorical features.
- Scaled numeric features.
- Used SMOTE and SMOTEENN for handling the imbalance issue.


### Training:
- Trained Logistic Regression, RandomForestClassifier, SVC, GradientBoosting, AdaBoost


### Challanges
- The biggest challange was the imbalance issue, SMOTEEN was the best approach.


### Conclusion
- The best performing model is GradientBoosting with the highest F1 score.
- Using SMOTEENN for resampling improved performance compared to using SMOTE alone.
- Encoding strategies and feature engineering did not significantly boost performance.
