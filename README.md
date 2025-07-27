# 🏦 Loan Approval Automation

This project focuses on building a machine learning model to automate loan approval decisions using a synthetic dataset of 50,000 applications. It covers data cleaning, feature engineering, model selection, and performance evaluation.

---

## 📌 Objective

To develop a binary classification model that predicts whether a loan should be **approved (1)** or **rejected (0)** based on applicant financial and demographic data.

---

## 🗂️ Dataset

- Synthetic dataset with 50,000 loan applications.
- Includes over 35 features such as:
  - `Age`, `AnnualIncome`, `CreditScore`, `LoanAmount`, `LoanPurpose`
  - Employment and education info
  - Debt, liabilities, and assets
  - Encoded categorical features and engineered ratios
- Target column: `LoanApproved`

---

## 🔍 Project Highlights

### ✅ Exploratory Data Analysis (EDA)
- Summary statistics
- Missing values & outlier handling (IQR & capping)
- Target variable distribution
- Correlation matrices (Pearson, Spearman)
- Mutual Information scoring

### 🧠 Feature Engineering
- Extracted features from `ApplicationDate`
- Ratios like `LoanAmount / AnnualIncome`
- Combined liquid assets and debt-to-income ratio

### 🏗️ Preprocessing
- One-hot encoding for categorical features
- Label encoding for education levels
- Scaling using `StandardScaler`
- Splitting into training/testing sets (80/20)

### 🤖 Models Applied
- **Basic Classifiers**: Logistic Regression, KNN, Naive Bayes, Decision Tree
- **Ensemble**: Random Forest, Extra Trees, AdaBoost, Gradient Boosting
- **Boosting**: XGBoost, LightGBM
- Evaluation using:
  - Accuracy
  - ROC AUC
  - Confusion Matrix
  - F1-score

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/loan-approval-automation.git
cd loan-approval-automation
```

### 2. Install required packages

```bash
pip install -r requirements.txt
```

### 3. Run the notebook

Use Jupyter Notebook or Google Colab to open and run `loan_approval_automation.ipynb`.

---

## 📊 Example Results (Logistic Regression)

Training Accuracy: 94.85%  
Training ROC AUC: 99.14%  
Test Accuracy: 94.60%  
Test ROC AUC: 98.85%  

---

## 📁 Folder Structure

.
├── loan_approval_automation.ipynb  
├── README.md  
├── requirements.txt  
└── data/  
    └── LoanApplicationsDataset.csv  

---

## 📜 License

This project is licensed under the MIT License.

---

## ✍️ Author

Turki Alqou  
As this is a learning project made by a beginner, feel free to fork, use, or contribute to it.
