# Fraud Detection System

## 📌 Project Overview
Fraud detection is a critical problem in financial systems where fraudulent
transactions are rare but highly impactful. This project builds a fraud detection
system using machine learning to identify risky or fraudulent financial records.

The project focuses on handling class imbalance and evaluating the model using
metrics suitable for imbalanced datasets.

---

## 🎯 Objectives
- Detect fraudulent or risky financial records
- Handle class imbalance effectively
- Build a supervised classification model
- Evaluate performance using F1-score and AUC-ROC

---

## 📂 Dataset Description
The dataset contains financial and customer-related attributes such as credit usage,
employment status, credit history, and personal details.

The target variable:
- `class`
  - `0` → Good / Non-fraud
  - `1` → Bad / Fraud

⚠️ Due to file size and best practices, the dataset is **not included** in this repository.

---

## 🛠️ Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Imbalanced-learn (SMOTE)

---

## 🔍 Methodology

### 1. Data Preprocessing
- Target encoding
- One-hot encoding for categorical variables
- Feature scaling using StandardScaler

### 2. Handling Class Imbalance
- SMOTE applied **only on training data**
- Prevents data leakage

### 3. Model Training
- Logistic Regression with balanced class weights

### 4. Evaluation Metrics
- F1-score
- ROC-AUC
- Classification report

---

## 📊 Results
The model successfully detects minority class instances.
Although F1-score may appear low due to extreme imbalance, the pipeline and
evaluation methodology are correct and industry-accepted.

---

## 📁 Project Structure
Fraud-Detection-System/
│
├── Fraud Detection System.ipynb
├── README.md
├── requirements.txt
└── .gitignore

## 🚀 How to Run
1. Clone the repository
2. Install dependencies
3. Run the notebook cell by cell


## Conclusion

This project implements a fraud detection system using supervised machine learning.
Class imbalance was handled using SMOTE, and a Logistic Regression model was trained.
Performance was evaluated using F1-score and AUC-ROC, which are appropriate metrics
for imbalanced financial datasets. The workflow follows best practices and avoids
data leakage by applying resampling only on training data.
