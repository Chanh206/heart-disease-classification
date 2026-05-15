# Contributing Guide

Thank you for contributing to the Heart Disease Classification project.

This document explains how team members should work with Git, branches, commits, and pull requests during the project.

---

## Project Workflow

All team members should avoid committing directly to the `main` branch.

The `main` branch should only contain stable and reviewed code.

---

## Branch Strategy

Use the following branch structure:

```text
main
├── feature/eda
├── feature/model-training
├── feature/evaluation
└── feature/report
---

# Repository Structure

The repository is organized as follows:

```text
data/               # raw and processed datasets
notebooks/          # Jupyter notebooks for experiments
src/                # reusable Python scripts
reports/            # generated figures and outputs
models/             # trained machine learning models
