# Task 2: Linear Regression
**Codveda Technologies Internship**

**Intern:** Muhammad Sakibur Rahaman
**Dataset Used:** Boston Housing Dataset (houseprice.csv)

## Objective
We, in this task, created a linear regression model to predict house prices (MEDV) from various features of the Boston Housing dataset.

We aimed to:
- Investigate and plot the dataset
- Select features through correlation
- Train a linear regression model
- Explain the model coefficients
- Evaluated the model performance on the basis of R-squared and Mean Squared Error (MSE)

---

## Steps Executed
1. Loaded dataset and assigned proper column names
2. Examined data types, distributions, and correlations
3. Selected features on the basis of correlation with target `MEDV`
4. Partitioned dataset into training (80%) and test (20%) sets
5. Fitted linear regression model to training set
6. Interpreted coefficients of feature
7. Evaluated the model on the basis of R-squared and MSE
8. Visualized Actual vs Predicted prices

---

## Results
✅ Selected features: `RM`, `LSTAT`, `PTRATIO`, `INDUS`, `TAX`
✅ R-squared obtained: *{your_r2_score_here}*
✅ Mean Squared Error: *{your_mse_here}*

The model suggests:
- Positive correlation: More rooms (`RM`) increases price
- Negative correlation: More `LSTAT` or `TAX` reduces price

---

## Repository Files
- `Task2_LinearRegression_Codveda.ipynb`: Jupyter Notebook containing code and explanations
- `README.md`: README for Task 2

---

## Notes
The model can be improved further by incorporating more features, polynomial terms, or trying regularization techniques.

