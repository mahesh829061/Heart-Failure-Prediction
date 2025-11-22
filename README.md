# Heart-Failure-Prediction

**Predicting heart failure using machine learning**

## 🔎 Project overview

This repository contains code and analysis to predict heart failure risk from patient-level features using classical machine learning and a small artificial neural network (ANN). The analysis demonstrates data cleaning, exploratory data analysis (EDA), feature engineering, model training, evaluation, and interpretation.

> *Goal:* Build and evaluate models that predict the presence/occurrence of heart failure from the provided dataset and package the pipeline so others can reproduce results.

---

## 📂 What’s in this repo

* `Analysis-and-Model.ipynb` — Jupyter notebook with EDA, preprocessing, training, evaluation, and visualizations.
* `ANN_heart_Prediction.csv` — (exported) dataset used for modeling.
* `README.md` — this file.

---

## 🧾 Dataset

**Columns (example):** `age, anaemia, creatinine_phosphokinase, diabetes, ejection_fraction, high_blood_pressure, platelets, serum_creatinine, serum_sodium, sex, smoking, time, target`

**Target:** `target` (1 = death event — or change depending on dataset). Clarify label encoding used in the notebook.

---

## 🛠️ Requirements

Create a Python virtual environment and install packages. Example dependencies used in the notebook:

```
python>=3.8
pandas
numpy
scikit-learn
matplotlib
seaborn
jupyter
tensorflow>=2.0  # only if using the ANN implementation
joblib
shap
```

---

## 📈 Models & Results

I trained several models and evaluated them on the held-out test set. For each model i report: Accuracy, Precision, Recall, F1-score, and ROC AUC.:

* Logistic Regression — Accuracy: 0.85, ROC AUC: 0.88
* Random Forest — Accuracy: 0.87, ROC AUC: 0.90
* ANN (Keras) — Accuracy: 0.86, ROC AUC: 0.89

Add confusion matrices and ROC plots saved to `reports/figures/` for reproducibility.

---
