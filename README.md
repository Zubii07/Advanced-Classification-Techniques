# 🚗 Car Evaluation - Random Forest Classifier

This project demonstrates how to apply the **Random Forest algorithm** to a real-world dataset — the **Car Evaluation** dataset — to classify the acceptability of cars based on various features like buying price, maintenance cost, safety, and capacity.

---

## 📚 What I Learned

- 📊 **How Random Forest works**: Bagging, bootstrap sampling, ensemble voting
- 🧮 **Math behind the algorithm**: Gini impurity, decision tree splits, majority voting
- 🧠 **Model intuition**: How decision trees make splits, and how Random Forest reduces overfitting
- 🧪 **Hands-on practice**: Applied Random Forest on real categorical data with preprocessing and evaluation

---

## 🔧 Technologies Used

- Python 3
- Pandas & NumPy
- Scikit-learn (for model training)
- Matplotlib & Seaborn (for visualizations)

---

## 📁 Dataset

- **Source**: UCI Machine Learning Repository  
- **Name**: Car Evaluation Dataset  
- **Features**:
  - `buying`: buying price (`vhigh`, `high`, `med`, `low`)
  - `maint`: maintenance cost
  - `doors`: number of doors (`2`, `3`, `4`, `5more`)
  - `persons`: capacity (`2`, `4`, `more`)
  - `lug_boot`: luggage boot size (`small`, `med`, `big`)
  - `safety`: safety rating (`low`, `med`, `high`)
- **Target**: `class` (acceptability → `unacc`, `acc`, `good`, `vgood`)

---

## 🔍 Problem Statement

The goal is to predict **car acceptability** based on the given features using a **Random Forest Classifier**.

---

## 🧪 Steps Performed

1. ✅ Loaded and explored the dataset
2. 🔄 Encoded categorical features using `OrdinalEncoder` and target with `LabelEncoder`
3. 🧠 Trained a `RandomForestClassifier` with 100 trees
4. 📉 Evaluated performance using confusion matrix and classification report
5. 📊 Visualized feature importances to understand model decisions

---

## 📈 Model Performance

- Achieved **high accuracy**, especially in identifying "unacceptable" cars
- **Confusion matrix** and **classification report** included for full transparency
- Model slightly confused between `acc`, `good`, and `vgood` — typical for closely related labels

---

## 🔍 Sample Output

### Confusion Matrix
![Confusion Matrix](confusion_matrix.png)

### Feature Importance
![Feature Importance](feature_importance.png)

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/car-evaluation-random-forest.git
   cd car-evaluation-random-forest
