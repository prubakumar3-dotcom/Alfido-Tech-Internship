# House Price Prediction

## Objective
Predict house prices using regression models.

## Models Used
1. Linear Regression
2. Random Forest Regressor
3. Gradient Boosting Regressor

## Preprocessing
- Missing Value Imputation
- One-Hot Encoding
- Feature Scaling
- Log Transformation of Target Variable

## Evaluation Metrics
- RMSE
- MAE
- R² Score
- Residual Analysis

## Best Model
Selected based on lowest RMSE.

## Saved Model
house_price_model.joblib

## Prediction Example

```python
import joblib
import pandas as pd

model = joblib.load("house_price_model.joblib")

sample = X.iloc[[0]]

prediction = model.predict(sample)

print(prediction)