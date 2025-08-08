# Diabetes-Bagging-Predictor

## Problem
We used a diabetes dataset to predict whether a person has diabetes (0 or 1). The goal was to improve accuracy using Bagging and compare it with other models.

## What Is Bagging?
Bagging (Bootstrap Aggregation) means training multiple models on random parts of the data and combining their results. It reduces overfitting and improves performance.
We used BaggingClassifier with DecisionTree as the base model.

## Solution
I used BaggingClassifier with 100 estimators and 80% data in each sample.

oob_score=True was used to test accuracy without splitting.

I also used score() function to check model accuracy, and it gave better results compared to single models.

## Models Tried
DecisionTreeClassifier – basic model

RandomForestClassifier – it's also based on bagging

BaggingClassifier – actual bagging done with DecisionTree as base model
BaggingClassifier gave better accuracy than the others.

## Dataset Used
The dataset used is diabetes.csv.

## Columns Used
- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age
- Outcome (target)
