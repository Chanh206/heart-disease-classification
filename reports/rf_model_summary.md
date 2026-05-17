# Model Training & Evaluation Summary — Random Forest

## Best Hyperparameters (GridSearchCV, 5-fold CV, scoring=roc_auc)

- `max_depth`: 10
- `max_features`: log2
- `min_samples_leaf`: 2
- `min_samples_split`: 2
- `n_estimators`: 300

- Best CV ROC-AUC: **0.9038**

## Test-Set Metrics

| Metric    |   Value |
|:----------|--------:|
| Accuracy  |  0.8852 |
| Precision |  0.8387 |
| Recall    |  0.9286 |
| F1-Score  |  0.8814 |
| ROC-AUC   |  0.9502 |

## Threshold Tuning
- Optimal decision threshold (max F1): **0.46**
  - Precision: 0.8438
  - Recall:    0.9643
  - F1:        0.9000

## Top-5 Features by Importance

| feature   |   importance |
|:----------|-------------:|
| thal_3    |    0.102659  |
| cp_4      |    0.10232   |
| thalach   |    0.0955273 |
| thal_7    |    0.0896528 |
| ca_0      |    0.0891327 |
