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

## 🚀 How to Run

Follow these steps to set up and run the project locally.

1. Clone the repository

Open a terminal and run:

git clone https://github.com/prernaahire2378-del/credit-risk-ml-explainable.git

Navigate into the project folder:

cd credit-risk-ml-explainable

2. Create a virtual environment

Create a virtual environment using Python:

python -m venv venv

Activate it on Windows:

venv\Scripts\activate

3. Install the required libraries

Install the libraries needed to run the notebook.

If the repository contains a "requirements.txt" file, run:

pip install -r requirements.txt

If no requirements file exists, install the dependencies specified in the notebook.

4. Launch Jupyter Notebook

Run:

pip install notebook
jupyter notebook

Open "credit-risk-analysis.ipynb" in your browser.

5. Run the notebook

1. Make sure "training-data.csv" is in the expected location.
2. Select the appropriate Python kernel.
3. Run the notebook cells from top to bottom.
4. Review the model evaluation results and explainability outputs.

Note: The exact dependencies and execution steps should be verified against the notebook before publishing this guide.
