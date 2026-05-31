
<div align="center">

# 🏥 Healthcare Readmission Analytics Dashboard

### Predicting 30-Day Hospital Readmissions Using Machine Learning, Explainable AI & Business Intelligence

<img src="https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python"/>
<img src="https://img.shields.io/badge/Power_BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi"/>
<img src="https://img.shields.io/badge/XGBoost-Best_Model-success?style=for-the-badge"/>
<img src="https://img.shields.io/badge/SHAP-Explainable_AI-red?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Healthcare-Analytics-green?style=for-the-badge"/>

---

### 🚀 End-to-End Healthcare Analytics Solution

Machine Learning • Predictive Modeling • Explainable AI • Clinical Risk Stratification • Power BI

</div>

---

# 📑 Table of Contents

- Executive Summary
- Business Problem
- Dataset Overview
- Project Architecture
- Feature Engineering
- Machine Learning Models
- Dashboard Overview
- Explainable AI Analysis
- Key Findings
- Business Recommendations
- Technology Stack
- Repository Structure
- Future Improvements

---

# 🎯 Executive Summary

Healthcare systems face significant financial and operational burdens due to avoidable hospital readmissions.

This project develops an end-to-end predictive analytics framework capable of identifying diabetic patients at risk of 30-day readmission while providing explainable insights into the underlying clinical drivers.

---

## 🔥 Project Highlights

| KPI | Value |
|------|------|
| Patients Analyzed | 101,763 |
| Readmission Rate | 11.16% |
| Average Length of Stay | 4.40 Days |
| Average Medications | 16.02 |
| Best Model | XGBoost |
| ROC-AUC | 0.687 |
| PR-AUC | 0.237 |
| Recall | 58.2% |

---

# 💼 Business Problem

Hospital readmissions negatively impact:

- Patient outcomes
- Healthcare costs
- Resource allocation
- Hospital performance metrics

Healthcare providers require predictive systems capable of identifying high-risk patients before discharge.

---

# 📊 Dataset Overview

## Source

UCI Diabetes 130-US Hospitals Dataset

## Scope

| Metric | Value |
|----------|----------|
| Hospitals | 130 |
| Encounters | 101,763 |
| Domain | Healthcare |
| Target | Readmitted <30 Days |
| Population | Diabetic Patients |

---

# ⚙️ Project Architecture

