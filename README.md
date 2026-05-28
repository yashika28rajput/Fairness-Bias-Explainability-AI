# Fairness-Bias-Explainability-AI
Responsible AI project analyzing fairness, bias, and explainability in COMPAS recidivism prediction using CatBoost, SHAP, LIME, and Fairlearn.
# Fairness, Bias and Explainability Analysis of COMPAS Recidivism Prediction Model

## Project Overview

This project focuses on Responsible Artificial Intelligence (Responsible AI) by analyzing fairness, bias, and explainability in machine learning models.

The project uses the COMPAS Recidivism Dataset to predict whether a defendant is likely to reoffend within two years while evaluating ethical concerns related to demographic bias and algorithmic fairness.

The study combines Machine Learning, Explainable AI (XAI), and Fairness Analysis techniques.

---

## Objectives

- Analyze fairness and bias in AI systems
- Evaluate demographic bias across race and gender
- Explain model predictions using SHAP and LIME
- Measure fairness metrics using Fairlearn
- Improve transparency and ethical AI understanding

---

## Dataset

### COMPAS Recidivism Dataset
Source:
- ProPublica COMPAS Dataset

### Target Variable
- `two_year_recid`
  - 1 → Reoffended within 2 years
  - 0 → Did not reoffend

### Sensitive Attributes
- Race
- Sex

---

## Technologies & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- CatBoost
- SHAP
- LIME
- Fairlearn

---

## Machine Learning Model

### CatBoost Classifier

The CatBoost model was selected because:

- Native handling of categorical features
- Better performance on structured/tabular datasets
- Strong compatibility with SHAP explainability
- Reduced overfitting through symmetric trees

---

## Explainable AI Techniques

### SHAP (SHapley Additive Explanations)

Used for:
- Global feature importance
- Feature contribution analysis
- SHAP summary plots
- SHAP beeswarm plots

### LIME (Local Interpretable Model-Agnostic Explanations)

Used for:
- Local prediction explainability
- Individual prediction analysis
- Feature contribution interpretation

---

## Fairness Analysis

The project evaluates fairness across sensitive demographic groups.

### Fairness Metrics Used

- Demographic Parity Difference
- Equalized Odds Difference

### Bias Evaluation

Bias was analyzed across:
- Race groups
- Gender groups

---

## Model Performance

### Final Results

- Accuracy: ~67%
- ROC-AUC Score: ~0.71

### Classification Metrics

- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## Important Findings

### Most Influential Features

- priors_count
- age
- race
- decile_score
- score_text

### Ethical Concerns

- Historical criminal justice bias may propagate into AI systems
- Sensitive attributes may indirectly influence predictions
- Accuracy differed across demographic groups

---

## Visualizations Included

- Confusion Matrix
- Feature Importance Graph
- SHAP Summary Plot
- SHAP Beeswarm Plot
- ROC Curve
- Correlation Heatmap
- Race Distribution
- Gender Distribution
- Accuracy by Race
- Accuracy by Gender

---

## Bias Mitigation Recommendations

- Balanced demographic representation
- Removal of proxy variables
- Fairness-aware learning
- Human oversight
- Continuous fairness auditing

---

## Project Structure

```bash
Fairness-and-Explainability-in-AI/
│
├── notebooks/
├── src/
├── results/
├── screenshots/
├── report/
├── README.md
├── requirements.txt
└── LICENSE
```

---

## How to Run

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run the Project

```bash
python fairness_analysis.py
```

---

## Future Improvements

- Adversarial Debiasing
- Explainable Deep Learning
- Real-time fairness monitoring
- Bias mitigation pipelines
- Interactive fairness dashboards

---

## Author

Yashika Rajput
