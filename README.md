# Telecom Customer Churn Prediction

## 🎯 Objective
The goal of this project is to predict whether a customer will churn (leave the service) based on their demographic, account, and service usage data.  

We used the **Telco Customer Churn dataset** from Kaggle for this task.  

---

## 🛠 Tools & Libraries
- **Python**
- **Pandas, NumPy** → Data preprocessing & handling missing values  
- **Matplotlib, Seaborn** → Data visualization  
- **Scikit-learn** → Machine learning (Logistic Regression, Random Forest, scaling, encoding)  
- **Joblib** → Save trained models for deployment  

---

## 📌 Steps Performed
1. **Data Loading & Cleaning**
   - Loaded dataset into Pandas
   - Removed unnecessary `customerID`
   - Converted `TotalCharges` to numeric and filled missing values  

2. **Encoding & Feature Engineering**
   - Used **LabelEncoder** for binary categorical features (e.g., Yes/No)  
   - Used **OneHotEncoding** for multi-class categorical variables (e.g., Contract type)  
   - Applied **StandardScaler** for numerical features  

3. **Model Training**
   - **Logistic Regression** → Simple baseline model  
   - **Random Forest Classifier** → More robust and better performing model  

4. **Evaluation**
   - Evaluated models using **Accuracy, Precision, Recall, F1-score**  
   - Compared Logistic Regression and Random Forest performance  

5. **Feature Importance**
   - Extracted feature importance from Random Forest  
   - Visualized top 10 most important features  

6. **Model Saving**
   - Saved trained Random Forest model as `churn_model.pkl` using joblib  

---

## 📊 Results
- Logistic Regression achieved ~80% accuracy  
- Random Forest achieved ~85%+ accuracy  
- Most important features affecting churn:
  - **Contract type**  
  - **Tenure (months with the company)**  
  - **MonthlyCharges**  
  - **TotalCharges**  
  - **InternetService**  

---

## 🚀 Deliverables
- **Google Colab Notebook (`Task_4_DA.ipynb`)** → Full implementation  
- **Saved Model (`churn_model.pkl`)** → Can be loaded later for deployment  
- **README.md** (this file) → Explanation of the project  

---
