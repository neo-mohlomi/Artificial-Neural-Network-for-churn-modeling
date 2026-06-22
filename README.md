# Customer Churn Prediction Using Artificial Neural Networks
##Overview
In this  project I implements an Artificial Neural Network (ANN) to predict customer churn in the banking sector. Customer churn refers to the loss of customers who discontinue using a bank's services. Accurately identifying customers who are likely to leave allows financial institutions to implement targeted retention strategies and improve customer satisfaction.

I used  customer demographic and financial information and trained to classify whether a customer is likely to exit the bank to build tis model.

## Problem Statement

Customer retention is a critical challenge for banks and financial institutions. Losing customers can significantly impact profitability and growth.

My objective is to build a machine learning model capable of predicting customer churn based on historical customer data.

## Dataset Features

I used several customer attributes, including:

* Credit Score
* Geography
* Gender
* Age
* Tenure
* Account Balance
* Number of Products
* Credit Card Ownership
* Active Member Status
* Estimated Salary

Target Variable:

* Exited (1 = Customer Left, 0 = Customer Stayed)


## Methodology

### Data Preprocessing

* Data cleaning and inspection
* Handling categorical variables using Label encoder and One Hot Encoder
* Feature scaling using standardization
* Splitting the dataset into training and testing sets

### Model Development

I built an Artificial Neural Network using TensorFlow/Keras consisting of:

* Input Layer
* Hidden Layer with ReLU activation
* Output Layer with Sigmoid activation

I trained the model using:

* Binary Cross-Entropy Loss Function
* Adam Optimizer

### Model Evaluation

I evaluated the model's performance using accuracy score:

* Accuracy Score

The trained model was tested on unseen data to assess its ability to generalize to new customer records.


## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Pandas
* Scikit-Learn
  

## Results

The Artificial Neural Network successfully learned patterns from customer data and generated churn predictions on the test dataset.

Performance Metric:

* Accuracy: 86%

## Future Improvements

* Hyperparameter tuning
* Cross-validation
* Precision, Recall, and F1-Score evaluation
* ROC-AUC analysis
* Model explainability using SHAP values
* Comparison with Logistic Regression, Random Forest, and XGBoost models

---

## Key Skills Demonstrated

* Machine Learning
* Deep Learning
* Artificial Neural Networks
* Data Preprocessing
* Feature Engineering
* Classification Modelling
* Model Evaluation
* Python Programming
* Financial Data Analytics

---

## Author

Neo Mohlomi

Msc in Astrophysics | Data Analytics | Machine Learning | Artificial Intelligence

LinkedIn: www.linkedin.com/in/neo-mohlomi-07a28a313

