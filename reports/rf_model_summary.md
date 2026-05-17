# Model Training & Evaluation Summary - Random Forest

## Input Data
- Training features: `data/processed/X_train.csv`
- Training target: `data/processed/y_train.csv`
- Test features: `data/processed/X_test.csv`
- Test target: `data/processed/y_test.csv`

## Best Hyperparameters
- `max_depth`: 5
- `max_features`: log2
- `min_samples_leaf`: 1
- `min_samples_split`: 2
- `n_estimators`: 200

- Best CV ROC-AUC: **0.9048**

## Test-Set Metrics

| Metric    |   Value |
|:----------|--------:|
| Accuracy  |  0.8852 |
| Precision |  0.8387 |
| Recall    |  0.9286 |
| F1-Score  |  0.8814 |
| ROC-AUC   |  0.9524 |

## Threshold Tuning
- Optimal decision threshold by F1: **0.48**
- Precision: 0.8438
- Recall: 0.9643
- F1: 0.9000

## Top-5 Features

| feature   |   importance |
|:----------|-------------:|
| thal_3    |    0.120654  |
| thal_7    |    0.091875  |
| cp_4      |    0.0869176 |
| ca_0      |    0.0860563 |
| thalach   |    0.077484  |
