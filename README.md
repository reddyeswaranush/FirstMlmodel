# Titanic Survivability Prediction 🚢

This project uses machine learning to predict passenger survivability from the Titanic dataset.

## 🔍 Overview

Using features such as age, sex, fare, and passenger class, the model predicts whether a passenger would survive the Titanic disaster.

## 📂 Dataset

- Source: [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)
- CSV file used: `Titanic-Dataset.csv`
- Preprocessing steps:
  - Dropped irrelevant columns (`Name`, `Ticket`, `Cabin`, `PassengerId`)
  - Filled missing `Age` values with the mean
  - Converted categorical data using one-hot encoding (`get_dummies`)

## 🧠 Model

- **Model Used**: Random Forest Regressor (though it behaves like a classifier in this case)
- **Train-Test Split**: 80-20 split
- **Evaluation Metrics**:
  - Accuracy: ~81%
  - Precision: 0.79
  - Recall: 0.74
  - F1-Score: 0.76

## 📊 Output

```python
Precision: 0.7971
Recall:    0.7432
F1-Score:  0.7692
Accuracy:  ~81%
