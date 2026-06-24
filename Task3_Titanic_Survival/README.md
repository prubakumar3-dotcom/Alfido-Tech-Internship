# Titanic Survival Prediction

## Objective
Predict passenger survival on the Titanic using machine learning.

## Feature Engineering
- Title Extraction from Name
- Family Size
- Cabin Presence

## Missing Value Handling
- Age → Median
- Fare → Median
- Embarked → Mode

## Models Used
1. Logistic Regression
2. Random Forest
3. Gradient Boosting

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

## Explainability
Feature Importance using Random Forest.

## Saved Model
titanic_survival_model.joblib

## Prediction Example

```python
import joblib

model = joblib.load(
    "titanic_survival_model.joblib"
)

prediction = model.predict(sample)

print(prediction)
```