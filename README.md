# 🛒 Big Mart Sales Prediction

This project aims to predict outlet sales (`OutletSales`) for various products in Big Mart stores using machine learning. It involves training a regression model on historical data and generating predictions for unseen test data.

---

## 📊 Project Overview

**Goal**: Build a predictive model that estimates the `OutletSales` for each product-outlet combination.

**Steps**:

* Data Cleaning and Feature Engineering
* Encoding Categorical Variables
* Feature Scaling
* Model Training using MLP Regressor
* Hyperparameter Tuning with GridSearchCV
* Model Evaluation and Test Prediction

---

## 📁 Dataset

The dataset includes:

* **Product features**: Product Type, MRP, fat content, visibility, etc.
* **Outlet features**: ID, size, location type, establishment year
* **Target**: `OutletSales` (present only in training data)

---

## 🛠️ Libraries Used

* `pandas`, `numpy`
* `matplotlib`, `seaborn` for visualization
* `scikit-learn` for preprocessing and modeling

---

## 📈 Modeling Details

* **Model**: Multi-Layer Perceptron Regressor (`MLPRegressor`)
* **Optimization**: `GridSearchCV` used to tune hyperparameters
* **Preprocessing**: StandardScaler and LabelEncoder applied consistently
* Final predictions made on test data using the trained and tuned model

---

## 💡 Insights

* The MLPRegressor showed improved performance after tuning.
* Label encoding and scaling helped handle mixed data types and numeric ranges.
* We considered decoding predictions for human readability but skipped it in the final version since it wasn’t necessary. Instead, predictions were simply added to a copy of the original test data for interpretation.

---

## ✅ Lessons Learned

* Store preprocessing tools like scalers and encoders for future use on new data.
* Not all additional processing (e.g., decoding) is always required—sometimes a simple approach is best.
* Consistency in the preprocessing pipeline is crucial for reliable predictions.

---

## 📂 Files

```
├── big_mart_model.ipynb     # Complete notebook with training, testing, and predictions
├── Test-Set.csv             # Test dataset used for final predictions
├── README.md                # This file
```

---

## 🚀 Run Instructions

1. Clone this repo
2. Launch `big_mart_model.ipynb` in Jupyter or VS Code
3. Run all cells to preprocess, train, evaluate, and generate predictions

---

## 👨‍💻 Author

Built as a learning project with a focus on real-world ML workflows, feature engineering, and model tuning.
