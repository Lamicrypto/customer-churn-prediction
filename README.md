# Customer Churn Analysis and Prediction

## 📌 Project Overview

This project analyzes customer churn data from a telecommunications company to identify the key factors associated with customer attrition and develop machine learning models capable of predicting customers who are at risk of churning.

The project combines exploratory data analysis (EDA), data visualization, and machine learning to generate actionable business insights that can help improve customer retention.

---

## 🎯 Business Problem

Customer churn is a major challenge for subscription-based businesses. Losing customers can reduce revenue and increase the cost of acquiring new customers.

The objective of this project is to:

* Understand the factors associated with customer churn.
* Identify customer segments with higher churn risk.
* Build a machine learning model to predict potential churners.
* Provide actionable recommendations to improve customer retention.

---

## 📂 Dataset

The dataset contains information about telecommunications customers, including:

* Customer demographics
* Contract type
* Tenure
* Internet service
* Payment method
* Monthly charges
* Additional services
* Churn status

The target variable is **Churn**, which indicates whether a customer left the company.

---

## 🛠️ Tools and Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook
* VS Code
* GitHub

---

## 🔍 Exploratory Data Analysis

The exploratory analysis examined relationships between customer churn and several variables, including:

* Contract type
* Tenure
* Monthly charges
* Internet service
* Payment method
* Senior citizen status

Several important patterns were identified.

---

## 📊 Key Findings

### Contract Type

Month-to-month customers had the highest churn rate at approximately **42.71%**, compared with **11.27%** for one-year contracts and **2.83%** for two-year contracts.

### Internet Service

Fiber optic customers had a churn rate of approximately **41.89%**, compared with **18.96%** for DSL customers and **7.40%** for customers without internet service.

### Payment Method

Customers using electronic checks had the highest churn rate at approximately **45.29%**.

### Senior Citizens

Senior citizens had a churn rate of approximately **41.68%**, compared with **23.61%** among non-senior customers.

### Customer Tenure

Customers who churned had an average tenure of approximately **18 months**, compared with approximately **38 months** for customers who stayed.

### Monthly Charges

Customers who churned had higher average monthly charges of approximately **$74.44**, compared with **$61.27** for customers who stayed.

---

## 🤖 Machine Learning

Two classification models were developed and evaluated:

1. Logistic Regression
2. Random Forest

The data was divided into:

* **80% training data**
* **20% testing data**

Categorical variables were converted into numerical features using one-hot encoding.

---

## 📈 Model Performance

### Logistic Regression — 50% Threshold

* Accuracy: **80.70%**
* Churn Precision: **66%**
* Churn Recall: **56%**
* Churn F1-score: **61%**

### Logistic Regression — 40% Threshold

* Accuracy: **78.00%**
* Churn Precision: **57%**
* Churn Recall: **67%**
* Churn F1-score: **61%**

### Random Forest

* Accuracy: **77.43%**
* Churn Precision: **57%**
* Churn Recall: **64%**
* Churn F1-score: **60%**

The Logistic Regression model performed best overall in terms of accuracy and precision. However, lowering the classification threshold to 40% increased churn recall from **56% to 67%**, allowing the model to identify more customers who were actually at risk of churning.

---

## 💡 Business Insights and Recommendations

### 1. Encourage Long-Term Contracts

The company should encourage month-to-month customers to move to one-year or two-year contracts through discounts, incentives, or additional benefits.

### 2. Focus on Early Customer Retention

Customers with shorter tenure are more likely to churn. The company should strengthen onboarding and engagement during the early stages of the customer relationship.

### 3. Investigate Fiber Optic Churn

The high churn rate among fiber optic customers should be investigated to determine whether pricing, service quality, or customer expectations contribute to the problem.

### 4. Review Electronic Check Customers

The company should investigate why electronic-check customers have significantly higher churn rates and determine whether billing or payment-related issues contribute to customer attrition.

### 5. Support High-Risk Customer Segments

Targeted retention strategies should be developed for high-risk groups, including senior citizens and customers with higher monthly charges.

### 6. Use Predictive Churn Modeling

The machine learning model can be used to identify customers who are at increased risk of leaving, allowing the company to intervene before churn occurs.

---

## 📁 Project Structure

```text
telco-customer-churn-analysis/
│
├── data/
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── images/
│   ├── customer_churn_distribution.png
│   ├── churn_rate_by_payment_method.png
│   ├── monthly_charges_by_churn.png
│   ├── tenure_distribution_by_churn.png
│   ├── churn_rate_by_senior_status.png
│   ├── logistic_regression_confusion_matrix.png
│   ├── model_comparison.png
│   └── top_churn_factors.png
│
├── churn_analysis.ipynb
├── README.md
└── requirements.txt
```

---

## 🏁 Conclusion

This project demonstrates an end-to-end approach to customer churn analysis, from data cleaning and exploratory analysis to machine learning and business recommendations.

The analysis shows that factors such as contract type, tenure, internet service, payment method, and monthly charges are strongly associated with customer churn.

The final analysis demonstrates how machine learning can support proactive customer retention by identifying customers who may be at higher risk of leaving.

---

## 👤 Author

**Timothy Olamide Balogun**

Data Analytics | Machine Learning | Python | AI
