 Diabetes Prediction using Machine Learning

**A machine learning project that predicts whether a patient has diabetes based on diagnostic health measurements, built as part of the InternPe Machine Learning Internship.**

---

## 📌 Project Overview

This project uses the **Pima Indians Diabetes Dataset** to train and compare multiple machine learning models that predict the likelihood of a patient having diabetes. The notebook covers the **full ML pipeline** — from data cleaning and exploratory analysis to model training, tuning, evaluation, and saving the final model for reuse.

**Key highlights:**

- ✅ **Real-world medical dataset** (768 patients, 8 diagnostic features)
- ✅ **Proper handling of missing/invalid data** (biologically impossible zero values treated as missing and imputed)
- ✅ **5 ML models trained and compared**: Logistic Regression, Decision Tree, Random Forest, K-Nearest Neighbors, and Support Vector Machine
- ✅ **Hyperparameter tuning** with GridSearchCV
- ✅ **XGBoost** implementation for advanced comparison
- ✅ **Model persistence** using `joblib` for deployment-readiness
- ✅ **Full EDA**: correlation heatmaps, boxplots, pairplots, class distribution

---

## 📊 Dataset

| Detail | Description |
|---|---|
| **Source** | Pima Indians Diabetes Dataset |
| **File** | `diabetes.csv` |
| **Rows** | 768 patients |
| **Features** | 8 predictor variables + 1 target (`Outcome`) |

**Predictor features:**

- `Pregnancies` — Number of times pregnant
- `Glucose` — Plasma glucose concentration
- `BloodPressure` — Diastolic blood pressure (mm Hg)
- `SkinThickness` — Triceps skinfold thickness (mm)
- `Insulin` — 2-Hour serum insulin (mu U/ml)
- `BMI` — Body mass index
- `DiabetesPedigreeFunction` — Diabetes likelihood based on family history
- `Age` — Age in years

**Target:**

- `Outcome` — `1` = Diabetic, `0` = Not Diabetic

---

## 🛠️ Tech Stack

- **Language:** Python 3
- **Environment:** Google Colab / Jupyter Notebook
- **Libraries:**
  - `pandas`, `numpy` — data handling
  - `matplotlib`, `seaborn` — visualization
  - `scikit-learn` — machine learning models, scaling, evaluation
  - `xgboost` — gradient boosting model
  - `joblib` — model saving/loading

---

## 🚀 Project Workflow

1. **Import Libraries**
2. **Load Dataset** — read `diabetes.csv`
3. **Exploratory Data Analysis (EDA)** — class balance, correlation heatmap, feature distributions, outlier detection, pairplots
4. **Data Cleaning & Validation** — replace invalid zero values in `Glucose`, `BloodPressure`, `SkinThickness`, `Insulin`, and `BMI` with the median
5. **Feature Scaling & Train-Test Split** — `StandardScaler` + 80/20 split
6. **Model Training** — Logistic Regression, Decision Tree, Random Forest, KNN, SVM
7. **Model Comparison** — accuracy and cross-validation scores across all models
8. **Detailed Evaluation** — confusion matrix, classification report, ROC curve for the best model
9. **Feature Importance** — Random Forest feature ranking
10. **Hyperparameter Tuning** — GridSearchCV on Random Forest
11. **XGBoost Model** — additional gradient boosting comparison
12. **Save Final Model** — export as `diabetes_model.pkl` and `scaler.pkl`
13. **Predict on New Patient** — sample real-world prediction demo

---

## ⚙️ How to Run

### Option 1: Google Colab (Recommended)

1. Upload `Diabetes_Prediction_InternPe.ipynb` to [Google Colab](https://colab.research.google.com/).
2. Upload `diabetes.csv` into the same session (sidebar → 📁 folder icon → upload), or mount Google Drive using the instructions in the notebook.
3. Go to **Runtime → Run all**.

### Option 2: Local Jupyter Notebook

```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
pip install -r requirements.txt
jupyter notebook Diabetes_Prediction_InternPe.ipynb
```

---

## 📦 Requirements

```
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
joblib
```

---

## 📈 Results

The notebook trains and compares **5 machine learning models**, then selects the best-performing one for detailed evaluation (confusion matrix, classification report, and ROC-AUC curve). It also applies **GridSearchCV** to tune Random Forest and trains an **XGBoost** model for further comparison.

> Exact accuracy scores will appear when you run the notebook — they can vary slightly depending on library versions and random seeds.

**Feature importance analysis** consistently highlights `Glucose`, `BMI`, and `Age` as the strongest predictors of diabetes risk.

---

## 📁 Project Structure

```
├── Diabetes_Prediction_InternPe.ipynb   # Main notebook (full ML pipeline)
├── diabetes.csv                         # Dataset
├── diabetes_model.pkl                   # Saved best model (generated after running)
├── scaler.pkl                           # Saved StandardScaler (generated after running)
└── README.md                            # Project documentation
```

---

## 🔮 Future Work

- Deploy the model as a **Flask** or **Streamlit** web app
- Collect a larger, more diverse patient dataset
- Experiment with deep learning (e.g., a simple neural network)
- Add SHAP/LIME explainability for individual predictions

## 📄 License

This project is open-source and available for educational use.
