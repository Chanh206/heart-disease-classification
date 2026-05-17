# Model Training & Evaluation Summary - Logistic Regression

## Input Data
- Training features: `data/processed/X_train.csv`
- Training target: `data/processed/y_train.csv`
- Test features: `data/processed/X_test.csv`
- Test target: `data/processed/y_test.csv`

## Best Hyperparameters
- `C`: 0.1
- `class_weight`: balanced

- Best CV ROC-AUC: **0.9028**

## Test-Set Metrics

| Metric    |   Value |
|:----------|--------:|
| Accuracy  |  0.8852 |
| Precision |  0.8387 |
| Recall    |  0.9286 |
| F1-Score  |  0.8814 |
| ROC-AUC   |  0.9654 |

## Threshold Tuning
- Optimal decision threshold by F1: **0.54**
- Precision: 0.8667
- Recall: 0.9286
- F1: 0.8966

## Top-5 Features

| feature   |   coefficient |   abs_coefficient |
|:----------|--------------:|------------------:|
| ca_0      |     -0.695464 |          0.695464 |
| cp_4      |      0.583399 |          0.583399 |
| thal_7    |      0.507176 |          0.507176 |
| thal_3    |     -0.477095 |          0.477095 |
| sex_0     |     -0.379424 |          0.379424 |
