# Stroke Risk Prediction Model 🧠

## 📌 Overview
This project focuses on the development of a Machine Learning model to predict the likelihood of a patient suffering a stroke. By analyzing clinical parameters such as glucose levels, BMI, and hypertension history, this tool aims to assist in early detection and preventative healthcare.

As a medical student, I approached this problem with a focus on **Recall**—prioritizing the minimization of False Negatives, as missing a stroke case in a real-world setting is life-threatening.

## ⚙️ Key Features
- **Data Preprocessing:** Handled missing values (BMI imputation) and normalized clinical features.
- **Exploratory Data Analysis (EDA):** Visualized correlations between age, glucose levels, and stroke risk.
- **Class Imbalance Handling:** Addressed the highly imbalanced dataset using **SMOTE** (Synthetic Minority Over-sampling Technique) and class weighting.
- **Model Comparison:** Evaluated 5 different algorithms to find the best balance between sensitivity and specificity.

## 🔬 Model Performance
Since "missing a stroke case" (False Negative) is critical, this project prioritized **Recall** as the primary metric.

I compared five algorithms:
1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Decision Tree
4. Random Forest
5. Gradient Boosting

### Key Findings:
- **Best Performer:** The **Random Forest** model emerged as the most balanced classifier. It achieved a **Recall of 80%** (identifying 80% of actual stroke cases) and the highest **F1-Score (0.28)** among all models tested.
- **Alternative:** Logistic Regression also achieved an excellent **Recall of 80%** and the highest **AUC-ROC score (0.83)**, making it a strong candidate for probability-based risk scoring.
- **Clinical Insight:** The analysis highlighted that Age and Average Glucose Levels were the most significant predictors of stroke risk in this dataset.

## 🛠 Tech Stack
- **Language:** Python 🐍
- **Libraries:**
  - `Pandas` & `NumPy` (Data Manipulation)
  - `Matplotlib` & `Seaborn` (Visualization)
  - `Scikit-learn` (Machine Learning)
  - `Imbalanced-learn` (SMOTE)
   ```bash
   git clone [https://github.com/YOUR_USERNAME_HERE/Stroke-Risk-Analysis.git](https://github.com/YOUR_USERNAME_HERE/Stroke-Risk-Analysis.git)
