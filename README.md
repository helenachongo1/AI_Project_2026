# Concrete Compressive Strength Prediction Using Machine Learning and Hybrid Ensemble Models

## Overview
This project focuses on predicting the compressive strength of concrete using various Machine Learning techniques. The goal is to replace time-consuming laboratory testing with accurate and efficient predictive models.

---

## Objectives
- Implement multiple ML models for regression
- Compare performance across models
- Develop a hybrid ensemble model
- Analyze feature importance
- Improve prediction accuracy and robustness

---

## Dataset
- Source: Yeh (1998)
- Total Samples: 1030
- Features:
  - Cement
  - Blast Furnace Slag
  - Fly Ash
  - Water
  - Superplasticizer
  - Coarse Aggregate
  - Fine Aggregate
  - Age

- Target:
  - Compressive Strength (MPa)

---

## Methodology

### Data Preprocessing
- No missing values
- Feature standardization
- Train-test split (80:20)

### Models Used
- Linear Regression
- Ridge & Lasso
- Decision Tree
- Random Forest
- SVR
- ANN
- GBRT
- XGBoost
- LightGBM

### Hybrid Model
A weighted ensemble of:
- GBRT
- LightGBM
- XGBoost

---

## Results

| Model | RMSE | MAE | R² |
|------|------|------|------|
| GBRT | 4.21 | 2.80 | 0.93 |
| LightGBM | 4.43 | 2.80 | 0.92 |
| XGBoost | 4.55 | 3.24 | 0.91 |

Boosting models performed best  
Hybrid model improved robustness  

---

## Evaluation Metrics
- R² Score
- RMSE
- MAE

---

## Screenshots

### 🔹 Model Performance
![Model Comparison](images/model_comparison.png)

### 🔹 Actual vs Predicted
![Prediction](images/prediction.png)

### 🔹 Residual Plot
![Residual](images/residual.png)

---

## Tools & Libraries
- Python
- NumPy, Pandas
- Scikit-learn
- XGBoost
- LightGBM
- Matplotlib

---

## How to Run

```bash
# Clone repository
git clone https://github.com/your-username/your-repo-name.git

# Navigate to project
cd your-repo-name

# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook
