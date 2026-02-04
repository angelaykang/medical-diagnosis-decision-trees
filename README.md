# Medical Diagnosis with Decision Trees and Regression Analysis

A comprehensive machine learning project demonstrating interpretable models for medical diagnosis and regression analysis. This project showcases decision trees for medical diagnosis and compares various regression techniques including LASSO, Ridge, PCR, and XGBoost.

## Project Overview

This project consists of two main components:

### 1. Decision Trees for Medical Diagnosis
- **Objective**: Predict inflammation and nephritis from patient symptoms
- **Dataset**: Acute inflammation dataset with 6 features (temperature, nausea, lumbar pain, urine pushing, micturition pains, urethra burning)
- **Techniques**:
  - Decision tree classification
  - Cost-complexity pruning
  - Rule extraction and interpretability analysis
  - Tree visualization

### 2. Regression Analysis
- **Objective**: Predict crime rates using community data
- **Dataset**: Communities and Crime dataset with 122 features
- **Techniques**:
  - Linear Regression (baseline)
  - Ridge Regression with cross-validation
  - LASSO Regression (standardized and non-standardized)
  - Principal Component Regression (PCR)
  - XGBoost Gradient Boosting
  - Feature importance analysis

## Features

- **Interpretable Models**: Decision trees provide clear, human-readable rules for medical diagnosis
- **Model Comparison**: Comprehensive comparison of multiple regression techniques
- **Feature Engineering**: Missing value imputation, feature selection, and coefficient of variation analysis
- **Visualization**: Tree plots, correlation matrices, scatter plots, and feature importance charts
- **Hyperparameter Tuning**: Cross-validation and grid search for optimal model parameters

## Project Structure

```
medical-diagnosis-decision-trees/
├── README.md
├── requirements.txt
├── .gitignore
├── data/
│   ├── diagnosis.csv
│   ├── diagnosis.names
│   ├── communities.csv
│   └── communities.names
└── notebooks/
    └── medical_diagnosis_analysis.ipynb
```

## Installation

1. Clone this repository:
```bash
git clone <repository-url>
cd medical-diagnosis-decision-trees
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

## Usage

1. Open the Jupyter notebook:
```bash
jupyter notebook notebooks/medical_diagnosis_analysis.ipynb
```

2. Run all cells to execute the analysis. The notebook includes:
   - Data loading and preprocessing
   - Decision tree training and visualization
   - Regression model training and evaluation
   - Results visualization and interpretation

## Key Results

### Decision Trees
- **Inflammation Prediction**: Simple decision tree with high interpretability
- **Nephritis Prediction**: Temperature and lumbar pain are key predictors
- **Pruning**: Cost-complexity pruning maintains model performance while improving interpretability

### Regression Models
- **XGBoost**: Best performance (Test R² = 0.663, MSE = 0.016024)
- **Ridge Regression**: Test R² = 0.632, MSE = 0.017504
- **LASSO Regression**: Test R² = 0.630, MSE = 0.017618 (74 features selected)
- **Linear Regression**: Test R² = 0.622, MSE = 0.017966
- **PCR**: Test R² = 0.615, MSE = 0.018303 (46 optimal components)

## Technologies Used

- **Python 3.x**
- **scikit-learn**: Machine learning models and preprocessing
- **XGBoost**: Gradient boosting framework
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computing
- **matplotlib & seaborn**: Data visualization

## Dataset Information

### Acute Inflammation Dataset
- **Source**: Medical diagnosis dataset
- **Features**: Temperature, nausea, lumbar pain, urine pushing, micturition pains, urethra burning
- **Targets**: Inflammation, Nephritis (binary classification)

### Communities and Crime Dataset
- **Source**: UCI Machine Learning Repository
- **Features**: 122 socio-economic and demographic features
- **Target**: Crime rate (continuous)

## Contributing

This is a portfolio project. Feel free to fork and modify for your own learning purposes.

## Author

Portfolio project demonstrating machine learning techniques for medical diagnosis and regression analysis.

---

**Note**: This project demonstrates practical applications of interpretable machine learning and regression analysis techniques commonly used in data science and healthcare analytics.
