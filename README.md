#🏥 Health Insurance Cross-Sell Prediction using Machine Learning
📌 Project Overview
Health insurance companies aim to increase revenue by cross-selling insurance products to existing customers. This machine learning (ML) project predicts whether a customer is likely to purchase additional coverage, enabling smarter marketing strategies.

The dataset contains 381,109 entries with features like:

id, Gender, Age, Driving_License, Region_Code, Previously_Insured, Vehicle_Age, Vehicle_Damage, Annual_Premium, Policy_Sales_Channel, Vintage, and Response.

🧹 Data Preparation
✅ Cleaning
No missing values.

Ensured correct data types and consistent formatting.

🔄 Encoding
Binary Encoding: Gender (Male=1, Female=0), Vehicle_Damage (Yes=1, No=0)

Ordinal Encoding: Vehicle_Age (<1 Year=0, 1–2 Year=1, >2 Years=2)

📊 Normalization
Scaled Age, Annual_Premium, and Vintage to improve model performance.

🏗️ Feature Engineering
Combined Region_Code and Policy_Sales_Channel to capture regional sales trends.

📈 Exploratory Data Analysis (EDA)
Descriptive Statistics: Summary of distributions.

Visualizations: Histograms, box plots, and bar charts for insights and outlier detection.

Correlation Matrix: Heatmaps to identify redundant features.

🤖 Model Development
🔍 Feature Selection
Selected based on EDA insights for better model performance.

🛠️ Algorithms Used
Logistic Regression

Decision Tree

Random Forest

Gradient Boosting (GBM)

XGBoost

Neural Networks

🧪 Training & Tuning
Used train-validation split.

Applied Random Search for hyperparameter tuning.

📊 Model Evaluation
Key metrics used:

Accuracy

Precision & Recall

F1 Score

ROC-AUC

🏆 XGBoost performed best, showing higher testing accuracy than training accuracy, indicating strong generalization to unseen data.

🚀 Deployment & Monitoring
Integration: Ready for production integration.

Monitoring: Continuous performance tracking.

Updating: Retrain periodically with fresh data to maintain accuracy.

✅ Conclusion
This project demonstrates how ML can boost cross-sell strategies in health insurance by identifying likely buyers of additional products. With proper data preparation, strong modeling, and XGBoost’s excellent generalization, the solution offers both business value and scalability.

