# Predicting Manufacturing Efficiency Using Sensor and Network Data

**Author:** Eric Meyer  
**Capstone Project – MS in Data Analytics, Northwest Missouri State University**  
[Overleaf Report](https://www.overleaf.com/read/ytnsxycrkbwr#20b809)  
[Dataset Source – Kaggle](https://www.kaggle.com/datasets/ziya07/intelligent-manufacturing-dataset)

---

## Project Summary

This capstone project investigates the use of machine learning to classify manufacturing process efficiency based on real-time sensor readings and network performance data. The goal was to assign each production observation to one of three efficiency levels **Low**, **Medium**, or **High** to support process monitoring and improvement in a smart manufacturing environment.

The dataset includes anonymized operational features such as temperature, vibration, operation mode, and connectivity metrics. After data cleaning and exploration, a Random Forest classification model was used to make predictions.

---

## Project Objectives

- Clean and preprocess sensor and network data for modeling.
- Use EDA to explore key variables influencing production efficiency.
- Train and evaluate classification model (Random Forest).
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

---

## Key Insights

- **Sensor Data Matters:** Variables such as production speed, air temperature, and process temperature were strong predictors of efficiency.
- **Class Imbalance is Real:** Most data points were labeled “Low,” making it hard for models to learn meaningful patterns in “Medium” and “High” classes.
- **Random Forest Wins:** This model offered the best trade-off between accuracy, interpretability, and training time.

---

## Opportunities for Future Work

- Apply other oversampling methods to address class imbalance.
- Expand to **regression models** to predict continuous efficiency scores instead of classes.
- Integrate the model into real-time **MES (Manufacturing Execution Systems)** for operational use.
  
---

## Final Thoughts

This project showcases how data science can unlock hidden insights from manufacturing environments and provide practical tools for process improvement. With more balanced data and real-time integration, these models have the potential to enhance decision-making and optimize factory performance on a large scale.

---