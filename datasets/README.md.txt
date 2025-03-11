# 📉 Customer Churn Prediction in Telecom
### 🔍 Identifying At-Risk Customers with AI

🚀 **Goal:** Predict whether a telecom customer is likely to churn using **Machine Learning**.

---
## 📂 Project Structure

Customer-Churn-Prediction/
│── customer_churn_prediction.Rmd  # Full R Markdown Notebook
│── customer_churn_prediction.html  # Rendered HTML Report
│── dataset/telecom_churn.csv  # Dataset (if available)
│── scripts/model_training.R  # Cleaned version of the R script
│── visualization/churn_analysis.png  # Key plots for presentations

---
## 📊 Dataset Overview
- **Columns:** Monthly Charges, Tenure, Contract Type, Churn (Target Variable)
- **Rows:** 7,000+ telecom customers
- **Source:** [Insert dataset link if public]

---
## 🏆 Key Findings
✅ **Customers with higher monthly charges** have a **greater likelihood of churning**  
✅ **Longer contract customers** tend to be more **loyal**  
✅ **ROC-AUC Score:** `0.85` (**Good predictive power**)  

---
## 🧑‍💻 How to Run This Project?
### 1️⃣ Install dependencies
```r
install.packages("caTools")
install.packages("ggplot2")
install.packages("pROC")


rmarkdown::render("customer_churn_prediction.Rmd")
