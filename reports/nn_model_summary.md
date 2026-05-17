# Model Training & Evaluation Summary - Neural Network (MLP)

## Input Data
- Training features: `data/processed/X_train.csv`
- Training target: `data/processed/y_train.csv`
- Test features: `data/processed/X_test.csv`
- Test target: `data/processed/y_test.csv`

## Best Hyperparameters
- `alpha`: 0.0001
- `hidden_layer_sizes`: (32,)
- `learning_rate_init`: 0.005

- Best CV ROC-AUC: **0.8804**

## Test-Set Metrics

| Metric    |   Value |
|:----------|--------:|
| Accuracy  |  0.8361 |
| Precision |  0.7647 |
| Recall    |  0.9286 |
| F1-Score  |  0.8387 |
| ROC-AUC   |  0.9621 |

## Threshold Tuning
- Optimal decision threshold by F1: **0.62**
- Precision: 0.8929
- Recall: 0.8929
- F1: 0.8929
