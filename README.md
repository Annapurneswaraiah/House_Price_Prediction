# 🏡 House Price Prediction using Machine Learning

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange.svg)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg)](https://pandas.pydata.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success.svg)]()

A comprehensive Machine Learning project to predict residential house prices using advanced regression techniques based on the Kaggle **House Prices: Advanced Regression Techniques** dataset.

---

## 📌 Project Overview

Predicting property valuations is critical for buyers, sellers, and real estate professionals. This project develops an end-to-end regression pipeline that:
- Cleans and preprocesses complex, high-dimensional housing data.
- Implements exploratory data analysis (EDA) and feature engineering.
- Trains and evaluates regularized regression algorithms (**Ridge**, **Lasso**, and **Linear Regression**).
- Produces final evaluated price predictions formatted for submission.

---

## 🚀 Key Features & Workflow

1. **Exploratory Data Analysis (EDA):**
   - Analysis of target variable distribution (`SalePrice`) and log transformation to handle skewness.
   - Correlation heatmaps to identify primary price drivers (Living Area, Overall Quality, Year Built, etc.).

2. **Data Preprocessing & Feature Engineering:**
   - Missing value imputation for numerical and categorical variables.
   - Outlier detection and handling.
   - One-hot encoding / categorical transformation for categorical features.
   - Feature scaling and log-scale target conversion (`np.log1p` / `np.expm1`).

3. **Model Training & Comparison:**
   - **Linear Regression**: Baseline regression model.
   - **Ridge Regression (L2 Regularization)**: Mitigates multicollinearity among related housing features.
   - **Lasso Regression (L1 Regularization)**: Performs feature shrinkage and selection by penalizing redundant features.

4. **Outputs & Submission:**
   - Exported prediction benchmarks (`ridge_predictions.csv`).
   - Project presentation deck (`House_Price_Prediction_Seminar.pptx`).

---

## 📂 Repository Structure

```plaintext
House_Price_Prediction/
├── liner regression.ipynb               # Data preprocessing, EDA, and initial baseline model
├── test_linear.ipynb                    # Pipeline comparison: Linear, Ridge, and Lasso Regression
├── ridge_predictions.csv                # Output predictions generated using Ridge Regression
├── House_Price_Prediction_Seminar.pptx  # Project presentation & seminar slides
└── README.md                            # Project documentation
```

---

## ⚙️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Annapurneswaraiah/House_Price_Prediction.git
   cd House_Price_Prediction
   ```

2. **Create and activate a virtual environment (optional but recommended):**
   ```bash
   # On Windows
   python -m venv venv
   .\venv\Scripts\activate
   ```

3. **Install the required dependencies:**
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn jupyter
   ```

4. **Run the Jupyter Notebooks:**
   ```bash
   jupyter notebook
   ```

---

## 📊 Models Evaluated

| Model | Regularization | Key Strength |
|---|---|---|
| **Linear Regression** | None (OLS) | Simple interpretable baseline |
| **Ridge Regression** | L2 Penalty | Handles multicollinearity well across correlated features |
| **Lasso Regression** | L1 Penalty | Automatically performs feature selection by shrinking coefficients |

---

## 👤 Author

- **Annapurneswaraiah**
- GitHub: [@Annapurneswaraiah](https://github.com/Annapurneswaraiah)

---

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).
