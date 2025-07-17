# Churn-Modeling
# 🔍 Bank Customer Churn Prediction

This project focuses on predicting which customers are likely to leave a bank using a supervised machine learning classification model.

---

## 📌 Objective
To build a model that identifies customers who are likely to churn (i.e., leave the bank), using various customer attributes.

---

## 🧾 Dataset
**Churn_Modelling.csv**  
You can download it from Kaggle:  
[Customer Churn Prediction Dataset](https://www.kaggle.com/datasets/shubhendra7/customer-churn-prediction)

### 🔑 Key Columns:
- `CreditScore`
- `Geography`
- `Gender`
- `Age`
- `Tenure`
- `Balance`
- `NumOfProducts`
- `HasCrCard`
- `IsActiveMember`
- `EstimatedSalary`
- `Exited` *(Target: 1 = Churned, 0 = Stayed)*

---

## 🛠️ Steps Followed

### 1. Data Cleaning
- Dropped irrelevant columns: `RowNumber`, `CustomerId`, `Surname`.

### 2. Encoding Categorical Variables
- `Gender` encoded using Label Encoding.
- `Geography` encoded using One-Hot Encoding.

### 3. Feature Scaling
- Applied StandardScaler to normalize features.

### 4. Model Training
- Trained a **Random Forest Classifier** on the data.
- Used `train_test_split` for a proper evaluation split.

### 5. Evaluation Metrics
- Confusion Matrix
- Classification Report (Accuracy, Precision, Recall, F1-Score)

### 6. Feature Importance
- Plotted feature importances to understand key drivers of churn.

---

## 📊 Results
- Identified top churn influencers: `Age`, `Balance`, `IsActiveMember`, `Geography_Germany`, etc.
- Achieved a balanced classification model using Random Forest.

---

## 💻 Libraries Used
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `sklearn` (for preprocessing and modeling)

---

## 🧠 Future Work
- Try other models like XGBoost, SVM, or Logistic Regression.
- Use GridSearchCV for hyperparameter tuning.
- Handle class imbalance using SMOTE or other techniques.

---

## 📁 Folder Structure

