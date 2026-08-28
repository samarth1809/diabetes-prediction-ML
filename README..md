# Diabetes Prediction using Machine Learning

A machine learning project that predicts whether a patient is likely to have diabetes based on diagnostic health measurements (Pima Indians Diabetes Dataset).

## 📋 Overview

This project builds and compares multiple ML models to classify patients as diabetic or non-diabetic, using features such as glucose level, BMI, blood pressure, insulin, and age.

## 📊 Dataset

- **Source:** Pima Indians Diabetes Dataset (`diabetes.csv`)
- **Target variable:** `Outcome` (1 = Diabetic, 0 = Non-diabetic)
- **Features:** Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age

## 🔍 Project Workflow

1. **Import Libraries** – pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost
2. **Load the Dataset** – reading and initial inspection of the data
3. **Exploratory Data Analysis (EDA)**
   - Outlier detection (boxplots)
   - Pairplot for feature relationships
4. **Data Cleaning & Validation** – handling missing/invalid values (e.g. biologically impossible zeros)
5. **Feature Scaling & Train-Test Split** – standardizing features and splitting data
6. **Model Training** – training multiple classification models
7. **Model Comparison** – comparing model performance
8. **Detailed Evaluation** – accuracy, classification report, confusion matrix
9. **Feature Importance** – using Random Forest to identify key predictors
10. **Hyperparameter Tuning** – optimizing model parameters
11. **XGBoost Classifier** – gradient boosting model for improved performance

## 🛠️ Tech Stack

- Python 3
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- XGBoost

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```

### Running the Notebook
1. Clone this repository
   ```bash
   git clone https://github.com/samarth1809/<repo-name>.git
   cd <repo-name>
   ```
2. Open the notebook in Jupyter or Google Colab
3. Run all cells in order

## 📈 Results

Model performance is evaluated using accuracy, precision, recall, F1-score, and classification reports across multiple models including Random Forest and XGBoost.

## 📁 Project Structure

```
├── diabetes.csv
├── Diabetes_Prediction.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

