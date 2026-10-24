# Credit Risk Prediction with Explainable Machine Learning

**Understanding Credit Risk Through Machine Learning and Explainable AI**

## Overview

How can machine learning help identify potential credit risk while making its predictions easier to understand?

This project explores that question by building a machine learning pipeline to predict credit risk from structured customer data. It combines data preprocessing, classification, model evaluation, and Explainable AI (XAI) techniques to examine both model performance and the factors influencing its predictions.

The goal is not just to generate predictions, but also to understand how a model reaches its conclusions.

**Key areas covered**: Machine Learning, Binary Classification, Data Preprocessing, Model Evaluation, and Explainable AI.

## Project Objectives

The project focuses on four main objectives:

- **Predict credit risk**: Build a classification model to distinguish between customers with and without the target risk label.
- **Prepare data for modeling**: Process numerical and categorical features using appropriate preprocessing techniques.
- **Evaluate model performance**: Examine classification results using multiple evaluation methods rather than relying on a single metric.
- **Improve interpretability**: Use SHAP to investigate how input features contribute to model predictions.

## How the Project Works

The notebook follows a structured machine learning workflow.

1. **Data preparation**: Load and inspect the dataset to understand its structure and features.
2. **Feature preprocessing**: Transform numerical and categorical variables into formats suitable for machine learning.
3. **Model training**: Train a Random Forest classifier using a scikit-learn pipeline.
4. **Model evaluation**: Analyze classification performance using evaluation metrics and diagnostic plots.
5. **Model explainability**: Apply SHAP to investigate feature contributions and understand model behavior.

This workflow brings together predictive modeling and interpretability in a single analysis.

## Dataset

The project uses "training-data.csv", a cleaned, structured dataset for credit risk analysis.

The documented input features include:

 **Feature        | Description** 
  
- "Age"           | Customer's age
- "Income"        | Customer's income
- "Married/Single"| Marital status category
-"Profession"    | Customer's profession

**Target variable**: "Risk_Flag"

- "0" — No risk
- "1" — Risk

The target labels represent the dataset's defined classification categories. Their meaning should be interpreted in the context of the original data source.

## Technology Stack

**Technology      | Purpose**  

- Python          | Data processing and machine learning
- Pandas          | Data manipulation and analysis
- NumPy           | Numerical operations
- scikit-learn    | Preprocessing, model training, and evaluation
- Random Forest   | Classification model
- SHAP            | Model explainability
- Matplotlib      | Data visualization
- Jupyter Notebook| Interactive analysis and experimentation

## Machine Learning Approach

### Data Preprocessing

The project uses scikit-learn preprocessing components to handle different feature types.

- "ColumnTransformer" applies transformations to selected columns.
- "StandardScaler" scales numerical features where appropriate.
- "OneHotEncoder" converts categorical variables into numerical representations.
- "Pipeline" organizes preprocessing and model training into a consistent workflow.

Keeping preprocessing steps together with the estimator helps maintain a reproducible modeling process.

### Classification Model

A **Random Forest Classifier** is used to predict the target risk category.

Random Forest combines predictions from multiple decision trees. It can model nonlinear relationships and interactions between features, making it a useful baseline for structured tabular classification tasks.

### Model Evaluation

The notebook includes several evaluation and diagnostic techniques:

- ROC curve and ROC-AUC analysis
- Precision-recall curve
- Confusion matrix
- Learning curve
- Calibration plot

These methods examine different aspects of model behavior, including discrimination, classification errors, learning behavior, and the reliability of predicted probabilities.

Actual performance values should be reported only after verifying the results produced by the notebook.

## Explainable AI with SHAP

A model's prediction is more useful when its behavior can be investigated.

This project uses SHAP (SHapley Additive exPlanations) to analyze the contribution of input features to model predictions.

SHAP can help explore two questions:

- **Global interpretation**: Which features contribute most to predictions across the analyzed dataset?
- **Individual interpretation**: How do features contribute to a particular prediction?

These explanations can make model behavior easier to inspect and communicate.

However, feature contributions describe the model's behavior; they do not establish that a feature causes credit risk.

## Project Structure

credit-risk-ml-explainable/
│
├── credit-risk-analysis.ipynb   # Analysis, training, evaluation and explainability
├── training-data.csv            # Dataset used for model development
└── README.md                    # Project documentation

## Getting Started

Follow these steps to run the project locally.

1. **Clone the Repository**

       git clone https://github.com/prernaahire2378-del/credit-risk-ml-explainable.git
       cd credit-risk-ml-explainable

2. **Create a Virtual Environment**

       python -m venv venv

       Activate it on Windows:

       venv\Scripts\activate

3. **Install the Required Libraries**

       Install the main libraries used by the project:

       python -m pip install pandas numpy scikit-learn matplotlib shap jupyter

       If the notebook uses additional libraries, install those as well.

4. **Launch Jupyter Notebook**

       jupyter notebook

       Open "credit-risk-analysis.ipynb" in your browser.

5. **Run the Analysis**

       1. Select the appropriate Python kernel.
       2. Confirm that "training-data.csv" is accessible from the notebook's working directory.
       3. Run the cells in order.
       4. Review the preprocessing steps, model evaluation results, plots, and SHAP explanations.

       For consistent results, use the same dataset and preprocessing configuration as the notebook.

## Results and Interpretation

- **Exact-profile overlap:** 85.6% of hold-out rows had a feature profile also present in training.
- **Grouped split (random_state=42):** ROC-AUC 0.511, accuracy 0.828, and high-risk recall 0.069.

The notebook is designed to examine model performance through multiple evaluation methods and explore feature contributions using SHAP.

The evaluation should consider more than overall accuracy. ROC-AUC, precision-recall behavior, the confusion matrix, and probability calibration provide complementary information about the classifier.



## Limitations and Future Improvements

This project is an educational machine learning exercise, and several improvements could make it more robust.

- Compare Random Forest with baseline models such as Logistic Regression and Decision Tree.
- Evaluate class imbalance and select metrics appropriate to the target distribution.
- Use stratified cross-validation to assess performance stability.
- Examine feature importance and SHAP explanations for unexpected model behavior.
- Investigate fairness and potential bias across relevant customer groups where suitable data is available.
- Document the dataset source, data quality checks, and final evaluation results.
- Add a simple application interface or API to demonstrate predictions interactively.

These extensions would help move the project from exploratory analysis toward a more complete and carefully evaluated machine learning application.

## Responsible Use

Credit risk assessment can affect important financial decisions. A model developed for learning or experimentation should not be treated as a validated lending system.

The model's predictions may reflect limitations, biases, or patterns present in its training data. Real-world use would require additional validation, fairness assessment, appropriate governance, and human oversight.

This project is intended for educational and portfolio demonstration purposes, not for making real credit or lending decisions.

## Acknowledgment

This project was inspired by existing credit risk analysis work. Appropriate credit should be given to the original authors and data providers whose work informed the project.

## Author

### Prerna Ahire

Explore the code and notebook in this repository:

"Credit Risk ML Explainable on GitHub" (https://github.com/prernaahire2378-del/credit-risk-ml-explainable)

---

Built to explore the practical application of machine learning and explainable AI to credit risk analysis.


