# 🧠 Customer Churn Prediction Using Artificial Neural Networks

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat-square&logo=python)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=flat-square&logo=tensorflow)](https://www.tensorflow.org/)
[![Keras](https://img.shields.io/badge/Keras-2.x-red?style=flat-square&logo=keras)](https://keras.io/)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)]()

**A Deep Learning Solution for Predicting Banking Customer Churn**

[Features](#features) • [Quick Start](#quick-start) • [Results](#results) • [Technologies](#technologies) • [Future Work](#future-work)

</div>

---

## 📋 Overview

This project implements a sophisticated **Artificial Neural Network (ANN)** using TensorFlow/Keras to predict customer churn in the banking sector. Customer churn—the loss of customers discontinuing their bank services—represents a critical business challenge that significantly impacts profitability and organizational growth.

By leveraging historical customer data and demographic information, this model classifies whether customers are likely to exit the bank, enabling proactive retention strategies.

---

## 🎯 Problem Statement

**Challenge:** Customer retention is a critical challenge for banks and financial institutions. Losing customers can significantly impact profitability and growth trajectory.

**Solution:** Build a machine learning model capable of predicting customer churn based on historical customer data, enabling targeted intervention strategies.

---

## 📊 Dataset Features

The model utilizes 11 customer attributes to make predictions:

| Feature | Description |
|---------|-------------|
| **Credit Score** | Customer's credit rating |
| **Geography** | Customer's location (encoded) |
| **Gender** | Customer's gender |
| **Age** | Customer's age in years |
| **Tenure** | Years as a customer |
| **Account Balance** | Current account balance |
| **Number of Products** | Banking products held |
| **Credit Card Ownership** | Whether customer holds a credit card |
| **Active Member Status** | Current account activity status |
| **Estimated Salary** | Annual salary estimate |

**Target Variable:**
- **Exited** (1 = Customer Left, 0 = Customer Stayed)

---

## 🔧 Methodology

### 1️⃣ Data Preprocessing
- ✓ Comprehensive data cleaning and inspection
- ✓ Categorical variable encoding (Label Encoder & One-Hot Encoding)
- ✓ Feature scaling using standardization (StandardScaler)
- ✓ Train-test split (80-20 ratio)

### 2️⃣ Model Architecture

The ANN consists of:

```
Input Layer (11 features)
    ↓
Dense Layer (64 units, ReLU activation) + Dropout
    ↓
Dense Layer (32 units, ReLU activation) + Dropout
    ↓
Output Layer (1 unit, Sigmoid activation)
```

**Training Configuration:**
- **Loss Function:** Binary Cross-Entropy
- **Optimizer:** Adam (learning rate: 0.001)
- **Batch Size:** 32
- **Epochs:** 100
- **Validation Split:** 20%

### 3️⃣ Model Evaluation

The model's performance was assessed using:
- ✓ **Accuracy Score** - Overall correctness
- ✓ Additional metrics available in `Future Improvements`

---

## 🚀 Quick Start

### Prerequisites
```bash
pip install tensorflow keras numpy pandas scikit-learn
```

### Running the Model
```python
# Data loading and preprocessing
import pandas as pd
from sklearn.preprocessing import StandardScaler, LabelEncoder

# Load dataset
data = pd.read_csv('your_data.csv')

# Preprocess data
# ... (see main notebook for full pipeline)

# Build and train ANN
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense, Dropout

model = Sequential([
    Dense(64, activation='relu', input_dim=11),
    Dropout(0.2),
    Dense(32, activation='relu'),
    Dropout(0.2),
    Dense(1, activation='sigmoid')
])

model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])
model.fit(X_train, y_train, epochs=100, batch_size=32, validation_split=0.2)
```

---

## 📈 Results

### Model Performance

| Metric | Value |
|--------|-------|
| **Accuracy Score** | **86%** ✨ |
| **Dataset** | Banking customer churn data |
| **Model Type** | Binary Classification (Deep Learning) |

**Key Insight:** The model successfully learns patterns from customer data and generates reliable churn predictions on unseen test data.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|-----------|---------|
| **Python** | Programming language |
| **TensorFlow** | Deep learning framework |
| **Keras** | Neural network API |
| **NumPy** | Numerical computations |
| **Pandas** | Data manipulation & analysis |
| **Scikit-Learn** | Data preprocessing & metrics |

---

## 💡 Key Skills Demonstrated

✅ Machine Learning & Deep Learning  
✅ Artificial Neural Networks Architecture  
✅ Data Preprocessing & Feature Engineering  
✅ Classification Modeling  
✅ Model Evaluation & Validation  
✅ Python Programming  
✅ Financial Data Analytics  
✅ TensorFlow/Keras Implementation  

---

## 🔮 Future Improvements

- 📊 Hyperparameter tuning (grid search, random search)
- 🔄 K-Fold Cross-validation for robust evaluation
- 📉 Precision, Recall, and F1-Score metrics
- 📈 ROC-AUC curve analysis
- 🔍 Model explainability using SHAP values
- 🤖 Comparison with alternative algorithms:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting (XGBoost)
  - Light GBM
- 📱 Model deployment as REST API
- 📊 Feature importance analysis
- ⚖️ Class imbalance handling (SMOTE, class weights)

---

## 📁 Project Structure

```
├── README.md
├── notebook/
│   └── ANN_Churn_Prediction.ipynb
├── data/
│   └── churn_data.csv
├── models/
│   └── trained_model.h5
└── requirements.txt
```

---

## 🎓 Author

**Neo Mohlomi**

📚 **Background:** MSc in Astrophysics | Data Analytics | Machine Learning | Artificial Intelligence

🔗 **LinkedIn:** [neo-mohlomi-07a28a313](https://www.linkedin.com/in/neo-mohlomi-07a28a313)  
🐙 **GitHub:** [neo-mohlomi](https://github.com/neo-mohlomi)

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

<div align="center">

⭐ If you found this helpful, please consider giving it a star!

[↑ Back to Top](#-customer-churn-prediction-using-artificial-neural-networks)

</div>