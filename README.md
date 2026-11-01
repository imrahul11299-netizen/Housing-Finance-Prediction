# Housing Finance Prediction Using Machine Learning

**Academic project | Data Analytics Programme, IIM Sirmaur × Masai**

## Overview

This project explores whether applicant and financial attributes can be used to classify housing finance decisions. A Decision Tree Classifier was developed and evaluated as part of a learning project.

## Business Question

Can historical applicant information help classify a housing finance decision, and how should the model's performance be evaluated before any real-world use?

## Project Objectives

- Inspect and prepare the dataset.
- Encode categorical variables for model training.
- Separate the data into training and test sets.
- Train a Decision Tree Classifier.
- Evaluate predictions with accuracy and a confusion matrix.
- Explore hyperparameter tuning using cross-validation.

## Dataset and Files

- `HousingFinance1.csv` — dataset used for the analysis.
- `HousingFinance1.pdf` — report containing the workflow, code, visualizations, and results.

The dataset is reported to contain **1,570 records and 23 original columns**. Confirm the dataset's source, licensing, and variable definitions before redistributing it or using it beyond coursework.

## Tools

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- scikit-learn
- Google Colab

## Methodology

1. Load and inspect the dataset.
2. Review missing values and variable types.
3. Encode categorical variables.
4. Define `Decision` as the target variable.
5. Split data into training and test subsets using an 80:20 ratio (`random_state=10`).
6. Train a Decision Tree Classifier.
7. Evaluate the model and visualize its confusion matrix.
8. Use `GridSearchCV` with cross-validation to explore model settings.

## Results Reported in the Coursework

- Initial test-set accuracy: **approximately 80.57%**
- Best cross-validation score during tuning: **approximately 84.87%**

These scores come from different evaluation procedures and should not be compared as if they were the same metric. Re-run the analysis to verify the values before relying on them in a presentation or interview.

## Interpretation and Business Relevance

A classifier like this could be studied as a decision-support aid, but accuracy alone does not show whether the model is fair, calibrated, or safe for lending decisions. False approvals and false rejections can have different consequences, so class-specific precision, recall, confusion-matrix results, and subgroup performance should also be examined.

## How to Review the Project

1. Open `HousingFinance1.pdf` and review the documented workflow and code.
2. Inspect `HousingFinance1.csv` and verify the target and input variables.
3. Re-run the code in Google Colab or a local Python environment.
4. Confirm the reported results and correct any code or evaluation issues before extending the model.

## Limitations

- This is an academic analysis, not a validated lending system.
- The reported metrics do not establish performance on new real-world applicants.
- The original tuning workflow should be reviewed for invalid parameter values and failed fits; only valid, successful runs should be included in final results.
- Lending-related models require careful fairness, privacy, explainability, and regulatory review.

## Project Status

**Academic project / prototype.** No live production deployment or real lending decision use is claimed.

## Learning Outcomes

Data preparation, categorical encoding, decision-tree classification, train/test evaluation, confusion-matrix interpretation, and cross-validation.

## Author

Rahul | [GitHub Profile](https://github.com/imrahul11299-netizen)

