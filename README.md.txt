# Customer Churn Prediction System

## 📌 Project Overview
This project predicts whether a customer is likely to churn (leave the service) using machine learning techniques.  
The goal is to help businesses identify high-risk customers and take proactive retention actions.

---

## 📊 Dataset
- Dataset: Telco Customer Churn Dataset
- Records: ~7,000 customers
- Features include:
  - Customer demographics
  - Subscription details
  - Contract type
  - Billing and payment information

**Target Variable:**
- `Churn` (1 = Yes, 0 = No)

---

## 🛠️ Tech Stack
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🔄 Project Workflow
1. Data loading and inspection
2. Data cleaning and preprocessing
3. Handling incorrect data types
4. Feature encoding using One-Hot Encoding
5. Train-test split
6. Model training and evaluation
7. Model comparison

---

## 🧹 Data Preprocessing
- Removed non-predictive identifier column (`customerID`)
- Converted numerical fields stored as text (`TotalCharges`)
- Encoded categorical variables using one-hot encoding
- Prepared final dataset with 31 meaningful features

---

## 🤖 Models Used
### Logistic Regression (Final Model)
- Accuracy: ~82%
- Strong recall for churned customers
- Chosen for interpretability and business relevance

### Random Forest (Compared)
- Accuracy: ~79%
- Lower recall for churned customers
- Not selected as final model

---

## 📈 Model Evaluation (Final Model)
- Accuracy: ~82%
- Precision (Churn): ~0.69
- Recall (Churn): ~0.60
- F1-score (Churn): ~0.64

Logistic Regression was selected as it performed better on the minority churn class, which is critical for business retention strategies.

---

## 💡 Business Insights
- Customers on month-to-month contracts are more likely to churn
- Higher monthly charges correlate with higher churn probability
- Long-tenure customers show lower churn risk

---

## 🚀 Conclusion
This project demonstrates an end-to-end machine learning pipeline for churn prediction, focusing on data preprocessing, model selection, and business-driven evaluation.

---

## 📂 Project Structure
customer-churn-project/
│
├── data/
│ └── raw_data.csv
│
├── notebooks/
│ ├── 01_data_loading.ipynb
│ ├── 02_data_cleaning.ipynb
│ ├── 03_encoding.ipynb
│ ├── 04_modeling.ipynb
│
├── README.md
└── requirements.txt


---

## 📌 How to Run
1. Clone the repository
2. Install dependencies:
pip install -r requirements.txt
3. Run notebooks in order from `notebooks/`