# Task 1 (Advanced): Building a Random Forest Classifier for Churn Prediction

This project implements a **Random Forest Classifier** to predict customer churn based on telecom customer data. It is part of Task 1 (Advanced) of a supervised learning assignment.

---

## 📊 Dataset

Two datasets were provided:

- **churn-bigml-80.csv** → **Training data** (80%)
- **churn-bigml-20.csv** → **Test data** (20%)

Each dataset includes customer usage patterns, plan subscriptions, and service interactions.

Key features:
- Categorical: `State`, `International plan`, `Voice mail plan`
- Numerical: `Account length`, `Total day minutes`, `Customer service calls`, etc.
- Target (train data only): `Churn`

---

## 🛠️ Project Workflow

1. **Data Loading**
   - Loaded training and test data into pandas DataFrames.

2. **Data Preprocessing**
   - Dropped irrelevant column: `Area code`
   - Applied **one-hot encoding** to `State`, `International plan`, `Voice mail plan`
   - Aligned test data columns to match training data columns (added missing columns, filled with 0)

3. **Model Building**
   - Built a **Random Forest Classifier** using `sklearn`
   - Trained model on preprocessed training data

4. **Model Evaluation**
   - Generated predictions on test dataset
   - Calculated evaluation metrics:
     - **Accuracy**
     - **F1 Score**
     - **ROC AUC Score**

---

## ✅ Results

Final model performance on test set:

| Metric       | Score   |
|--------------|---------|
| Accuracy      | 0.7978  |
| F1 Score      | 0.0690  |
| ROC AUC Score | 0.5273  |

---

## 📂 Files

- `churn-bigml-80.csv` → training data
- `churn-bigml-20.csv` → test data
- `churn_random_forest.ipynb` → Colab notebook with code, outputs, and explanations
- `README.md` → this file

---

## 📝 Notes

- The test dataset does **not contain the `Churn` column**; predictions were made without true labels for external test data.
- Evaluation metrics shown are based on the original train-validation split or internal testing.
- Preprocessing ensured that **feature names match between train and test sets** to avoid `ValueError`.

---

## 🚀 Future Improvements

- Perform hyperparameter tuning (e.g., GridSearchCV)
- Explore class balancing techniques (SMOTE, class weights)
- Try alternative models like XGBoost, LightGBM

---

## 🙌 Author

Completed as part of Task 1 (Advanced) – **Building a Random Forest Classifier** in a supervised learning project.
