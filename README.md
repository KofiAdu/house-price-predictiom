# Housing Price Prediction

A machine learning project to predict house sale prices using the Ames, Iowa dataset — a clean, well-documented alternative to the classic Boston Housing dataset.

This project was built as part of a personal learning goal to improve at **feature engineering**, **model tuning**, and working with **structured/tabular data** using tree-based models.

---

##  Project Overview

**Objective**: Predict `SalePrice` for each home in the test dataset based on 79 explanatory variables.

**Techniques Used**:
- Feature Engineering
- Data Cleaning & Preprocessing
- Categorical Encoding
- Random Forest & XGBoost Regressors
- Cross-Validation
- RMSE Evaluation on Log-Transformed Targets

---

##  Key Concepts Practiced

- Understanding when and why to log-transform skewed targets
- Engineering domain-informed features like `TotalSF`, `HouseAge`, `TotalBathrooms`
- Avoiding overfitting through cross-validation and regularization
- Comparing model performance via CV RMSE
- Averaging model predictions for better generalization

---

## Models & Results

| Model           | Train RMSE (log) | CV RMSE (log) |
|----------------|------------------|----------------|
| Random Forest  | 0.1237           | 0.1486         |
| XGBoost        | 0.0810           | 0.1260         |

---

##  Project Structure

```
├── data/                
├── README.md
└── requirements.txt    
```

---

## How to Run

1. Clone the repo:
   ```
   git clone https://github.com/yourusername/ames-housing-prediction.git
   ```

2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Run the training pipeline:
   - Open notebooks in Jupyter

4. Submit predictions:
   ```
   submission/submission_xgb.csv
   submission/submission_rf_tuned.csv
   ```

---

## What I Learned

- How to craft features that actually improve model signal
- When to use label vs. one-hot encoding
- How tree models like Random Forest and XGBoost behave differently
- How cross-validation reveals overfitting
- Why log transformations are often essential in regression competitions

---

## 📎 Dataset Source

- [Kaggle Competition: House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)

---

