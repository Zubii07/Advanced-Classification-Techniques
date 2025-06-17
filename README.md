# 🤖 Advanced Classification Algorithms: Random Forest, SVM & KNN

This repository showcases three real-world classification problems solved using machine learning algorithms — **Random Forest**, **Support Vector Machine (SVM)**, and **K-Nearest Neighbors (KNN)**. Each project applies core ML principles, highlights algorithmic intuition, and evaluates model performance with visualizations.

---

## 🌲 1. Random Forest Classifier – Car Evaluation

This project demonstrates how to apply the **Random Forest algorithm** to classify the acceptability of cars using the **Car Evaluation Dataset**.

### 📚 About Random Forest

Random Forest is an **ensemble learning algorithm** that combines multiple decision trees to improve accuracy and reduce overfitting. It works by:
- **Bagging (Bootstrap Aggregation)**: Training each tree on a random sample of data.
- **Random Feature Selection**: Each tree splits on a random subset of features.
- **Majority Voting**: Final prediction is based on the majority class predicted by individual trees.

### 🧠 What I Learned
- How Random Forest reduces overfitting via bagging.
- How decision trees use Gini impurity or entropy to split data.
- How ensemble voting improves model robustness.
- Hands-on experience with categorical preprocessing and model evaluation.

### 🧪 Implementation Steps
1. Loaded and explored the dataset.
2. Encoded categorical features using `OrdinalEncoder` and `LabelEncoder`.
3. Trained a `RandomForestClassifier` with 100 estimators.
4. Evaluated with confusion matrix & classification report.
5. Visualized feature importances.

### 📊 Model Performance

- High accuracy, especially in predicting the "unacceptable" (`unacc`) class.
- Slight confusion between `acc`, `good`, and `vgood` due to class similarity.

**Confusion Matrix Snapshot:**

| Actual \ Predicted | acc | good | unacc | vgood |
|--------------------|-----|------|--------|--------|
| acc                | 108 | 5    | 12     | 2      |
| good               | 1   | 10   | 2      | 5      |
| unacc              | 10  | 0    | 389    | 0      |
| vgood              | 4   | 1    | 0      | 21     |

---

## 🧬 2. Support Vector Machine – Breast Cancer Detection

A binary classification task using the **Breast Cancer Wisconsin dataset** to predict whether a tumor is benign or malignant.

### 🧠 What I Learned
- SVM aims to find the **maximum-margin hyperplane** that best separates the classes.
- The **kernel trick** (e.g., RBF kernel) helps in solving non-linear problems.
- Applied model evaluation using confusion matrix and boundary plots.

### 🧮 Mathematical Foundation
- Maximizing margin between support vectors:
  \[
  \text{maximize } \frac{2}{\|\mathbf{w}\|} \quad \text{subject to constraints}
  \]
- Uses **hinge loss** for optimization.

---

## 👥 3. K-Nearest Neighbors – Social Network Ads

This project uses **KNN** to predict whether a user purchases a product based on their **age** and **estimated salary**.

### 🧠 What I Learned
- KNN is a **non-parametric, lazy learning** algorithm.
- Predictions are made based on the **majority vote** of the k nearest points.
- Explored the influence of distance metrics (e.g., Euclidean).

### 🧮 Mathematical Foundation
- Euclidean Distance:
  \[
  d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}
  \]

---

## 🔧 Technologies Used

- **Python 3**
- **Pandas & NumPy** – data manipulation
- **Scikit-learn** – model training and evaluation
- **Matplotlib & Seaborn** – visualizations

---


## 🔍 Problem Statements Recap

| Algorithm | Dataset             | Goal                                               |
|-----------|---------------------|----------------------------------------------------|
| Random Forest | Car Evaluation   | Predict car acceptability class                   |
| SVM         | Breast Cancer      | Classify tumors as benign or malignant            |
| KNN         | Social Ads         | Predict purchase decision from age & salary       |

---

## Happy Learning
