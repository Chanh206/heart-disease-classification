# Contributing Guide

Thank you for contributing to the Heart Disease Classification project.

This document describes the collaboration workflow, Git conventions, branch strategy, notebook organization, and machine learning experiment standards used in this repository.

---

# Project Overview

This repository contains a machine learning research project focused on predicting heart disease using clinical healthcare data from the UCI Heart Disease Dataset.

The project includes:

- Data preprocessing
- Exploratory Data Analysis (EDA)
- Machine learning model training
- Model evaluation
- ROC curve visualization
- Feature importance analysis
- Final research reporting

---

# Repository Structure

```text
heart-disease-classification/
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_model_training.ipynb
│   └── 03_evaluation.ipynb
│
├── src/
│   ├── preprocess.py
│   ├── train.py
│   ├── evaluate.py
│   └── visualize.py
│
├── reports/
│   └── figures/
│
├── models/
│
├── README.md
├── CONTRIBUTING.md
├── requirements.txt
└── .gitignore
```

---

# Git Workflow

This project follows a lightweight feature-branch workflow to ensure organized collaboration and reproducible machine learning experiments.

---

# Branch Strategy

The repository uses the following branch structure:

```text
main
├── feature/eda
├── feature/model-training
├── feature/evaluation
├── feature/report
└── fix/*
```

---

# Branch Purposes

## `main`

The `main` branch should always contain:

- stable code
- reviewed changes
- reproducible notebooks
- finalized outputs

Avoid committing directly to `main`.

---

## `feature/*`

Feature branches are used for isolated development tasks.

Examples:

```text
feature/eda
feature/model-training
feature/evaluation
feature/report
```

Each branch should focus on a single task or project component.

---

## `fix/*`

Used for bug fixes and corrections.

Examples:

```text
fix/missing-value-handling
fix/data-loading-error
fix/roc-curve-plot
```

---

# Commit Convention

To maintain a clean and readable Git history, contributors should follow the commit naming convention below.

Format:

```text
<type>(<scope>): <description>
```

---

# Commit Types

| Type | Description |
|---|---|
| `feat` | Add new functionality |
| `fix` | Fix bugs or errors |
| `docs` | Documentation updates |
| `style` | Formatting or styling changes |
| `refactor` | Internal code restructuring |
| `test` | Add or update tests |
| `chore` | Maintenance tasks |

---

# Commit Examples

## Feature commits

```text
feat(eda): add correlation heatmap analysis
feat(model): implement random forest classifier
feat(eval): add ROC-AUC evaluation
```

---

## Bug fix commits

```text
fix(preprocess): handle missing values in thal column
fix(eval): correct confusion matrix labels
```

---

## Documentation commits

```text
docs(readme): update project workflow
docs(contributing): improve git workflow documentation
```

---

# Standard Development Workflow

## 1. Update local repository

Before starting work:

```bash
git switch main
git pull origin main
```

---

## 2. Create a feature branch

```bash
git switch -c feature/eda
```

---

## 3. Work on your task

Examples:

- Data preprocessing
- Visualization
- Model training
- Evaluation
- Report writing

---

## 4. Add changes

```bash
git add .
```

---

## 5. Commit changes

```bash
git commit -m "feat(eda): add target distribution analysis"
```

---

## 6. Push branch

```bash
git push -u origin feature/eda
```

---

## 7. Open Pull Request

After finishing your task:

- Open Pull Request
- Request review
- Merge into `main`

---

# Notebook Workflow

Jupyter notebooks can easily create merge conflicts. Contributors should follow these rules:

- Avoid editing the same notebook simultaneously
- Keep notebooks task-specific
- Remove unnecessary outputs before committing
- Use clear notebook names

Recommended notebook structure:

```text
01_eda.ipynb
02_model_training.ipynb
03_evaluation.ipynb
```

---

# Code Style Guidelines

## Python Style

- Follow PEP8 conventions
- Use meaningful variable names
- Avoid duplicated code
- Write modular functions

Good example:

```python
def preprocess_data(df):
    return cleaned_df
```

Avoid:

```python
def x(a):
    return a
```

---

# Data Management Rules

## Raw Data

Original datasets should remain unchanged.

Store raw files inside:

```text
data/raw/
```

---

## Processed Data

Cleaned datasets should be stored separately:

```text
data/processed/
```

Do not overwrite original datasets.

---

# Model Storage

All trained machine learning models should be saved inside:

```text
models/
```

Examples:

```text
random_forest.pkl
svm_model.pkl
```

---

# Visualization Output

All generated figures should be exported to:

```text
reports/figures/
```

Examples:

```text
correlation_heatmap.png
roc_curve.png
feature_importance.png
```

---

# Machine Learning Experiment Tracking

To ensure reproducibility:

- Use fixed random seeds
- Record preprocessing steps
- Document model parameters
- Keep evaluation metrics consistent

Example:

```python
RandomForestClassifier(random_state=42)
```

---

# Pull Request Checklist

Before merging:

- [ ] Code runs correctly
- [ ] Notebook outputs are readable
- [ ] No unnecessary temporary files included
- [ ] Commit messages follow convention
- [ ] Figures exported successfully
- [ ] Branch updated with latest `main`

---

# Collaboration Rules

To reduce merge conflicts:

- Pull latest changes before coding
- Communicate major modifications
- Avoid force-pushing shared branches
- Keep commits small and meaningful

Recommended command before starting work:

```bash
git pull origin main
```

---

# Files That Should Not Be Committed

Avoid committing:

```text
__pycache__/
.ipynb_checkpoints/
*.pkl
*.zip
.~lock*
```

Large temporary files should not be uploaded unless necessary.

---

# Final Deliverables

The final project should contain:

- Clean GitHub repository
- Reproducible machine learning workflow
- EDA notebook
- Model comparison
- ROC curve visualization
- Feature importance analysis
- Final research report

---

# Final Notes

Please keep the repository:

- organized
- reproducible
- readable
- collaborative

All contributors are encouraged to follow the project workflow consistently to maintain code quality and project stability.
