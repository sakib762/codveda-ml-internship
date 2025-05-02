# Task 1: Preprocessing Data for Machine Learning
**Codveda Technologies Internship**

**Intern:** Muhammad Sakibur Rahaman
**Dataset:** stockprice.csv

## Objective
We are here prepping the stock price data for machine learning by performing necessary preprocessing operations on the data, which are as follows:
- Handling missing data
- Categorical variable encoding
- Date feature transformation
- Normalizing numerical features
- Splitting data into training and test sets

## Steps Performed
1. Loaded and explored the dataset (497,472 rows × 7 columns)
2. Identified and imputed missing values in 'open', 'high', and 'low' columns with median
3. Applied one-hot encoding to the 'symbol' categorical column
4. Converted 'date' column into datetime format and extracted 'year', 'month', 'day' features
5. Dropped the original 'date' column
6. Normalized numeric columns ('open', 'high', 'low', 'close', 'volume') with `StandardScaler`
7. Split the dataset into 80% training and 20% test sets

## Repository Files
- `Task1_DataPreprocessing_Codveda.ipynb`: Jupyter Notebook with the complete code, descriptions, and results
- `README.md`: Documentation for this task

## Results
✅ Missing values handled
✅ Categorical variables encoded
✅ Numerical features scaled
✅ Dataset split into train/test, ML models ready

## Notes
The preprocessed dataset can now be used to build regression or classification models in subsequent tasks.

