# Predicting Manufacturing Efficiency Using Sensor and Network Data

**Author:** Eric Meyer  
**Capstone Project – MS in Data Analytics, Northwest Missouri State University**  
[Overleaf Report](https://www.overleaf.com/read/ytnsxycrkbwr#20b809)  
[Dataset Source – Kaggle](https://www.kaggle.com/datasets/ziya07/intelligent-manufacturing-dataset)

---

## Project Summary

This capstone project investigates the use of machine learning to classify manufacturing process efficiency based on real-time sensor readings and network performance data. The goal was to assign each production observation to one of three efficiency levels—**Low**, **Medium**, or **High**—to support process monitoring and improvement in a smart manufacturing environment.

The dataset includes anonymized operational features such as temperature, vibration, operation mode, and connectivity metrics. After data cleaning and exploration, several classification models were tested. **XGBoost** and **Random Forest** were the top performers, with **XGBoost achieving an accuracy of 77.3%**.

---

## Project Objectives

- Clean and preprocess sensor and network data for modeling.
- Use EDA to explore key variables influencing production efficiency.
- Train and evaluate classification models (Logistic Regression, Random Forest, XGBoost).
- Assess model performance using accuracy, F1-score, and confusion matrix.
- Visualize key results including feature importance and class distributions.

---

## Tools & Technologies

- Python (pandas, scikit-learn, seaborn, matplotlib)
- Jupyter Notebooks
- Git & GitHub
- Overleaf (LaTeX)
- VS Code

---

## Model Performance Summary

**Model:** Random Forest 
**Test Accuracy:** 77.3%  
**F1-Score (Low Efficiency):** 0.87  
**Class Imbalance Observed:** Majority of samples labeled “Low” efficiency

### Classification Report:

| Class     | Precision | Recall | F1-Score | Support |
|-----------|-----------|--------|----------|---------|
| High      | 0.00      | 0.00   | 0.00     | 625     |
| Low       | 0.77      | 1.00   | 0.87     | 15,464  |
| Medium    | 0.00      | 0.00   | 0.00     | 3,911   |
| **Overall Accuracy** | - | - | **0.773** | 20,000 |

