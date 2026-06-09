# End-to-End ML Pipeline for Customer Churn Prediction

## Overview

Customer churn is one of the most important business problems in the telecommunications industry. Retaining existing customers is often more cost-effective than acquiring new ones.

This project builds a complete **Machine Learning Pipeline** using **Scikit-learn** to predict whether a customer is likely to leave a telecom service provider. The pipeline automates data preprocessing, feature transformation, model training, and evaluation, making it reusable for future datasets and production deployment.

Two machine learning models are implemented and compared:

* Logistic Regression
* Random Forest Classifier

---

## Objective

The goal of this project is to develop an end-to-end machine learning workflow that can accurately identify customers at risk of churn.

The pipeline includes:

* Data preprocessing
* Missing value handling
* Feature encoding
* Feature scaling
* Model training
* Performance evaluation
* Prediction generation

---

## Dataset

### Telco Customer Churn Dataset

The dataset contains customer demographic information, account details, subscribed services, and churn status.

### Target Variable

| Column | Description                                            |
| ------ | ------------------------------------------------------ |
| Churn  | Indicates whether a customer left the company (Yes/No) |

### Example Features

* Gender
* Senior Citizen
* Partner
* Dependents
* Tenure
* Internet Service
* Contract Type
* Monthly Charges
* Total Charges
* Payment Method

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

---

## Project Structure

```text
Customer-Churn-Prediction/
│
├── data/
│   └── Telco-Customer-Churn.csv
│
├── notebooks/
│   └── task2_ml_pipeline.ipynb
│
├── models/
│
├── README.md
├── requirements.txt
└── churn_pipeline.py
```

---

## Machine Learning Pipeline

The project utilizes Scikit-learn Pipelines and Column Transformers to create a reusable workflow.

### Data Preprocessing

#### Numerical Features

* Missing value imputation
* Standard Scaling

#### Categorical Features

* Missing value imputation
* One-Hot Encoding

### Pipeline Components

```text
Raw Data
    ↓
Data Cleaning
    ↓
Feature Engineering
    ↓
Column Transformer
    ↓
Model Training
    ↓
Prediction
    ↓
Evaluation
```

---

## Models Used

### Logistic Regression

A simple and interpretable baseline model for binary classification.

**Advantages**

* Fast training
* Easy interpretation
* Good baseline performance

### Random Forest Classifier

An ensemble learning algorithm that combines multiple decision trees.

**Advantages**

* Handles nonlinear relationships
* Robust to overfitting
* High predictive performance

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/customer-churn-prediction.git
cd customer-churn-prediction
```

Install required packages:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

---

## Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
task2_ml_pipeline.ipynb
```

Run all cells to:

1. Load the dataset
2. Build preprocessing pipelines
3. Train Logistic Regression
4. Train Random Forest
5. Compare performance
6. Generate churn predictions

---

## Evaluation Metrics

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC Score
* Confusion Matrix

Example:

| Metric    | Logistic Regression | Random Forest |
| --------- | ------------------- | ------------- |
| Accuracy  | 80%                 | 84%           |
| Precision | 79%                 | 83%           |
| Recall    | 72%                 | 78%           |
| F1 Score  | 75%                 | 80%           |

*Results may vary depending on train-test split and preprocessing choices.*

---

## Sample Prediction

Input customer information:

```text
Tenure: 5 months
Contract: Month-to-Month
Internet Service: Fiber Optic
Monthly Charges: $95
```

Output:

```text
Churn Probability: 82%
Prediction: Customer Likely to Churn
```

---

## Key Features

* End-to-end machine learning workflow
* Automated preprocessing pipeline
* Reusable and scalable architecture
* Comparison of multiple models
* Suitable for deployment and production environments

---

## Future Improvements

* Hyperparameter tuning using GridSearchCV
* Feature selection techniques
* XGBoost implementation
* Model deployment using Streamlit
* Real-time prediction API using Flask or FastAPI

---

## Learning Outcomes

Through this project, you will learn:

* Data preprocessing with Scikit-learn
* Building reusable ML pipelines
* Feature engineering
* Binary classification
* Model evaluation
* Customer churn analytics
* Production-ready machine learning workflows

---

## Author

**Nimra Zia**

BS Artificial Intelligence

Machine Learning & Data Science Enthusiast
