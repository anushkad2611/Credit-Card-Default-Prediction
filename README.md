Credit Card Default Prediction

This machine learning project aims to predict whether a credit card customer is likely to default on their payment in the upcoming month.

The project encompasses various stages, including Exploratory Data Analysis (EDA), data preprocessing, feature engineering, handling class imbalance, model training, and evaluation.

Objective

The primary objective is to identify patterns in customer demographics, credit utilization, billing amounts, and repayment behavior that can aid in predicting credit card payment defaults.

Exploratory Data Analysis

The EDA delves into various aspects of the dataset, including:

* - Customer demographics and age distribution
* - Credit limits
* - Billing and payment amounts
* - Repayment history
* - Default distribution
* - Correlations between variables
* - Credit utilization and payment behavior
* 
After preprocessing, the dataset comprises over 25,000 customer records, with approximately 19% of customers classified as defaulters.

Feature Engineering

Several behavioral features were meticulously crafted to capture customer risk, such as:

* - Credit Utilization Ratio
* - Delayed Payment Count
* - Recent Overdue Count
* - Maximum Payment Delay
* - Payment-to-Bill Ratio
* - Payment Volatility
* - Delinquency Streak
* 
Handling Class Imbalance

Since default cases constitute a minority of the dataset, SMOTETomek was employed on the training data to enhance the model’s ability to learn from the minority class.

Machine Learning Models

The project evaluates a diverse range of classification algorithms, including:

* - Logistic Regression
* - Random Forest
* - XGBoost
* - LightGBM
* 
These models are assessed using various evaluation metrics, including:

* - AUC-ROC
* - Accuracy
* - Precision
* - Recall
F1 Score, F2 Score, and Confusion Matrix are key metrics used to evaluate the performance of a classification model. By analyzing different classification thresholds, we can understand the trade-off between precision, recall, F1 score, F2 score, and accuracy. The analysis revealed that optimizing for F2 score can enhance recall-oriented performance but may significantly decrease overall accuracy. Therefore, the 0.5 threshold was chosen as a practical balance.

The project structure is organized as follows:

- Credit-Card-Default-Prediction/
  │
  ├── Credit_Card_EDA.ipynb
  ├── Credit_Card_Model.ipynb
  ├── README.md
  └── credit_default_predictions.csv

* The technologies used in this project include Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Imbalanced-learn, XGBoost, and LightGBM.
* 
