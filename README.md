# 🤖 XAI Assignment
# 💓 Heart Disease Prediction with XGBoost, SHAP, LIME, and DiCE

This repository demonstrates how to predict heart disease using the **XGBoost** model and explain its predictions using three powerful explainability techniques: **SHAP**, **LIME**, and **DiCE**. The dataset used is the famous **Cleveland Heart Disease Dataset**.

## 🚀 Overview

This project walks you through:
- **Data preprocessing** (cleaning and scaling).
- **Model training** with **XGBoost**.
- **Model explanation** using **SHAP**, **LIME**, and **DiCE** to interpret the model's predictions.

### 🧑‍💻 Techniques Used:

1. **XGBoost Classifier**: 
   - A state-of-the-art gradient boosting algorithm for classification tasks. It helps predict whether a person has heart disease or not.

2. **SHAP (Shapley Additive Explanations)**: 
   - Visualizes **how each feature** (e.g., age, cholesterol, etc.) contributes to the model's prediction.
   - Provides both **global insights** (overall trends) and **local insights** (individual predictions).

3. **LIME (Local Interpretable Model-agnostic Explanations)**:
   - Explains **individual predictions** by approximating the model locally using interpretable models.
   - Helps understand which features most influenced a specific prediction (e.g., why a patient is predicted to have heart disease).

4. **DiCE (Diverse Counterfactual Explanations)**:
   - Provides **counterfactual explanations** to show how changes to feature values can flip a model’s prediction (e.g., lowering cholesterol to avoid a disease prediction).

---

## 🛠️ How to Use

### 1. **Training the Model**:
   - The model is trained on the Cleveland Heart Disease dataset using **XGBoost**.

### 2. **Explanation of Predictions**:
   - **SHAP** and **LIME** generate visualizations of feature importance for individual predictions.
   - **DiCE** shows **counterfactuals**, indicating how features would need to change to alter the model's prediction (e.g., how to avoid being predicted as having heart disease).

---

## 📊 Example Outputs

- **SHAP**: 
   - A summary plot visualizing the **feature importance** across the dataset.
   - Force plots for **local explanations**, showing how features contributed to a specific prediction.

- **LIME**: 
   - A strip plot indicating the **range of feature values** for a given prediction and its impact on the model’s outcome.

- **DiCE**:
   - A **counterfactual explanation table** showing what changes would be needed in features like cholesterol, age, or exang (exercise induced angina) to flip the prediction from having heart disease to not having it.

---

## 📦 Requirements

To run this project, install the necessary libraries using pip:

```bash
pip install xgboost shap lime dice-ml pandas numpy scikit-learn matplotlib seaborn
