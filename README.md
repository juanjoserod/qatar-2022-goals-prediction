# Qatar 2022 Goals Prediction

This repository provides a reproducible pipeline for building and evaluating machine learning models that predict goal outcomes from event data of the FIFA World Cup Qatar 2022, extracted via StatsBomb Open Data
.

Project Overview

Goal: Predict whether a shot results in a goal based on contextual event features.

Data Source: StatsBomb event data (events.csv), publicly available via statsbombpy.

Approach: Combination of feature engineering (distance, angle, body part, play pattern, etc.) and multiple ML models (Logistic Regression, Random Forest, Gradient Boosting, Neural Networks).

Evaluation Metrics: Accuracy, F1, ROC-AUC, PR-AUC — with a focus on precision-recall due to class imbalance.

Explainability: Local and global model explanations using LIME/SHAP.
## Quickstart
```bash
conda env create -f environment.yml
conda activate qatar2022
python -m src.qatar_goals.train --data data/raw/events.csv --model-out models/baseline.joblib
