# 🏥 CODTECH IT Solutions — Data Analytics Internship
## Task 2: Predictive Analysis Using Machine Learning
### Project: Heart Attack Risk Prediction

<div align="center">

![Python](https://img.shields.io/badge/Python-3.14.5-blue?style=for-the-badge&logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?style=for-the-badge)
![Pandas](https://img.shields.io/badge/Pandas-Analysis-green?style=for-the-badge&logo=pandas)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-red?style=for-the-badge&logo=jupyter)
![Healthcare](https://img.shields.io/badge/Domain-Healthcare-blueviolet?style=for-the-badge)

</div>

---

## 📋 Internship Details

| Field | Details |
|-------|---------|
| **Name** | Ayush Kumar Singh |
| **Company** | CODTECH IT Solutions Pvt. Ltd. |
| **Intern ID** | CITS527 |
| **Domain** | Data Analytics |
| **Duration** | 4 Weeks |
| **Mentor** | Neela Santhosh Kumar |

---

## 🎯 Task Objective

> Build a **Machine Learning Classification Model** to predict whether a patient is at **High Risk or Low Risk** of a heart attack based on 17 clinical and lifestyle features from a large dataset of **50,000 patients**.

This project demonstrates the complete ML pipeline — feature selection, preprocessing, model training with 3 algorithms, evaluation using Accuracy + ROC-AUC, and prediction on new patient data.

---

## 🗂️ Project Structure

```
Task-2-Predictive-Analysis-ML/
│
├── 📓 predictive_analysis.ipynb   ← Main Jupyter Notebook
├── 📊 heart_attack_data.csv       ← Dataset (50,000 patients)
└── 📝 README.md
```

---

## 📊 Dataset Description

**File:** `heart_attack_data.csv`
**Records:** 50,000 rows | **Columns:** 19

| Column | Type | Description |
|--------|------|-------------|
| `patient_id` | int | Unique patient ID |
| `age` | int | Patient age (25–80) |
| `gender` | str | Male / Female |
| `chest_pain_type` | str | typical_angina / atypical_angina / non_anginal / asymptomatic |
| `resting_bp` | int | Resting blood pressure (mmHg) |
| `cholesterol` | int | Serum cholesterol (mg/dL) |
| `fasting_blood_sugar` | int | FBS > 120 mg/dL (1=Yes, 0=No) |
| `resting_ecg` | str | ECG results: normal / st_t_abnormality / left_ventricular_hypertrophy |
| `max_heart_rate` | int | Maximum heart rate achieved |
| `exercise_angina` | int | Exercise-induced angina (1=Yes, 0=No) |
| `st_depression` | float | ST depression induced by exercise |
| `st_slope` | str | Slope of peak exercise ST segment |
| `num_major_vessels` | int | Number of major vessels colored by fluoroscopy (0–3) |
| `thalassemia` | str | normal / fixed_defect / reversible_defect |
| `smoking` | int | Smoker (1=Yes, 0=No) |
| `diabetes` | int | Diabetic (1=Yes, 0=No) |
| `family_history` | int | Family history of heart disease (1=Yes, 0=No) |
| `obesity` | int | Obese (1=Yes, 0=No) |
| `heart_attack_risk` | int | **Target** — High Risk (1) / Low Risk (0) |

---

## 🛠️ Tools & Libraries Used

| Library | Purpose |
|---------|---------|
| **Pandas** | Data loading and manipulation |
| **NumPy** | Numerical operations |
| **Matplotlib & Seaborn** | Visualisation and EDA |
| **Scikit-Learn** | ML models, preprocessing, evaluation |

---

## 🤖 ML Models Trained

| Model | Type | Key Strength |
|-------|------|-------------|
| **Logistic Regression** | Linear Classification | Fast, interpretable baseline |
| **Random Forest** | Ensemble (Bagging) | Handles non-linearity, feature importance |
| **Gradient Boosting** | Ensemble (Boosting) | Best accuracy, handles complex patterns |

---

## 🔧 How to Run

### Step 1 — Install dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Step 2 — Open the notebook
```bash
jupyter notebook predictive_analysis.ipynb
```

### Step 3 — Run all cells
Go to **Kernel → Restart & Run All**

---

## 📈 Model Results

| Model | Accuracy | AUC Score |
|-------|----------|-----------|
| Logistic Regression | ~75–80% | ~0.82 |
| Random Forest | ~88–92% | ~0.95 |
| Gradient Boosting | ~89–93% | ~0.96 |

---

## 🔑 Key Insights

1. **ST slope (downsloping)** and **num_major_vessels** are the strongest predictors of heart attack risk
2. **Thalassemia (reversible defect)** is a critical clinical indicator
3. **Age > 55** significantly increases heart attack probability
4. **Smoking + Diabetes** combination almost doubles the risk
5. **Exercise-induced angina** is a strong positive risk indicator
6. **Gradient Boosting** gives the best accuracy and AUC among all 3 models
7. **Logistic Regression** provides the fastest training with reasonable accuracy as a baseline

---

## 📸 Output Plots Generated

Running the notebook generates these plots automatically:

- `eda_plots.png` — 6-panel EDA dashboard
- `correlation_heatmap.png` — Feature correlation matrix
- `confusion_matrices.png` — Confusion matrices for all 3 models
- `roc_model_comparison.png` — ROC curves + accuracy comparison
- `feature_importance.png` — Random Forest feature importance chart

---

<div align="center">
<b>CODTECH IT Solutions Pvt. Ltd.</b> — Data Analytics Internship — Task 2
</div>