```text
Raw Hospital Data
        │
        ▼
 Data Cleaning
        │
        ▼
 Feature Engineering
        │
        ▼
 Model Development
        │
 ┌───────────────┐
 │ Logistic Reg. │
 │ Random Forest │
 │   XGBoost     │
 └───────────────┘
        │
        ▼
 Model Evaluation
        │
        ▼
 SHAP Explainability
        │
        ▼
 Power BI Dashboard
        │
        ▼
 Business Recommendations
````

---

# 🧠 Feature Engineering

Several healthcare-specific features were engineered to improve predictive performance.

| Feature                  | Purpose                       |
| ------------------------ | ----------------------------- |
| Utilization Score        | Healthcare usage intensity    |
| Frequent Admitter Flag   | Repeat admission history      |
| Medication Burden        | Treatment complexity          |
| Diagnosis Groups         | Clinical categorization       |
| Length of Stay Flag      | Hospitalization severity      |
| Diabetes Medication Flag | Treatment adherence indicator |

---

# 🤖 Machine Learning Models

## Models Evaluated

| Model               | Accuracy | Precision | Recall | F1   | ROC-AUC | PR-AUC |
| ------------------- | -------- | --------- | ------ | ---- | ------- | ------ |
| Logistic Regression | 0.67     | 0.18      | 0.58   | 0.28 | 0.68    | 0.22   |
| Random Forest       | 0.73     | 0.20      | 0.49   | 0.29 | 0.68    | 0.22   |
| XGBoost             | 0.67     | 0.19      | 0.58   | 0.28 | 0.69    | 0.24   |

---

## 🏆 Best Performing Model

# XGBoost

| Metric            | Score |
| ----------------- | ----- |
| ROC-AUC           | 0.687 |
| PR-AUC            | 0.237 |
| Recall            | 58.2% |
| Precision         | 19.1% |
| Optimal Threshold | 0.53  |

---

# 📈 Dashboard Overview

---

## 📍 Page 1 — Executive Summary

### Purpose

Provides a high-level overview of the patient population and readmission statistics.

### KPIs

* Total Patients
* Readmission Rate
* Average Length of Stay
* Average Medications

### Visualizations

* Patient Age Distribution
* Gender Distribution
* Readmission Distribution

```markdown
![Executive Summary](images/executive_summary.png)
```

---

## 📍 Page 2 — Readmission Risk Analysis

### Purpose

Identify patient segments most vulnerable to readmission.

### Visualizations

* Readmission Risk by Utilization Level
* Readmission Rate by Medication Burden
* Readmission Rate by Age Group
* Readmission Rate by Diagnosis Group

```markdown
![Risk Analysis](images/risk_analysis.png)
```

---

## 📍 Page 3 — Predictive Model Performance

### Purpose

Compare machine learning models and evaluate predictive effectiveness.

### Visualizations

* ROC Curves
* Precision Recall Curves
* Model Comparison Table
* Performance KPIs

```markdown
![Model Performance](images/model_performance.png)
```

---

## 📍 Page 4 — Explainability & Business Recommendations

### Purpose

Provide transparency into model predictions and convert insights into business actions.

### Visualizations

* SHAP Feature Importance
* SHAP Summary Plot
* Key Findings
* Strategic Recommendations

```markdown
![Explainability](images/explainability.png)
```

---

# 🔬 Explainable AI Analysis

## Top Clinical Drivers of Readmission

| Rank | Clinical Driver           |
| ---- | ------------------------- |
| 1    | Previous Inpatient Visits |
| 2    | Discharge Disposition     |
| 3    | Utilization Score         |
| 4    | Circulatory Diagnosis     |
| 5    | Number of Diagnoses       |
| 6    | Length of Stay            |
| 7    | Medication Count          |
| 8    | Lab Procedures            |
| 9    | Frequent Admitter         |
| 10   | Age                       |

---

# 📌 Key Findings

## Clinical Insights

✔ Previous inpatient admissions were the strongest predictor of future readmission.

✔ Utilization history outperformed demographic variables.

✔ Circulatory disease patients demonstrated elevated risk.

✔ Medication burden significantly contributed to readmission likelihood.

✔ High-risk patients exhibited repeated healthcare utilization patterns.

---

## Machine Learning Insights

✔ XGBoost achieved the highest ROC-AUC and PR-AUC.

✔ Threshold optimization improved sensitivity to high-risk patients.

✔ Explainability outputs aligned with clinical intuition.

✔ Feature importance highlighted actionable intervention points.

---

# 🚀 Business Recommendations

## 1. Post-Discharge Follow-Up Programs

Prioritize patients with prior inpatient admissions.

---

## 2. High Utilization Care Management

Develop targeted intervention pathways for high-utilization patients.

---

## 3. Medication Reconciliation

Perform discharge medication reviews to reduce complications.

---

## 4. Chronic Disease Monitoring

Increase surveillance of circulatory and respiratory patients.

---

## 5. Predictive Risk Scoring

Deploy the model into operational workflows for proactive intervention.

---

# 🛠️ Technology Stack

## Data Science

* Python
* Pandas
* NumPy

## Machine Learning

* Scikit-Learn
* XGBoost

## Explainability

* SHAP

## Visualization

* Power BI
* Matplotlib
* Seaborn

## Environment

* Jupyter Notebook

---

# 📂 Repository Structure

```text
Healthcare-Readmission-Analytics
│
├── data
│
├── notebooks
│   ├── 01_Data_Cleaning.ipynb
│   ├── 02_Feature_Engineering.ipynb
│   ├── 03_Model_Development.ipynb
│   ├── 04_Model_Evaluation.ipynb
│   └── 05_SHAP_Analysis.ipynb
│
├── models
│
├── dashboard
│   └── Healthcare_Readmission_Dashboard.pbix
│
├── images
│   ├── executive_summary.png
│   ├── risk_analysis.png
│   ├── model_performance.png
│   └── explainability.png
│
├── README.md
│
└── requirements.txt
```

---

# 🔮 Future Enhancements

* Real-Time Readmission Risk Scoring
* Azure Deployment
* Streamlit Application
* Automated Model Retraining
* Clinical Decision Support Integration

---

# 👩‍💻 Author

## Shaik Afsar Jahan 

Healthcare Analytics • Data Science • Machine Learning • Business Intelligence

---

<div align="center">

### ⭐ If you found this project useful, consider starring the repository.

### Thank you for visiting!

</div>
```
