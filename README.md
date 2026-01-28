# Clinical Heart Disease Study: Classification, Clustering & Regression

##  Research Objective
To develop a multi-dimensional diagnostic support tool using the Heart Failure Prediction Dataset. This project explores patient data through three distinct computational lenses to identify severity, risk profiles, and biomarker correlations.

## Technical Implementation

### 1. Classification (Disease Severity)
* **Goal:** Predict heart disease severity on a scale of 0 (No Disease) to 4 (High Severity).
* **Algorithm Performance:** Successfully implemented **Random Forest** to capture non-linear patterns.
* **Key Insight:** I discovered that no single clinical feature (like cholesterol) was a strong predictor alone. The model relied on **"weak signals"**—subtle combinations of all features—which is where Random Forest outperformed simpler models like k-NN.
* **Interpretability:** I documented the critical trade-off between the high accuracy of "Black Box" models vs. the explainability of Decision Trees, essential for medical adoption.



### 2. Clustering (Patient Risk Profiling)
* **Goal:** Group patients based on clinical similarities using Unsupervised Learning.
* **Algorithm:** **K-Means Clustering**.
* **Clinical Application:** Identified distinct "High-Risk" vs. "Low-Risk" subgroups. This allows healthcare providers to focus early intervention strategies on specific patient clusters that share similar physiological markers, regardless of their diagnosis label.



### 3. Regression (Biomarker Analysis)
* **Goal:** Predict cholesterol levels based on patient age.
* **Statistical Finding:** The model yielded a **low R² score of 0.005**, indicating that age alone is not a reliable predictor of cholesterol in this dataset.
* **Critical Conclusion:** This "negative result" demonstrates that clinical predictions must move beyond simple demographic heuristics and incorporate a wider range of features (genetics, diet, and lifestyle) to be accurate.



## 📊 Technical Stack
* **Language:** Python (Jupyter)
* **Libraries:** Scikit-learn, Pandas, Seaborn, Matplotlib.
* **Data Pipeline:** Encoding -> Feature Scaling -> Model Selection -> Evaluation (RMSE, MAE).
