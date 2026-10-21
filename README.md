# 🧠 Credit Risk Prediction with Machine Learning

This project builds a full machine learning pipeline to predict credit risk using structured tabular data. It includes data preprocessing, model evaluation using ROC AUC and PR curves, model calibration, and explainability via SHAP. Developed entirely in Jupyter Notebook with `scikit-learn`, the pipeline is transparent, modular, and suitable for extension or deployment.

---

## 📂 Project Overview

- Predict whether a customer is a credit risk (`Risk_Flag`) based on features like age, income, marital status, and profession.
- Evaluate model performance with ROC AUC, precision-recall, learning curves, and calibration plots.
- Interpret model behavior using SHAP values for feature importance and explanation.
- Focused on clarity, reproducibility, and explainability.

---

## 📈 Techniques Used

- **Preprocessing:**  
  `ColumnTransformer` with `StandardScaler` and `OneHotEncoder` for handling numeric and categorical data.

- **Model:**  
  Random Forest Classifier via a clean `Pipeline`.

- **Evaluation Metrics:**  
  - ROC AUC and PR Curve  
  - Confusion Matrix  
  - Learning Curve  
  - Calibration Plot

- **Explainability:**  
  SHAP (SHapley Additive exPlanations) to identify and visualize feature impact.

---

## 📊 Dataset

- **Training Data Source:**  
  `training-data.csv` — a cleaned and structured dataset based on public credit scoring data.

- Features used:  
  - `Age`  
  - `Income`  
  - `Married/Single`  
  - `Profession`  

- Target variable:  
  - `Risk_Flag` (0 = No Risk, 1 = Risk)

---

## 📌 Inspiration

> This project was heavily inspired by [Dr. Haulder](https://github.com/haulder)'s original credit risk analysis notebook, which laid the foundation for data structure and modeling approach.

---

## 🧪 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/jackdoesjava/credit-risk-prediction-ml.git
   cd credit-risk-prediction-ml

2. Create a venv and install dependencies

3. Open the notebook

