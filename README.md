# 🏥 Health Insurance Cross-Sell Prediction using Machine Learning

## 📌 Project Overview

Health insurance companies aim to increase revenue by **cross-selling** insurance products to existing customers. This machine learning (ML) project predicts whether a customer is likely to purchase additional coverage, enabling smarter marketing strategies.

The dataset contains 381,109 entries with features like:

`id`, `Gender`, `Age`, `Driving_License`, `Region_Code`, `Previously_Insured`, `Vehicle_Age`, `Vehicle_Damage`, `Annual_Premium`, `Policy_Sales_Channel`, `Vintage`, `Response`

---

## 🧹 Data Preparation

### ✅ Cleaning
- No missing values
- Verified data types and consistency

### 🔄 Encoding
- **Binary Encoding**: 
  - `Gender`: Male = 1, Female = 0  
  - `Vehicle_Damage`: Yes = 1, No = 0
- **Ordinal Encoding**: 
  - `Vehicle_Age`: `< 1 Year` = 0, `1-2 Year` = 1, `> 2 Years` = 2

### 📊 Normalization
- Scaled numerical features: `Age`, `Annual_Premium`, `Vintage`

### 🏗️ Feature Engineering
- Created interaction features (e.g., `Region_Code` + `Policy_Sales_Channel`) to capture regional sales trends

---

## 📈 Exploratory Data Analysis (EDA)

- **Descriptive Statistics**: Central tendencies and spread
- **Visualizations**: Histograms, bar charts, box plots for pattern discovery and outlier detection
- **Correlation Matrix**: Heatmaps to identify redundant or highly correlated variables

---

## 🤖 Model Development

### 🔍 Feature Selection
- Based on EDA findings to reduce dimensionality and noise

### 🛠️ Algorithms Tried
- Logistic Regression  
- Decision Tree  
- Random Forest    
- XGBoost  


### 🧪 Training & Tuning
- Used train-validation split for model evaluation
- Applied **Random Search** for hyperparameter tuning

---

## 📊 Model Evaluation

Evaluation metrics used:
- **Accuracy**
- **Precision** & **Recall**
- **F1 Score**
- **ROC-AUC**

> 🏆 **XGBoost** outperformed other models with the highest testing accuracy and better generalization. The difference between training and testing performance was positive and significant—indicating reliability on unseen data.

---

## 🚀 Deployment & Monitoring

- **Integration**: Ready to integrate into production systems
- **Monitoring**: Ongoing evaluation using live data
- **Updating**: Retrain with updated data periodically to preserve model relevance

---

## ✅ Conclusion

This project showcases the power of ML in boosting cross-sell strategies for the health insurance sector. With structured data processing, careful model selection, and XGBoost's superior performance, insurers can expect better targeting, increased sales, and improved customer satisfaction.

---
