# Supervised Learning Competition — Student Performance Prediction

## Overview
This repository contains the code, report, and predictions for **Assignment 3: Supervised Learning Competition**. The task is framed as a "common task framework" (benchmark-style) machine learning competition: predict a continuous student performance variable (`score`) from a set of student characteristics.

- **Target variable:** `score`
- **Performance metric:** Mean Squared Error (MSE)
- **Prediction output:** 79 numeric values (one per test-set student)

## Task Summary
1. Choose **two or more** appropriate prediction methods (e.g., linear regression, KNN, regression tree, or any other suitable method).
2. Train and evaluate the models' predictive ability on the training data using techniques covered in the course.
3. Select the best-performing model based on the evaluation/comparison study and generate predictions for the test set.
4. Save predictions as a single numeric vector of length 79 in `predictions.rds`.
5. Communicate the full workflow in a written report.

## Data
- `train.rds` — training data, includes the target variable `score`
- `test.rds` — test data, target variable withheld

## Repository Structure
```
.
├── README.md                # This file
├── report.qmd                # Quarto source for the written report
├── report.html                # Rendered report (or .pdf)
├── data/
│   ├── train.rds
│   └── test.rds
├── predictions.rds            # Final predicted scores for the test set (79 values)
└── scripts/                   # Any additional analysis/modeling scripts
```

## Report Contents
The written report (`report.qmd`) covers:
- **Data description & exploration** — summary statistics and a visualization of the data
- **Model overview** — the prediction methods compared and rationale for choosing them
- **Pre-processing** — steps such as handling categorical variables, scaling, and feature engineering
- **Model comparison methodology** — how and why the models were evaluated against each other
- **Final model selection** — which method performed best and why
- **Team contributions** — summary of each team member's role in the project

## Reproducibility
The project is designed to be computationally reproducible:
1. Clone this repository.
2. Open `report.qmd` in RStudio (or another Quarto-compatible environment).
3. Install any required packages listed at the top of the `.qmd` file.
4. Click **Render** (or run `quarto render report.qmd`) to regenerate the report from scratch.

## Notes
- This assignment was completed without the use of AI tools or AutoML systems, per the assignment guidelines.
- Grading is based on code quality (20%), report content (70%), and prediction performance relative to baseline models (10%).
