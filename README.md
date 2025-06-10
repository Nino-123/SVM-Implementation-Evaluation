# 🫀 Heart Disease Prediction using SVM Kernels

**Group 4 – Machine Learning CSB**  
Final Group Assignment – SVM Kernel Evaluation

## 📌 Overview

This project evaluates the performance of various **Support Vector Machine (SVM)** kernels in predicting heart disease. We compare **single SVM models** and **ensemble classifiers** using accuracy, precision, sensitivity, and F1-score on a structured heart dataset.

## 👥 Team Members
- Satwika Nino Wandhana - 23/516202/PA/22066
- Adam Maulana Haq- 23/511623/PA/21832
- Daniel Winston Mandela Tulung - 23/516260/PA/22080
- Rindra Adriansyah - 23/511559/PA/21820
- Mohammad Azka Khairur Rohman - 23/511608/PA/21830

## 📊 Dataset

- **Name:** [Heart Disease Dataset (Kaggle)](https://www.kaggle.com/datasets/arezaei81/heartcsv)
- **Features:** Age, Sex, Chest pain type, Cholesterol, Fasting Blood Sugar, etc.
- **Target:** Heart Disease Presence (binary classification)

## 🧠 Models Used

### 🔹 Single SVM Models
| Kernel   | Accuracy | Precision | Sensitivity | F1-Score |
|----------|----------|-----------|-------------|----------|
| Linear   | 0.861    | 0.865     | 0.855       | 0.857    |
| RBF      | 0.673    | 0.694     | 0.651       | 0.640    |
| Poly (3) | 0.666    | 0.672     | 0.646       | 0.639    |
| Sigmoid  | 0.541    | 0.271     | 0.496       | 0.350    |

> 🔍 **Best:** Linear SVM – high overall performance with 86% accuracy

### 🔹 Ensemble Meta-Models
Each kernel was tested as a **meta-model** with base learners:
- Logistic Regression
- Decision Tree Classifier
- Gaussian Naive Bayes

| Meta Kernel | Accuracy | Precision | Sensitivity | F1-Score |
|-------------|----------|-----------|-------------|----------|
| Poly (3)    | 0.874    | 0.874     | 0.875       | 0.873    |
| RBF         | 0.868    | 0.867     | 0.867       | 0.865    |
| Linear      | 0.858    | 0.857     | 0.855       | 0.855    |
| Sigmoid     | 0.782    | 0.844     | 0.761       | 0.755    |

> 🏆 **Best Overall:** Ensemble with **Polynomial kernel** – captures complex patterns effectively

## 🔧 Tools & Libraries

- Google Colab
- `scikit-learn`
- `numpy`
- `pandas`
- `matplotlib` / `seaborn` (for visualization)

## 📈 Key Takeaways

- **Linear SVM** is reliable as a standalone model.
- **Ensembling** improves performance, especially with nonlinear kernels like Polynomial.
- **Sigmoid kernel** consistently underperforms and is not recommended for this task.


## 📎 References

- [SVM Kernels - scikit-learn docs](https://scikit-learn.org/stable/modules/svm.html)
- [Heart Disease Dataset - Kaggle](https://www.kaggle.com/datasets/arezaei81/heartcsv)

