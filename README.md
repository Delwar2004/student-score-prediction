# 🎓 Student Score Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange)
![Regression](https://img.shields.io/badge/Task-Regression-success)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

An end-to-end Machine Learning regression project developed. The objective is to predict students' examination scores using various regression techniques while following a complete machine learning workflow—from exploratory data analysis (EDA) to model evaluation and proper data leakage prevention.

---

# 📌 Project Overview

Student academic performance depends on multiple factors, including study habits, attendance, previous academic achievement, and lifestyle. This project investigates how effectively these factors can predict students' examination scores.

The project begins with a **baseline Linear Regression model** using only **Hours_Studied**, then progressively evaluates:

- Expanded feature sets
- Polynomial Regression
- Full-feature Linear Regression
- Proper outlier handling
- Data leakage prevention

The goal is not only to build a predictive model but also to understand which factors contribute most to student performance.

---

# 🎯 Objectives

- Perform comprehensive Exploratory Data Analysis (EDA)
- Build a baseline Linear Regression model
- Compare Polynomial Regression (Degree 2 & Degree 3)
- Evaluate different feature combinations
- Investigate the impact of outlier removal
- Demonstrate proper preprocessing without data leakage
- Compare model performance using multiple evaluation metrics

---

# 📂 Dataset

**Dataset:** Student Performance Factors (Kaggle)

### Dataset Summary

| Property | Value |
|-----------|--------|
| Samples | 6,607 |
| Features | 19 |
| Target Variable | Exam_Score |
| Problem Type | Supervised Regression |

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

---

# 📊 Machine Learning Workflow

```
Dataset

↓

Data Quality Assessment

↓

Exploratory Data Analysis (EDA)

↓

Data Preprocessing

↓

Feature Selection

↓

Train-Test Split

↓

Linear Regression

↓

Polynomial Regression

↓

Feature Comparison

↓

Outlier Analysis

↓

Model Evaluation

↓

Research Findings
```

---

# 📈 Exploratory Data Analysis

The following analyses were performed before model development:

- Missing Value Analysis
- Duplicate Detection
- Data Type Verification
- Histograms
- Boxplots
- Count Plots
- Correlation Heatmap
- Scatter Plots
- Outlier Detection (IQR Method)

---

# 🤖 Models Implemented

## 1. Baseline Linear Regression

**Feature Used**

- Hours_Studied

This model serves as the baseline required by the internship task.

---

## 2. Polynomial Regression

Two polynomial models were evaluated:

- Degree 2
- Degree 3

The objective was to investigate whether nonlinear transformations improve prediction performance.

---

## 3. Expanded Feature Model

Features:

- Hours_Studied
- Attendance
- Previous_Scores
- Sleep_Hours
- Tutoring_Sessions
- Physical_Activity

---

## 4. Full Feature Model

Uses all available numerical and encoded categorical features.

---

# 📊 Model Performance

| Model | Features | MAE | RMSE | R² |
|------|------|------|------|------|
| Baseline Linear Regression | Hours_Studied | **2.448** | **3.295** | **0.232** |
| Polynomial Regression (Degree 2) | Hours_Studied | **2.445** | **3.293** | **0.233** |
| Polynomial Regression (Degree 3) | Hours_Studied | **2.445** | **3.293** | **0.233** |
| Expanded Feature Set | 6 Features | **1.266** | **2.251** | **0.642** |
| Full Feature Set | All Features | **0.452** | **1.804** | **0.770** |

---

# 🔍 Key Findings

- **Hours_Studied** alone is a moderate predictor of student performance, explaining approximately **23%** of the variance in exam scores.
- Polynomial Regression provides **minimal improvement**, indicating that the relationship between study hours and exam scores is largely linear.
- Incorporating additional academic and behavioral factors significantly improves prediction accuracy.
- The **Full Feature Model** achieved the highest predictive performance with an **R² score of 0.770**.
- Proper outlier handling demonstrated that removing outliers did **not** provide any meaningful improvement for this dataset.

---

# ⚠️ Preventing Data Leakage

A dedicated experiment was conducted to demonstrate proper preprocessing practices.

Outlier thresholds were calculated **only from the training set** using the Interquartile Range (IQR) method.

This prevents information from the testing data from influencing preprocessing decisions.

> Incorrect preprocessing using the entire dataset can artificially inflate evaluation metrics and produce misleadingly high R² scores.

---

# 📈 Research Insights

This project demonstrates several important machine learning concepts:

- Importance of establishing a baseline model
- Feature engineering significantly improves predictive performance
- Polynomial models do not always outperform linear models
- More features do not always imply overfitting when they provide meaningful information
- Proper preprocessing is essential for unbiased model evaluation
- Preventing data leakage is a critical aspect of real-world machine learning pipelines

---

# 📁 Repository Structure

```
student-score-prediction/

│

├── data/
│   └── StudentPerformanceFactors.xls
│
├── notebooks/
│   └── Student_Score_Prediction_ML.ipynb
│
├── images/
│
├── README.md
│
├── requirements.txt
│
└── LICENSE
```

---

# 🚀 Future Improvements

Future work may include:

- Ridge Regression
- Lasso Regression
- Decision Tree Regression
- Random Forest Regression
- XGBoost Regression
- Cross Validation
- Hyperparameter Optimization
- SHAP Explainability
- Model Deployment using Streamlit or Flask

---

# 📚 Learning Outcomes

Through this project, I gained practical experience in:

- End-to-end Machine Learning workflow
- Data preprocessing
- Exploratory Data Analysis
- Feature Engineering
- Regression Modeling
- Model Evaluation
- Outlier Analysis
- Data Leakage Prevention
- Research-style experimentation

---

# 👨‍💻 Author

**MD DELWAR HUSEN**

B.Sc. in Information and Communication Engineering (ICE)

Bangladesh University of Professionals (BUP)

---

# ⭐ If you found this project useful, consider giving it a star!
