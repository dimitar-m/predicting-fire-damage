# Predicting Forest Fire Damage: From Weather Signals to Burned Area Forecasts  

## How to Run  
- Open the latest version of the project in **NBViewer**:  
  [View in NBViewer](https://nbviewer.org/github/dimitar-m/predicting-heart-disease/blob/master/predicting-heart-disease-v1.3.ipynb)  

## Overview  
This project uses the [UCI Forest Fires dataset](https://archive.ics.uci.edu/dataset/162/forest+fires) to predict the extent of burned area in Portuguese forests. The goal is to explore how weather conditions, fire indices, and seasonal patterns contribute to fire damage, while systematically testing multiple machine learning models.  

## Methods and Workflow  
- **Data Preprocessing**:  
  - KNN imputation for missing values  
  - Feature engineering: log-transforms, interaction terms, categorical encoding  
  - Outlier handling and scaling  
  - New binary and grouped features (`is_weekend`, `fire_season`)  
- **Pipelines**: End-to-end workflows for clean and reproducible modeling.  
- **Models Explored**:  
  - Baseline Linear Regression  
  - Feature Selection approaches  
  - RidgeCV & LassoCV  
  - Polynomial & Spline models  
  - Random Forest Regression  
  - XGBoost Regression  
  - Two-Stage (Zero-Inflated) Model: Classification (fire occurrence) + Regression (burned area).  

## Results  
- Weak correlations between predictors and burned area made prediction challenging.  
- All models achieved similar error levels.  
- Tree-based methods (Random Forest, XGBoost) and the two-stage model offered modest improvements over linear baselines.  

## Key Takeaways  
- Pipelines streamlined preprocessing + modeling, reducing complexity.  
- Systematic comparison of diverse models highlighted the dataset’s limitations.  
- Even with modest results, this project demonstrates the full ML workflow from EDA to advanced models.  

## Repository Structure  
- `notebooks/` → Jupyter notebooks with analysis  
- `data/` → Dataset (if allowed to share, otherwise link to UCI)  
- `images/` → Visualizations and figures  
- `README.md` → Project overview  

## Dataset Source  
[Forest Fires – UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/162/forest+fires)  
