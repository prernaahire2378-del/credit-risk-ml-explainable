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

📌 Inspiration

This project explores how machine learning can help assess credit risk and how Explainable AI can make model predictions easier to understand.

The goal is to analyze customer-related information, predict potential credit risk, evaluate model performance, and identify the factors influencing predictions.

Acknowledgment: This project was inspired by existing credit risk analysis work. Credit and acknowledgment should be given to the original authors whose work informed this project.

---

## 🚀 How to Run

🚀 How to Run

Follow these steps to run the project on your computer.

1. Download the repository

Download the project files from this GitHub repository and extract them into a folder.

Alternatively, clone the repository using Git:

git clone https://github.com/prernaahire2378-del/credit-risk-ml-explainable.git
cd credit-risk-ml-explainable

2. Create a virtual environment

python -m venv venv

On Windows, activate it using:

venv\Scripts\activate

3. Install dependencies

Install Jupyter Notebook:

pip install notebook

Install the other Python libraries required by the project. Check the notebook for the exact dependencies.

4. Open Jupyter Notebook

jupyter notebook

Open "credit-risk-analysis.ipynb" in your browser.

5. Run the notebook

1. Confirm that "training-data.csv" is available in the expected location.
2. Select the appropriate Python kernel.
3. Run the notebook cells in order.
4. Review the model evaluation and explainability results.

Note: The required libraries and execution steps should be verified by running the notebook.






