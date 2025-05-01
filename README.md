# Patient Readmission Prediction and Dashboard

This project analyzes hospital patient records to identify key factors influencing readmission using data science and business intelligence. It combines **EDA**, **machine learning with SHAP AI explainability**, and a **Power BI dashboard** to deliver a full end-to-end analysis pipeline.

---

## 📚 Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [EDA & ML Modeling](#eda--ml-modeling)
- [SHAP Explainability](#shap-explainability)
- [Power BI Dashboard](#power-bi-dashboard)
- [Key Insights](#key-insights)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)

---

## 🎯 Overview

Hospital readmissions increase costs and indicate care gaps. This project uses a real-world dataset to:
- Analyze patient demographics and diagnoses related to readmission
- Predict readmission likelihood using **Logistic Regression**
- Explain predictions using **SHAP (AI Explainability)**
- Visualize insights in an interactive **Power BI dashboard**

---

## 🗂 Dataset

- **Source**: [UCI Diabetes 130-US Hospitals Dataset](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008)
- **Size**: ~100,000 patient records
- **Fields**: demographics, hospital admissions, diagnosis codes, medications, procedures, lab results, readmission flags

---

## 🧪 EDA & Machine Learning

- Cleaned missing values (`?` → `Unknown`)
- Explored demographics, procedures, and diagnosis trends
- Built a **Logistic Regression** model to predict readmission
- Evaluated performance with **accuracy, precision, recall, F1-score**

### 📸 Sample Outputs:
![Age Distribution](images/Python_Code_outputs/eda_age_distribution.png)
![Readmission Bar](images/Python_Code_outputs/readmission_bar.png)
![Model Metrics](images/Python_Code_outputs/ML model_metrics.png)
![Primary Diagnosis](images/Python_Code_outputs/Top 10 Primary Diagnosis.png)

---
## 🤖 SHAP AI Explainability

**SHAP** (SHapley Additive exPlanations) was used to interpret model predictions and identify the most impactful features.

### 📊 SHAP Summary Plot:
![SHAP Summary](images/Python_Code_outputs/shap AI_summary.png)

---

## 📊 Power BI Dashboard

Built a 3-page Power BI dashboard to visually explore readmission trends, patient demographics, and diagnosis breakdowns.

### 📸 Dashboard Screenshots:

#### 🧩 Page 1: Readmission Overview
- Total patients
- Readmission breakdown (Yes/No)
- Avg. time in hospital

![Page 1](images/Readmission_overview.png)

#### 👥 Page 2: Demographics Analysis
- Age vs Readmission
- Gender & Race distribution
- Slicers for Race, Gender, Admission Type

![Page 2](images/demographic Analysis.png)

#### 🏥 Page 3: Diagnoses & Specialties
- Top 10 primary diagnosis codes
- Readmission by medical specialty
- A1C Result and DiabetesMed insights

![Page 3](images/Diagnosis and Specialty Analysis.mp4)

---

## 🔍 Key Insights

- Patients with multiple **inpatient visits**, **diagnoses**, and **emergency encounters** are most likely to be readmitted.
- Most readmitted patients fall in the **60–80 age range**.
- Departments like **Cardiology** and **Internal Medicine** show higher readmission counts.
- **SHAP** showed that `NUMBER_INPATIENT`, `NUMBER_DIAGNOSES`, and `NUMBER_EMERGENCY` were the most impactful features.

---

## 🛠 Technologies Used

- **Python**: Pandas, Scikit-learn, SHAP, Matplotlib, Seaborn
- **Power BI**: Dashboard creation & data storytelling
- **Jupyter Notebook**: Analysis & model development
- **Git & GitHub**: Version control & project hosting

---

## ▶️ How to Run

1. Clone the repository:
   bash
   git clone https://github.com/Maitreyie99/patient-readmission-analysis.git
2. Navigate to project folder:
  bash
  cd patient-readmission-analysis
3. Open and run notebooks/readmission_model.ipynb to reproduce the analysis.
4. Open dashboard/Patient_Readmission_Dashboard.pbix in Power BI Desktop to   explore the dashboard.
