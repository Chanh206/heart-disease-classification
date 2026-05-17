# Model Training & Evaluation Summary - XGBoost

## Input Data
- Training features: `data/processed/X_train.csv`
- Training target: `data/processed/y_train.csv`
- Test features: `data/processed/X_test.csv`
- Test target: `data/processed/y_test.csv`

## Best Hyperparameters
- `colsample_bytree`: 0.8
- `learning_rate`: 0.03
- `max_depth`: 2
- `n_estimators`: 100
- `subsample`: 0.8

- Best CV ROC-AUC: **0.8939**

## Test-Set Metrics

| Metric    |   Value |
|:----------|--------:|
| Accuracy  |  0.8852 |
| Precision |  0.8387 |
| Recall    |  0.9286 |
| F1-Score  |  0.8814 |
| ROC-AUC   |  0.9437 |

## Threshold Tuning
- Optimal decision threshold by F1: **0.47**
- Precision: 0.8387
- Recall: 0.9286
- F1: 0.8814

## Top-5 Features

| feature   |   importance |
|:----------|-------------:|
| thal_3    |    0.176158  |
| cp_4      |    0.106766  |
| thal_7    |    0.094205  |
| ca_1      |    0.0656331 |
| ca_0      |    0.0591907 |
