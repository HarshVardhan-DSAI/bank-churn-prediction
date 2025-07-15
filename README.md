# 🏦 Bank Churn Prediction

Predicting whether bank customers are likely to churn (leave the bank) using machine learning.

---

## 📌 **Project Goal**
To identify customers most likely to churn, so the bank can proactively reduce churn through targeted retention strategies.

---

## 📊 **Dataset**
The dataset contains anonymized bank customer information with the following key features:
- **RowNumber**: Index of the row
- **CustomerId**: Unique ID of the customer
- **Surname**: Customer surname (not used in prediction)
- **CreditScore**: Numeric credit score
- **Geography**: Country (France, Spain, Germany)
- **Gender**: Male/Female
- **Age**: Customer age
- **Tenure**: Number of years as a customer
- **Balance**: Account balance
- **NumOfProducts**: Number of bank products the customer has
- **HasCrCard**: Has credit card (1 = Yes, 0 = No)
- **IsActiveMember**: Active member (1 = Yes, 0 = No)
- **EstimatedSalary**: Estimated annual salary
- **Exited**: Target variable (1 = churned, 0 = stayed)

**Sample data:**
| CreditScore | Geography | Gender | Age | Tenure | Balance | NumOfProducts | HasCrCard | IsActiveMember | EstimatedSalary | Exited |
|-------------|-----------|--------|-----|--------|---------|---------------|----------:|---------------:|----------------:|-------:|
| 619 | France | Female | 42 | 2 | 0.00 | 1 | 1 | 1 | 101348.88 | 1 |
| 608 | Spain | Female | 41 | 1 | 83807.86 | 1 | 0 | 1 | 112542.58 | 0 |
| 502 | France | Female | 42 | 8 | 159660.80 | 3 | 1 | 0 | 113931.57 | 1 |

---

## ⚙️ **Method**
- Data cleaning and preprocessing
- Feature encoding (e.g., converting Geography & Gender to numeric values)
- Trained a **Random Forest Classifier** to predict churn
- Saved trained model using `joblib` for reuse
- Evaluated performance using accuracy score and confusion matrix

---

## 📈 **Results**
Achieved good predictive performance (add your actual accuracy here, e.g., “Accuracy: 86%”).  
Identified key drivers of churn, such as:
- Lower credit scores
- Fewer active products
- Younger age groups

---

## 🧪 **How to Run**
1. Clone this repository:
```bash
git clone https://github.com/HarshVardhan-DSAI/bank-churn-prediction.git

