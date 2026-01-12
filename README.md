# Customer Churn Prediction
This project focuses on predicting customer churn using a supervised machine learning approach.
The goal is to identify customers at high risk of leaving, using structured customer data and interpretable classification models.

The project is designed as an end-to-end data analysis workflow, from exploratory data analysis to model evaluation.

---

## Project Overview

Customer churn prediction is a common business problem in subscription-based and customer-centric industries.
In this project, I develop a classification pipeline to:

- explore and preprocess customer data
- engineer relevant features
- train and validate predictive models
- evaluate performance using standard classification metrics

The emphasis is on clarity, reproducibility, and interpretability rather than model complexity.

---

## Dataset

- The dataset contains customer-level information such as demographics, service usage, and contract details.
- The target variable indicates whether a customer has churned.
- Data are provided as a structured tabular dataset (CSV format).

The dataset is included in the repository to ensure full reproducibility.

---

## Project Structure

```
customer-churn-prediction/
│
├── data/
│   ├── raw/                # Original dataset
│   └── processed/          # Cleaned data used for modeling
│
├── models/                 # Saved models or model-related artifacts
│
│
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_preprocessing.ipynb
│   └── 03_modeling.ipynb
│
├── requirements.txt
├── .gitignore
└── README.md
\
```

---

## Workflow

The analysis is organized into sequential notebooks:
1. Exploratory Data Analysis
   - inspection of data quality and distributions
   - identification of missing values and potential predictors
   - initial insights into churn patterns
2. Preprocessing & Feature Engineering
   - encoding of categorical variables
   - feature selection and transformation
   - preparation of train/test splits
3. Modeling & Evaluation
   - baseline classification models
   - performance evaluation on test data
   - comparison using standard metrics (accuracy, precision, recall, ROC-AUC)

---

## Results

- A baseline classification model was trained to predict customer churn.
- Model performance was evaluated using standard metrics to assess predictive quality.
- The final model provides a reasonable trade-off between performance and interpretability.

This project is intended as a demonstrator of a clean and reproducible ML workflow rather than a production-grade system.

---

## How to Run the Project

Clone the repository:
```
git clone https://github.com/stefanoavanzini/customer-churn-prediction.git
cd customer-churn-prediction
```

Create and activate a virtual environment:
```
python -m venv venv
source venv/bin/activate
```

Install dependencies:
```
pip install -r requirements.txt
```

Open the notebooks:
```
jupyter notebook
```

and run them in order (01_eda → 02_preprocessing → 03_modeling).

---

## Technologies Used

Python  
pandas, numpy  
scikit-learn  
matplotlib, seaborn  
Jupyter Notebook  
Git

---

## Notes

This project is part of a personal portfolio focused on applied data analysis and predictive modeling.
The emphasis is on methodological clarity, reproducibility, and clear communication of results.

---
## Author

Stefano Avanzini