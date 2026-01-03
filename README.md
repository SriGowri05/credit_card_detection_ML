# 💳 Credit Card Fraud Detection using Machine Learning

## 📌 Project Overview
This project detects **fraudulent credit card transactions** using **machine learning**.  
Since fraud cases are very rare, the dataset is **highly imbalanced**, and techniques like **SMOTE** are used to improve detection performance.

The model is implemented and tested using **Google Colab**.

---

## 📂 Dataset
- Files used:
  - `fraudTrain.csv`
  - `fraudTest.csv`
- Target column:
  - `is_fraud`
    - `0` → Normal transaction  
    - `1` → Fraud transaction

---

## 🛠 Tools & Technologies
- Python
- Google Colab
- Pandas
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Random Forest Classifier

---

## DataSet
- kaggle:https://www.kaggle.com/code/youssefelbadry10/credit-card-fraud-detection/input

---

## ⚙️ Steps Performed

### 1. Data Loading
- Dataset is uploaded to Google Colab
- Files are extracted and read from `/mnt/data/`

### 2. Data Preprocessing
- Target variable (`is_fraud`) is separated
- Non-numeric columns are removed
- Dataset is prepared for model training

### 3. Handling Imbalanced Data
- **SMOTE (Synthetic Minority Oversampling Technique)** is applied
- Balances fraud and non-fraud transactions

### 4. Model Training
- **Random Forest Classifier** is used
- Dataset is split into training and testing sets

### 5. Model Evaluation
- Confusion Matrix
- Precision, Recall, F1-score
- Recall is prioritized to detect maximum fraud cases

---

## 🧪 Manual Testing

### Test using a single transaction
```python
sample = X_test.iloc[0:1]
model.predict(sample)
```
---

## Author
Srigowri Cheboyina


