# Heart Disease Classification Using Machine Learning

## Overview

This project focuses on the development and evaluation of machine learning models for heart disease prediction using clinical healthcare data from the UCI Heart Disease Dataset.

The primary objective is to compare multiple classification algorithms and identify the most effective model for predicting the presence of heart disease based on patient clinical features.

This project was developed as part of a Scientific Research Methodology course in the field of Medical Healthcare AI.

---

# Research Objectives

* Perform exploratory data analysis (EDA) on clinical heart disease data
* Preprocess and clean medical tabular data
* Train and compare multiple machine learning classification models
* Evaluate model performance using standard classification metrics
* Analyze feature importance and clinical relevance
* Generate visualization outputs for research reporting

---

# Dataset

## UCI Heart Disease Dataset

Source:

* UCI Machine Learning Repository

Dataset characteristics:

* Clinical healthcare tabular dataset
* Binary classification problem
* Target:

  * 0 = No heart disease
  * 1 = Heart disease

Features include:

* Age
* Sex
* Chest pain type
* Resting blood pressure
* Cholesterol
* Fasting blood sugar
* Maximum heart rate achieved
* Exercise induced angina
* ST depression
* Number of major vessels
* Thalassemia

---

# Machine Learning Pipeline

## 1. Data Collection

* Download dataset from UCI repository
* Convert raw `.data` file into structured dataframe

## 2. Data Preprocessing

* Handle missing values
* Feature scaling using StandardScaler
* Convert target into binary classification labels

## 3. Exploratory Data Analysis

* Correlation heatmap
* Feature distribution analysis
* Target class distribution
* Statistical summaries

## 4. Model Training

The following machine learning models are implemented:

* Logistic Regression
* Random Forest Classifier
* Support Vector Machine (SVM)

## 5. Model Evaluation

Evaluation metrics:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC score

## 6. Explainability

* Feature importance analysis
* ROC curve visualization

---

# Project Structure

```text
heart-disease-classification/
├── data/
│   ├── raw/
│   │   └── heart.csv
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
│       ├── correlation_heatmap.png
│       ├── roc_curve.png
│       └── feature_importance.png
│
├── models/
│   └── random_forest.pkl
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

# Installation

## Clone repository

```bash
git clone https://github.com/YOUR_USERNAME/heart-disease-classification.git
cd heart-disease-classification
```

---

## Create environment

### Using venv

```bash
python -m venv venv
source venv/bin/activate
```

---

## Install dependencies

```bash
pip install -r requirements.txt
```

---

# Requirements

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
joblib
```

---

# Example Workflow

## Run notebook

```bash
jupyter notebook
```

---

## Train models

```bash
python src/train.py
```

---

## Evaluate performance

```bash
python src/evaluate.py
```

---

# Expected Outputs

The final project includes:

* Comparative machine learning model analysis
* ROC curve visualization
* Feature importance visualization
* Research report (10–15 pages)
* Performance evaluation table

---

# Sample Research Questions

* Which machine learning model performs best for heart disease prediction?
* Which clinical features contribute most strongly to prediction?
* Can simple clinical measurements effectively predict heart disease risk?

---

# Limitations

* Small dataset size
* Public dataset may not fully represent real-world clinical populations
* No external validation dataset
* Limited interpretability compared to real clinical decision systems

---

# Future Improvements

Potential future extensions:

* Hyperparameter optimization
* Cross-validation
* Explainable AI using SHAP
* Deep learning approaches
* Deployment as a web application

---

# Team Workflow

## Branch Strategy

```text
main
├── feature/eda
├── feature/model-training
├── feature/evaluation
└── feature/report
```

---

## Recommended Git Workflow

### Create new branch

```bash
git switch -c feature/your-feature-name
```

### Commit changes

```bash
git add .
git commit -m "Add EDA notebook"
```

### Push branch

```bash
git push -u origin feature/your-feature-name
```

---

# Authors

* Data Science Research Team
* Scientific Research Methodology Course

---

# License

This project is developed for academic and educational purposes.

---

# Acknowledgements

* UCI Machine Learning Repository
* Scikit-learn documentation
* Open-source machine learning community

