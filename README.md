# 📌 Customer Churn Prediction using Machine Learning

## 🚀 Project Overview
Customer churn is a major issue in industries like **telecommunications, banking, and SaaS (Software as a Service)**. This project aims to **predict customer churn** using machine learning, enabling businesses to take proactive actions to retain customers.

By analyzing customer demographics, service usage, billing details, and contract types, this model provides **actionable insights** to help reduce churn and improve **customer lifetime value (CLV)**.

---

## 🎯 Real-Life Business Problems Solved

### ✅ 1. Preventing Revenue Loss
Companies lose billions annually due to **customer attrition**. This project helps businesses:
- **Predict churn early** and take preventive measures.
- **Prioritize high-value customers** at risk of leaving.
- **Optimize retention strategies** to improve customer loyalty.

### ✅ 2. Reducing Customer Acquisition Costs
It is **5x more expensive** to acquire new customers than to retain existing ones. With churn prediction, businesses can:
- **Identify reasons for customer loss** and address service issues.
- **Offer personalized discounts** to retain customers.
- **Improve customer experience**, reducing costly acquisition efforts.

### ✅ 3. Enhancing Customer Support & Service Quality
By analyzing churn trends, companies can:
- **Identify service-related issues** causing dissatisfaction.
- **Enhance customer support responsiveness** for at-risk customers.
- **Improve contract offerings** to better fit customer needs.

### ✅ 4. Smart Marketing & Personalized Offers
- **Target customers with customized promotions** (e.g., special deals, premium services).
- **Optimize pricing strategies** based on customer segmentation.
- **Improve marketing ROI** by focusing on at-risk customers.

---

## 📂 Dataset Information
The dataset used is **Telco Customer Churn Dataset**, containing customer details from a telecom provider.

- **Dataset Name:** `WA_Fn-UseC_-Telco-Customer-Churn.csv`
- **Total Rows:** 7043
- **Total Columns:** 21
- **Target Variable:** `"Churn"` (Yes/No)
- **Missing Values:** None (but `TotalCharges` had blank values)

### 📊 Key Features
| Feature Name         | Description |
|----------------------|-------------|
| `gender` | Male / Female |
| `SeniorCitizen` | 1 = Senior Citizen, 0 = Not a Senior Citizen |
| `Partner` | Customer has a partner (Yes/No) |
| `Dependents` | Customer has dependents (Yes/No) |
| `tenure` | Number of months a customer has stayed |
| `PhoneService` | Whether customer has phone service (Yes/No) |
| `InternetService` | DSL / Fiber Optic / No Internet |
| `Contract` | Type of contract (Month-to-month, One year, Two year) |
| `PaymentMethod` | Payment method (Electronic check, Bank transfer, etc.) |
| `MonthlyCharges` | Monthly amount charged to customer |
| `TotalCharges` | Total amount charged to customer |

---

## 🛠️ Machine Learning Approach
This project follows a structured machine learning pipeline:

### 1️⃣ Data Preprocessing
✔ **Handled missing values** in `TotalCharges`.  
✔ **Converted categorical variables** using Label Encoding.  
✔ **Balanced the dataset** using SMOTE (Synthetic Minority Over-sampling Technique).  

### 2️⃣ Exploratory Data Analysis (EDA)
✔ **Histograms & Boxplots** to analyze feature distributions.  
✔ **Correlation Heatmap** to identify feature relationships.  
✔ **Count Plots** for categorical features.  

### 3️⃣ Model Training & Hyperparameter Tuning
We trained and compared multiple models, ultimately selecting **Random Forest** due to its superior performance.

**Models Tested:**
- **Decision Tree Classifier**
- **Random Forest Classifier** ✅ *(Best Performing Model)*

✅ **Hyperparameter tuning** using **GridSearchCV**.  
✅ **Final Model:** **Random Forest**
   - **Test Accuracy:** 77.86%
   - **Recall (Churn Detection):** 64%

---

## 🚀 Deployment & Usage

### 📌 Running the Project
1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/customer-churn-prediction.git
   cd customer-churn-prediction
