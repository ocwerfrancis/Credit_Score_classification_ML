# Credit_Score_classification_ML
Banks and credit card companies calculate your credit score to determine your creditworthiness. It helps banks and credit card companies immediately to issue loans to customers with good creditworthiness. Today banks and credit card companies use Machine Learning algorithms to classify customers in their database based on their credit history

# **Overview**
This project focuses on `classifying customers'` credit scores into three categories: `Good, Standard,` and `Poor`, using machine learning techniques. The goal is to help banks and credit card companies assess creditworthiness efficiently by leveraging historical credit data.

# Dataset
The dataset contains the following features:

**Demographic Information:** `Age, Occupation, Annual Income, Monthly Inhand Salary`.

**Financial Behavior:** `er of bank accounts, credit cards, loans, delayed payments, outstanding debt`, etc.

**Credit History:** `Credit mix, credit utilization ratio, credit history age` and more.

**Target Variable:** `Credit_Score (Good, Standard, Poor).`

# Data Source
The dataset is sourced from `Kaggle` and includes:

**Training Data:** *train.csv* (**100,000** rows, 28 columns).

**Test Data:** *test.csv*(**50,000** rows, 27 columns).

# Data Preprocessing
## Steps Performed:
- **Handling Missing Values:** Replaced invalid entries (e.g., _, !@9#%8) with NaN and imputed missing values where necessary.

- **Data Type Conversion:** Converted columns like `Age, Annual_Income,` and `Num_of_Loan` to numeric types.

# Feature Engineering:

- Extracted `Month_Num` from the `Month column` for numerical analysis.

- Converted Credit_History_Age (e.g., `"22 Years and 1 Months"`) into months (`Credit_History_Age_Months`).

- Created binary features for loan types (e.g., Loan_auto_loan, Loan_personal_loan).

- Added `Num_Loan_Types` to count the number of loan types per customer.

- Encoding: Mapped the target variable Credit_Score to numerical values (Good: 2, Standard: 1, Poor: 0).

# Key Features
- **Numerical Features:** `Age, Annual Income, Monthly Inhand Salary, Number of Bank Accounts`, etc.

- **Categorical Features:** `Occupation, Credit Mix, Payment Behavior,` etc.

- **Derived Features:** `Credit History Age in months, Loan Type indicators.`

## Next Steps
- Exploratory Data Analysis (EDA): Visualize distributions, correlations, and outliers.

- Model Training: Experiment with classifiers like Random Forest, Gradient Boosting, and Logistic Regression.

- Evaluation: Use metrics like accuracy, precision, recall, and F1-score to assess model performance.

- Deployment: Deploy the best-performing model for real-time credit score classification.

## Dependencies
`Python 3.x`

**Libraries:** `pandas, numpy, matplotlib, seaborn, scikit-learn.`

Usage
Clone the repository.

Install dependencies: pip install pandas numpy matplotlib seaborn scikit-learn.

Run the Jupyter notebook to preprocess data, train models, and evaluate results.

