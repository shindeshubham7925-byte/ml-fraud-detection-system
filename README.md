# 💳 Online Payment Fraud Detection using Machine Learning in Python

## 📌 Overview
With the increasing trend of online payments, fraud detection has become a crucial aspect of financial security.  
This project implements multiple **Machine Learning models** to detect fraudulent transactions in online payments using Python.  
The solution analyzes transaction patterns, identifies anomalies, and classifies transactions as fraudulent or legitimate.

---

## ✨ Features
- Data preprocessing & feature engineering
- Exploratory Data Analysis (EDA) with **Seaborn** & **Matplotlib**
- Comparison of multiple classification algorithms:
  - Logistic Regression
  - XGBoost Classifier
  - Random Forest Classifier
- Model evaluation using **ROC-AUC Score** & **Confusion Matrix**
- Highly accurate fraud detection (Best: **XGBoost**)

---

## 📂 Dataset
The dataset contains transaction details such as:
| Feature           | Description |
|-------------------|-------------|
| `step`            | Time step (unit of time) |
| `type`            | Type of transaction (cash_out, transfer, etc.) |
| `amount`          | Transaction amount |
| `nameOrig`        | Sender account ID |
| `oldbalanceOrg`   | Sender's balance before transaction |
| `newbalanceOrg`   | Sender's balance after transaction |
| `nameDest`        | Receiver account ID |
| `oldbalanceDest`  | Receiver's balance before transaction |
| `newbalanceDest`  | Receiver's balance after transaction |
| `isFraud`         | Target variable (1 = Fraud, 0 = Legitimate) |

---

## 🛠️ Tech Stack
- **Python 3**
- **Libraries**:
  - Pandas, NumPy
  - Matplotlib, Seaborn
  - Scikit-learn
  - XGBoost

---

## 📊 Exploratory Data Analysis (EDA)
- Transaction type distribution
- Fraud vs Non-Fraud comparison
- Correlation heatmap
- Transaction amount analysis

---

## 🔍 Data Preprocessing
- Encoding categorical variables (`type`)
- Dropping irrelevant columns (`nameOrig`, `nameDest`)
- Splitting dataset into **training** and **testing** sets

---

## 🤖 Model Training & Accuracy
| Model                  | Training ROC-AUC | Validation ROC-AUC |
|------------------------|------------------|--------------------|
| Logistic Regression    | 0.8873           | 0.8849             |
| XGBoost Classifier     | **0.99997**      | **0.99921**        |
| Random Forest (n=7)    | 0.99999          | 0.9650             |

**Best Model:** `XGBoost Classifier`

---

## 📈 Confusion Matrix (XGBoost)
![Confusion Matrix](docs/confusion_matrix.png)

---

