# 🏠 Housing Finance Prediction Using Machine Learning

## 📌 Project Overview

This project focuses on predicting housing finance approval decisions using a Decision Tree Classification model. It was developed as part of the **Data Analytics Programme at IIM Sirmaur × Masai**.

The project uses applicant-related information, including age, income, employment type, loan requirements, property value, and financial indicators, to classify housing finance decisions.

## 🎯 Objectives

* Analyze housing finance applicant data.
* Clean and preprocess the dataset.
* Encode categorical variables into numerical format.
* Split the data into training and testing sets.
* Build a Decision Tree Classification model.
* Evaluate the model using accuracy and a confusion matrix.
* Apply hyperparameter tuning to identify a suitable model configuration.

## 📂 Project Files

* `HousingFinance1.csv` — Dataset used for model development.
* `HousingFinance1.pdf` — Project report containing code, workflow, visualizations, and results.

## 🛠️ Technologies Used

* **Python:** Programming language used for data analysis and machine learning.
* **Pandas:** Data manipulation and dataset handling.
* **NumPy:** Numerical operations.
* **Matplotlib:** Data visualization.
* **Seaborn:** Statistical visualizations.
* **Scikit-learn:** Model building, data splitting, evaluation, and hyperparameter tuning.
* **Google Colab:** Environment used to execute the Python code.

## ⚙️ Project Workflow

### 1. Data Preprocessing

Imported the dataset using Pandas and examined its structure, summary statistics, and missing values.

### 2. Data Encoding

Converted categorical variables into numerical representations using label encoding and dummy variables. This allowed the machine learning model to process categorical information.

### 3. Feature Selection

Selected applicant and financial attributes as input features. The target variable was `Decision`, representing the housing finance decision.

### 4. Train-Test Split

Split the dataset into training and testing sets using an 80:20 ratio and `random_state=10`.

### 5. Decision Tree Classification

Built a Decision Tree Classifier with `max_depth=2` and trained it on the training data.

### 6. Model Evaluation

Evaluated predictions using accuracy and a confusion matrix. A heatmap was also created to visualize the classification results.

### 7. Hyperparameter Tuning

Used `GridSearchCV` with 10-fold cross-validation to explore different decision tree criteria and maximum depths.

## 📊 Results

* **Dataset size:** 1,570 records.
* **Number of original dataset columns:** 23.
* **Initial Decision Tree accuracy:** Approximately 80.57%.
* **Best cross-validation score reported during tuning:** Approximately 84.87%.

The initial accuracy was measured on the test set. The 84.87% score was the best cross-validation score reported by the tuning process. These are different evaluation measures and should not be treated as directly equivalent.

## 📈 Confusion Matrix

The initial model produced the following confusion matrix:

| Actual Class | Predicted 0 | Predicted 1 |
| ------------ | ----------: | ----------: |
| 0            |          20 |          52 |
| 1            |           9 |         233 |

The matrix shows the number of correct and incorrect classifications for each class.

## 🚀 Key Learnings

* Data preprocessing and categorical encoding.
* Feature selection and train-test splitting.
* Decision Tree classification.
* Model evaluation using accuracy and a confusion matrix.
* Hyperparameter tuning using cross-validation.
* Visualizing machine learning results.

## ▶️ How to Run

1. Clone or download this repository.
2. Open the project in Google Colab or Jupyter Notebook.
3. Upload `HousingFinance1.csv`.
4. Update the dataset file path in the Python code.
5. Install any missing Python libraries.
6. Execute the code cells in the order shown in the project report.

## ⚠️ Limitations

* The reported results do not establish how the model performs on entirely new real-world applicants.
* The hyperparameter tuning code contains an invalid criterion value (`entorpy` instead of `entropy`), which caused some model fits to fail.
* The model should be further evaluated and validated before any real lending decision.

## 👨‍🎓 Project Information

**Programme:** Data Analytics Programme
**Institution:** IIM Sirmaur × Masai
**Project:** Housing Finance Prediction
**Primary Algorithm:** Decision Tree Classifier
**Language:** Python

