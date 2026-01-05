# Customer Churn Prediction

This project explores a supervised machine learning approach to predict customer churn using Python and scikit-learn.

The goal is to build a clear, reproducible end-to-end workflow covering:
- exploratory data analysis,
- feature engineering and preprocessing,
- baseline predictive modeling and evaluation.

The project is intended as a portfolio example of applied data science rather than a production-ready system.

---

## Project Structure

customer-churn-prediction/
│
├── data/
│ └── raw/ # Raw dataset (not tracked if proprietary)
│
├── notebooks/
│ ├── 01_data_exploration.ipynb
│ ├── 02_feature_engineering.ipynb
│ └── 03_modeling.ipynb
│
├── requirements.txt
└── README.md


---

## Dataset

The dataset contains customer-level information such as:
- demographic features,
- subscription details,
- usage patterns,
- churn status (target variable).

The target variable is binary (`Yes` / `No`) and represents whether a customer has churned.

---

## Workflow Overview

### 1. Exploratory Data Analysis
Initial inspection of the dataset, including:
- distribution of the target variable,
- relationships between churn and key features,
- identification of missing values and categorical variables.

### 2. Feature Engineering
- Separation of numerical and categorical features.
- Scaling of numerical variables.
- One-hot encoding of categorical variables.
- Use of scikit-learn pipelines to prevent data leakage.

### 3. Modeling
- Logistic Regression used as a baseline classifier.
- Model evaluation using accuracy, confusion matrix, ROC curve, and AUC.
- Emphasis on interpretability and reproducibility.

---

## Results & Insights

A baseline classification model was trained to predict customer churn using engineered features derived from customer demographics, account information, and service usage.

**Key results:**
- The baseline Logistic Regression model achieves reasonable performance on unseen data.
- ROC–AUC was used as the primary evaluation metric to account for class imbalance.
- The model provides interpretable coefficients, allowing insight into key drivers of churn.

**Key insights:**
- Contract type and tenure are among the strongest predictors of churn.
- Customers on month-to-month contracts show significantly higher churn risk.
- Longer tenure and bundled services are associated with lower churn probability.

---

## Technologies Used

- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
- Jupyter Notebook
- Git / GitHub

---

## Notes

This project focuses on clarity, interpretability, and reproducibility rather than model complexity.
Future extensions may include:
- alternative classifiers,
- hyperparameter tuning,
- cross-validation,
- feature importance analysis.

---

## Author

Stefano Avanzini
