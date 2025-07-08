# 🩺 WiDS Datathon 2024 – Metastatic Diagnosis Period Prediction

This repository contains exploratory data analysis (EDA), feature exploration, and modeling strategies developed for the **WiDS Datathon 2024 Challenge 2**. The challenge focuses on predicting the period in which patients are diagnosed with metastatic cancer using diverse clinical, demographic, and environmental data.

---

## 📌 Problem Statement

The goal of this project is to build a predictive model that estimates a patient’s **Metastatic Diagnosis Period**, based on a wide range of features including medical history, personal demographics, environmental factors, and social determinants of health.

This problem is vital in enhancing early diagnosis, planning interventions, and improving cancer treatment outcomes in real-world clinical settings.

---

## 📊 Dataset Overview

The dataset provided by the competition includes **18,819** records and approximately **152 features**, split into training and test sets.

- 🔍 **Data Includes:**
  - **Patient Characteristics:** Age, race, BMI, zip code
  - **Medical Records:** Diagnosis codes (e.g., breast cancer, metastatic cancer), treatment history
  - **Geodemographics:** Income, education, housing, race, poverty levels by zip code
  - **Climate Data:** Region-level environmental information tied to patient locations

📂 **Source**:  
[WiDS Datathon 2024 – Challenge 2 (Kaggle)](https://www.kaggle.com/competitions/widsdatathon2024-challenge2/data)

---

## 🔍 Key Explorations and Analysis

### 1. 📌 Data Inspection
- Overview of null values, data types, and unique value counts
- Distribution analysis for categorical and numerical features
- Detection of duplicate records and skewed distributions

### 2. 🧹 Data Cleaning & Preprocessing
- **Missing Value Treatment:**
  - Categorical → Mode imputation
  - Numerical → Median/Mean based on skewness
- **Outlier Detection & Removal:**
  - IQR-based filtering on sensitive features
- **Feature Grouping & Engineering:**
  - Combined income brackets into `Low`, `Medium`, `High`
  - Grouped age into bins: `Under_20`, `20s_to_40s`, `50s_to_70s`
  - Derived meaningful variables for modeling

---

## 💡 Notable Insights

- More than 60% of patients have missing BMI and race data — filled carefully to avoid model bias.
- Income and age show predictive strength for the metastatic diagnosis timeline.
- Seasonal and regional environmental features vary widely and affect cancer progression patterns.
- Post-cleaning, the dataset was reduced to ~3,293 quality samples for modeling.

---

## 📈 Tools & Technologies

- Python
- Jupyter Notebook
- pandas, numpy
- seaborn, matplotlib
- scikit-learn (for imputation and preprocessing)

---

## 🧠 Future Work

- Implement advanced regression models (XGBoost, RandomForest)
- Hyperparameter tuning and validation
- Incorporate interaction effects between regional climate and income
- Evaluate model generalizability across subgroups

---

## 👥 Team Contributors

- **Aishwarya Metri**
- **Ratan Badiger**
- **Roopa Boodi**
- **Varad B**

---

## 📜 License & Data Policy

This project is solely for educational and research purposes.  
Data used in this project is subject to Kaggle’s competition terms:  
[WiDS 2024 Challenge 2 Rules](https://www.kaggle.com/competitions/widsdatathon2024-challenge2/rules)

---

## 🙌 Acknowledgments

- **WiDS Conference & Datathon Team**  
- **Stanford University & Kaggle** for organizing and supporting the challenge  
- All contributors to the public datasets and documentation



