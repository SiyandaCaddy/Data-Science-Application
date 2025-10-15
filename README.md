# Data-Science-Application
# 🎓 Student Performance Analytics
 

---

## Project Overview

This project applies **Data Science and Machine Learning** techniques to analyze and predict student academic performance.  
It uses data from the **UCI Machine Learning Repository – Student Performance Dataset**, which contains detailed academic, demographic, and social attributes of secondary school students from Portugal.

The aim is to develop a **classification model** that can predict whether a student will **pass or fail** based on their performance indicators such as study time, previous grades, absences, and family background.

---

## Oobjectives

1. Preprocess and clean the dataset to ensure quality and consistency.  
2. Perform Exploratory Data Analysis (EDA) to identify key factors affecting performance.  
3. Train machine learning models (Logistic Regression, Random Forest, and XGBoost).  
4. Evaluate models using accuracy, precision, recall, F1-score, and ROC-AUC metrics.  
5. Identify important predictors influencing academic success.  
6. Provide visual insight and interpret results to support educational decision-making.

---

## 📂 Dataset

**Source:**  
[UCI Machine Learning Repository – Student Performance Data Set](https://archive.ics.uci.edu/ml/datasets/student+performance)

**Files Used:**  
- `student-mat.csv` – Mathematics student records  
- `student-por.csv` – Portuguese language student records  

Both datasets were merged into a single dataframe for a more comprehensive analysis.  
If only one dataset is available, the notebook automatically adjusts and continues with that file.

**Attributes include:**  
- Demographic: `sex`, `age`, `address`, `family_size`  
- Academic: `studytime`, `failures`, `G1`, `G2`, `G3`  
- Social: `internet`, `romantic`, `famsup`, `schoolsup`  
- Target Variable: Final grade (`G3`) converted into binary labels (Pass = 1, Fail = 0)  

---

## ⚙️ Methodology

1. **Data Upload & Merge:**  
   The Colab notebook allows uploading one or both CSV files and merges them automatically.

2. **Data Preprocessing:**  
   - Encoding categorical variables  
   - Scaling numerical features  
   - Handling missing values (none in this dataset)  
   - Creating binary target variable (`pass`)

3. **Exploratory Data Analysis (EDA):**  
   - Distribution plots  
   - Correlation with target variable  
   - Feature importance visualization  

4. **Modeling:**  
   - Logistic Regression  
   - Random Forest Classifier  
   - XGBoost Classifier  

5. **Evaluation Metrics:**  
   - Accuracy  
   - Precision  
   - Recall  
   - F1-score  
   - ROC-AUC  
   - Confusion Matrix  

---

## 🧠 Results Summary

Model	Accuracy	Precision	Recall	F1-score	ROC-AUC
Logistic Regression	0.92	0.96	0.94	0.95	0.89
Random Forest	0.90	0.94	0.93	0.94	0.87
XGBoost	0.90	0.95	0.92	0.93	0.87



- **Best Model:** Logistic Regression (≈92% accuracy)  
- **Top Features:**  
  - Previous failures  
  - Study time  
  - Absences  
  - Parental education  
  - Family support  

---

## 📊 Visual Outputs

The notebook automatically generates:
- Bar chart: Pass vs. Fail distribution  
- Correlation chart: Feature vs. Target  
- Confusion matrix for each model  
- Feature importance (Random Forest)

---

## 🖥️ How to Run (Google Colab)

1. Open [Google Colab](https://colab.research.google.com)  
2. Create a new notebook or upload `Student_Performance_Analytics.ipynb`  
3. Run all cells in order  
4. When prompted, **upload**:  
   - `student-mat.csv`  
   - `student-por.csv` (optional, if available)  
5. View outputs and performance metrics directly in Colab.  

---

## 📁 Repository Structure

