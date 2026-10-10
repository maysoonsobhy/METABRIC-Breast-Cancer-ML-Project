# METABRIC Breast Cancer Classification & Machine Learning Pipeline

## 📌 Project Overview
This repository contains an end-to-end Machine Learning classification and data preprocessing pipeline built using the **METABRIC** breast cancer gene expression dataset. The project implements robust data preprocessing, dimensionality reduction, hyperparameter tuning, and cross-validation to predict clinical patient outcomes.

---

## 🚀 Key Features & Workflow
* **Data Preprocessing & Cleaning:** Handled missing values using median/most frequent imputation, encoded categorical features safely, and converted types to prevent mixed-type errors.
* **Feature Engineering & Transformation:** Utilized `ColumnTransformer` and `Pipeline` architectures to seamlessly integrate numerical scaling and categorical encoding.
* **Dimensionality Reduction:** Applied **Principal Component Analysis (PCA)** to reduce feature redundancy while retaining 95% of cumulative variance.
* **Model Optimization:** Performed hyperparameter tuning using `GridSearchCV` combined with **Stratified K-Fold Cross-Validation** across multiple classifiers:
  * Random Forest Classifier
  * Gradient Boosting Classifier
  * Logistic Regression
* **Artifact Exporting:** Saved the optimal trained pipeline and preprocessor transformer as `.joblib` files for direct inference and production deployment.

---

## 🛠️ Tech Stack & Libraries
* **Python**
* **Pandas & NumPy** (Data manipulation and numerical operations)
* **Scikit-Learn** (Pipelines, preprocessing, PCA, models, and grid search)
* **Joblib** (Model serialization and artifact persistence)


│   ├── metabric_model_pipeline.joblib    # Fully trained optimal pipeline & model
│   └── preprocessor_transformer.joblib   # Fitted data preprocessor transformer
├── README.md                             # Project documentation
