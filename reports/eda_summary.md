# EDA Summary - Heart Disease Dataset

## Dataset Overview
- Number of rows: 303
- Number of original columns: 14
- Duplicate rows: 0

## Missing Values
- `ca`: 4 missing values, imputed with mode.
- `thal`: 2 missing values, imputed with mode.

## Target Distribution
|   target |   count | label      |   percent |
|---------:|--------:|:-----------|----------:|
|        0 |     164 | No disease |     54.13 |
|        1 |     139 | Disease    |     45.87 |

## Strongest Correlations With Binary Target
|         |   correlation_with_target |   abs_correlation |
|:--------|--------------------------:|------------------:|
| thal    |                     0.522 |             0.522 |
| ca      |                     0.46  |             0.46  |
| exang   |                     0.432 |             0.432 |
| oldpeak |                     0.425 |             0.425 |
| thalach |                    -0.417 |             0.417 |
| cp      |                     0.414 |             0.414 |
| slope   |                     0.339 |             0.339 |
| sex     |                     0.277 |             0.277 |

## Modeling Notes
- Use binary target: `0 = no disease`, `1 = disease`.
- Apply one-hot encoding to categorical features.
- Scale numerical features for distance-based or regularized models.
- Evaluate with accuracy, precision, recall, F1-score and ROC-AUC because this is a medical classification problem.
