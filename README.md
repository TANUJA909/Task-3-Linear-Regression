# Task 3: Linear Regression – Housing Price Prediction

## Objective
To implement and understand simple and multiple linear regression using the Housing Price Prediction dataset. This includes data preprocessing, model training, evaluation, and interpretation of results.

---

## Tools Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## Dataset
Dataset used: [Housing Price Prediction – Kaggle](https://www.kaggle.com/datasets/harishkumardatalab/housing-price-prediction)

This dataset contains features such as area, number of bedrooms, bathrooms, furnishing status, and more — to predict house prices.

---

## Steps Performed

### 1. Data Loading and Exploration
- Loaded the CSV file using `pandas`.
- Explored dataset using `df.info()`, `df.describe()`, and `df.isnull().sum()`.

### 2. Data Preprocessing
- Converted binary categorical columns (e.g., `mainroad`, `guestroom`, `basement`, `airconditioning`) from `'yes'`/`'no'` to `1`/`0`.
- Mapped furnishing status to ordinal values:
  - `'unfurnished'` → `0`
  - `'semi-furnished'` → `1`
  - `'furnished'` → `2`

### 3. Feature and Target Selection
- Selected `price` as the target variable.
- All other columns were used as features.

### 4. Train-Test Split
- Split the dataset into training and testing sets using `train_test_split()` with an 80-20 ratio.

### 5. Model Training
- Trained a `LinearRegression` model using scikit-learn.

### 6. Model Evaluation
- Evaluated the model
