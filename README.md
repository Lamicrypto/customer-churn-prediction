## 📊 Customer Churn Analysis and Prediction

An end-to-end data analysis and machine learning project that explores the factors associated with customer churn in a telecommunications company and develops classification models to identify customers who may be at risk of leaving.

The project combines data cleaning, exploratory data analysis (EDA), visualization, feature engineering, and machine learning to generate actionable insights that can support proactive customer retention strategies.

⸻

## 📌 Project Overview

Customer churn is a major challenge for subscription-based businesses. When customers leave, companies lose recurring revenue and often incur additional costs to acquire new customers.

This project analyzes telecommunications customer data to:

* Understand the key factors associated with customer churn.
* Identify customer groups with higher churn risk.
* Explore patterns in customer behavior and service usage.
* Build machine learning models to predict potential churners.
* Evaluate different classification thresholds and their impact on churn detection.
* Translate analytical findings into actionable business recommendations.

⸻

## 🎯 Business Problem

The primary business question is:

Can customer data be used to identify customers who are more likely to churn, allowing the company to take proactive retention actions?

The analysis focuses on customer characteristics such as:

* Contract type
* Customer tenure
* Internet service
* Payment method
* Monthly charges
* Customer demographics
* Additional services

Understanding these relationships can help businesses prioritize retention efforts and focus resources on customers with a higher likelihood of leaving.

⸻

## 📂 Dataset

The dataset contains telecommunications customer information, including:

* Customer demographics
* Contract type
* Tenure
* Internet service
* Payment method
* Monthly charges
* Additional services
* Churn status

The target variable is Churn, which indicates whether a customer left the company.

⸻

## 🛠️ Tools and Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook
* VS Code
* Git & GitHub

⸻

## 🔍 Exploratory Data Analysis

The exploratory analysis examined the relationship between customer churn and several customer characteristics, including:

* Contract type
* Tenure
* Monthly charges
* Internet service
* Payment method
* Senior citizen status

The analysis revealed several notable patterns that may help explain why certain customers are more likely to leave.

⸻

## 📊 Key Findings

1. Contract Type

Customers on month-to-month contracts had the highest churn rate:

Contract Type	Churn Rate
Month-to-month	42.71%
One year	11.27%
Two year	2.83%

Customers with longer-term contracts were significantly less likely to churn than customers on month-to-month contracts.

Business implication: Contract length appears to be strongly associated with customer retention.

⸻

2. Internet Service

Fiber optic customers recorded a relatively high churn rate:

Internet Service	Churn Rate
Fiber optic	41.89%
DSL	18.96%
No internet service	7.40%

The higher churn rate among fiber optic customers may warrant further investigation into pricing, service quality, customer expectations, or other factors.

⸻

3. Payment Method

Customers using electronic checks had the highest observed churn rate at approximately 45.29%.

This suggests that payment method may be associated with customer retention and deserves further investigation.

⸻

4. Senior Citizen Status

Senior citizens had a churn rate of approximately 41.68%, compared with 23.61% among non-senior customers.

This indicates that customer demographics may play a role in churn behavior and could be considered when designing targeted retention strategies.

⸻

5. Customer Tenure

Customers who churned had an average tenure of approximately 18 months, compared with approximately 38 months for customers who stayed.

This suggests that newer customers may be more vulnerable to churn, highlighting the importance of effective onboarding and early customer engagement.

⸻

6. Monthly Charges

Customers who churned had higher average monthly charges:

* Churned customers: approximately $74.44
* Retained customers: approximately $61.27

Higher monthly charges may be associated with increased churn risk, although this relationship may also be influenced by other factors such as contract type and service configuration.

⸻

## 🤖 Machine Learning

Two classification models were developed and evaluated:

1. Logistic Regression
2. Random Forest

Data Preparation

The dataset was divided into:

* 80% training data
* 20% testing data

Categorical variables were converted into numerical representations using one-hot encoding before model training.

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-score

Because the objective is to identify customers who may churn, recall is particularly important. A model that misses too many actual churners may reduce the effectiveness of a customer retention campaign.

⸻

## 📈 Model Performance

Logistic Regression — 50% Classification Threshold

* Accuracy: 80.70%
* Churn Precision: 66%
* Churn Recall: 56%
* Churn F1-score: 61%

Logistic Regression — 40% Classification Threshold

* Accuracy: 78.00%
* Churn Precision: 57%
* Churn Recall: 67%
* Churn F1-score: 61%

