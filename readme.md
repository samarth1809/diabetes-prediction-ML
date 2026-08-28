Diabetes Prediction using Machine Learning
A machine learning project built during my AI/ML internship at InternPe, predicting whether a patient is likely to have diabetes based on diagnostic health measurements.
Dataset
Pima Indians Diabetes Dataset — 768 patient records with 8 diagnostic features (Pregnancies, Glucose, Blood Pressure, Skin Thickness, Insulin, BMI, Diabetes Pedigree Function, Age) and a binary target (Outcome: 1 = diabetic, 0 = not diabetic).
🔍 Project Workflow
Exploratory Data Analysis — class distribution, feature histograms, correlation heatmap, outlier detection (boxplots), pairplots
Data Cleaning & Validation — handled invalid/missing values in medical features (e.g. zero values in Glucose, BMI, BloodPressure)
Feature Scaling & Train-Test Split — standardized features using StandardScaler
Model Training — trained and compared multiple models
Model Comparison — evaluated Logistic Regression, KNN, Random Forest, and XGBoost
Detailed Evaluation — accuracy, precision, recall, F1-score, confusion matrix
Feature Importance — identified key predictors using Random Forest
Hyperparameter Tuning — optimized model parameters for best performance
🛠️ Tech Stack
Python 3
pandas, numpy
matplotlib, seaborn
scikit-learn
XGBoost
🚀 Getting Started
Prerequisites
Bash
Running the Notebook
Bash
Open Diabetes_Prediction_using_ML.ipynb in Jupyter or Google Colab and run all cells.
📈 Results
Glucose, BMI, and Age turned out to be the strongest predictors — highlighting how much proper data cleaning adds value before modelling even starts.
📁 Project Structure
Code