# 🍷 Wine Quality Classification Using Machine Learning

## 📌 Project Overview

This project focuses on predicting wine quality categories using Machine Learning techniques. It uses the Wine Quality Red dataset and applies Feature Engineering, Feature Selection, and Principal Component Analysis (PCA) to explore different approaches for improving classification performance.

A Random Forest Classifier is trained using three different feature approaches, and their performances are compared using various evaluation metrics.

## 🎯 Project Objectives

- Perform data preprocessing and exploratory data analysis.
- Create meaningful features using Feature Engineering.
- Identify important features using SelectKBest.
- Reduce dimensionality using Principal Component Analysis (PCA).
- Build classification models using Random Forest.
- Compare model performance using evaluation metrics.

## 📂 Dataset

**Dataset:** Wine Quality – Red Wine

**Original dataset dimensions:** 1,599 rows and 12 columns.

**After removing duplicates:** 1,359 rows and 12 columns.

**Target Variable:** `quality_category`

The original numerical wine quality values are converted into three categories:

- Low: Quality 3–5
- Medium: Quality 6
- High: Quality 7–8

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## ⚙️ Project Workflow

1. Data Loading and Exploration
2. Data Preprocessing
3. Duplicate Removal
4. Target Variable Creation
5. Feature Engineering
6. Feature Selection using SelectKBest
7. Feature Scaling using StandardScaler
8. Dimensionality Reduction using PCA
9. Train-Test Splitting
10. Random Forest Model Building
11. Model Evaluation and Comparison

## 🧪 Feature Engineering

Three new features were created:

- **Total Acidity:** Combination of fixed acidity, volatile acidity, and citric acid.
- **Sulfur Dioxide Ratio:** Ratio of free sulfur dioxide to total sulfur dioxide.
- **Alcohol to Density:** Ratio of alcohol to density.

## 🔍 Feature Selection

SelectKBest with ANOVA F-test (`f_classif`) was used to identify the five most relevant features.

Selected features:
- Volatile Acidity
- Citric Acid
- Sulphates
- Alcohol
- Alcohol to Density

## 📉 Principal Component Analysis (PCA)

PCA was applied after feature scaling to reduce the original 14 features into 9 principal components while retaining approximately 97.50% of the variance.

## 🤖 Model Building

Three Random Forest classification models were developed:

1. **Original Features:** Uses all 14 input features.
2. **Feature Selection:** Uses the 5 selected features.
3. **PCA:** Uses 9 principal components.

## 📊 Model Evaluation and Comparison

All three models were evaluated using Accuracy, Precision, Recall, and F1-score.

| Evaluation Metric | Original Features | Feature Selection | PCA |
|---|---:|---:|---:|
| Accuracy | 59.56% | 56.25% | **62.13%** |
| Precision | 60.35% | 52.65% | **63.13%** |
| Recall | 54.17% | 48.96% | **57.48%** |
| F1-score | 56.12% | 50.00% | **59.42%** |

## 🏆 Key Findings

- The original feature model achieved 59.56% accuracy.
- The feature selection model achieved 56.25% accuracy.
- The PCA-based model achieved the highest accuracy of 62.13%.
- PCA performed better across all four evaluation metrics in this experiment.

## 📝 Conclusion

This project demonstrates the practical application of Feature Engineering, Feature Selection, and Dimensionality Reduction in a Machine Learning classification problem.

Among the three approaches, the PCA-based Random Forest model achieved the best performance with 62.13% accuracy and a macro F1-score of 59.42%.

The project provided practical experience in data preprocessing, feature transformation, model development, and evaluation.

## 👩‍💻 Author

**Devadharshni S**

B.Sc. Data Science
