# Iris Classification Project

## Objective
Predict Iris flower species using sepal and petal measurements.

## Algorithms Used
1. k-Nearest Neighbors (k-NN)
2. Logistic Regression
3. Decision Tree

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- Confusion Matrix

## Best Model
Model selected based on highest test accuracy.

## Saved Model
iris_best_model.joblib

## Inference Example

```python
import joblib
import pandas as pd

model = joblib.load("iris_best_model.joblib")

sample = pd.DataFrame({
    "sepal_length":[5.1],
    "sepal_width":[3.5],
    "petal_length":[1.4],
    "petal_width":[0.2]
})

prediction = model.predict(sample)

print(prediction)