Random Forest

* Accuracy: 77.43%
* Churn Precision: 57%
* Churn Recall: 64%
* Churn F1-score: 60%

⸻

## ⚖️ Classification Threshold Analysis

The Logistic Regression model was evaluated using two different probability thresholds.

At the standard 50% threshold, the model achieved:

56% churn recall

When the threshold was reduced to 40%, churn recall increased to:

67% churn recall

This means the model was able to identify a larger proportion of customers who actually churned, although this came with a reduction in precision and overall accuracy.

For a customer retention campaign, the lower threshold may be preferable if the business is willing to contact more customers in exchange for identifying more potential churners.

This demonstrates an important machine learning principle:

The best classification threshold depends on the business objective and the relative cost of false positives and false negatives.

⸻

## 🏆 Model Selection

Based on the evaluation results, Logistic Regression provided the strongest overall performance among the tested models.

The model achieved the highest accuracy and precision at the 50% threshold, while lowering the threshold to 40% improved recall for the churn class.

The appropriate threshold would ultimately depend on the company’s retention strategy and the cost of missing a potential churner versus contacting a customer who would not have churned.

⸻

## 💡 Business Insights and Recommendations

1. Encourage Long-Term Contracts

The company could encourage month-to-month customers to move to one-year or two-year contracts through:

* Discounts
* Loyalty incentives
* Additional service benefits
* Contract upgrade offers

⸻

2. Focus on Early Customer Retention

Customers with shorter tenure showed higher churn tendencies.

The company could strengthen:

* New customer onboarding
* Early engagement campaigns
* Customer education
* First-year loyalty programs

⸻

3. Investigate Fiber Optic Churn

The relatively high churn rate among fiber optic customers should be investigated further.

Potential areas to explore include:

* Pricing
* Service quality
* Customer expectations
* Technical support
* Competitor offerings

⸻

4. Review Electronic Check Customers

The high churn rate among electronic-check customers may indicate potential billing or payment-related issues.

The company could investigate whether:

* Payment processes are creating friction.
* Customers using electronic checks have different demographic profiles.
* Payment method is associated with other churn-related factors.

⸻

5. Develop Targeted Retention Strategies

Customers identified as higher risk could receive targeted interventions such as:

* Personalized offers
* Loyalty incentives
* Customer support outreach
* Contract upgrade options
* Service improvement offers

⸻

6. Use Predictive Churn Modeling

The machine learning model can support proactive retention by identifying customers who are more likely to churn.

A business could use these predictions to prioritize retention campaigns and allocate customer service resources more efficiently.

⸻

## 📁 Project Structure

Customer-churn-prediction/
│
├── Images/
│   ├── customer_churn_distribution.png
│   ├── churn_rate_by_payment_method.png
│   ├── monthly_charges_by_churn.png
│   ├── tenure_distribution_by_churn.png
│   ├── churn_rate_by_senior_status.png
│   ├── logistic_regression_confusion_matrix.png
│   ├── model_comparison.png
│   └── top_churn_factors.png
│
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
├── churn_analysis.ipynb
├── README.md
└── requirements.txt

⸻

## ▶️ How to Run the Project

1. Clone the repository

git clone https://github.com/Lamicrypto/Customer-churn-prediction.git

2. Navigate to the project directory

cd Customer-churn-prediction

3. Install the required dependencies

pip install -r requirements.txt

4. Open the Jupyter Notebook

Open:

churn_analysis.ipynb

Run the notebook cells sequentially to reproduce the analysis and model results.

⸻

## 🏁 Conclusion

This project demonstrates an end-to-end approach to customer churn analysis, combining data preparation, exploratory analysis, visualization, machine learning, and business interpretation.

The analysis identified several factors associated with customer churn, including:

* Contract type
* Customer tenure
* Internet service
* Payment method
* Monthly charges

The machine learning analysis also demonstrated the importance of selecting an appropriate classification threshold based on business objectives.

Overall, the project highlights how data analysis and predictive modeling can support proactive customer retention by helping businesses identify customers who may be at higher risk of leaving.

⸻

## 👤 Author

Timothy Olamide Balogun

AI & Machine Learning | Data Analysis | Python | SQL

📧 Email: olapyperfx24@gmail.com

🔗 GitHub: https://github.com/Lamicrypto

💼 LinkedIn: https://www.linkedin.com/in/timothy-balogun-0a27192a2