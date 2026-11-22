# Loan Approval Prediction using Logistic Regression

**Activity:** Loan Approval Prediction  
**Roll Number:** AD3203  
**Algorithm:** Logistic Regression  
**Project Type:** Machine Learning – Binary Classification

---

## 1. Project Overview

This project implements a Machine Learning classification model using **Logistic Regression** to predict whether a loan application is likely to be approved or rejected.

The model uses applicant information such as income, education, marital status, credit history, loan amount, employment status, and property area to estimate loan approval probability.

The project demonstrates a complete Machine Learning workflow, including data loading, exploratory data analysis, preprocessing, model training, probability prediction, model evaluation, and prediction for a new applicant.

## 2. Project Objectives

- Explore and understand the Loan Prediction dataset.
- Identify numerical and categorical features.
- Handle missing values using appropriate imputation techniques.
- Encode categorical variables using One-Hot Encoding.
- Scale numerical features using StandardScaler.
- Train a Logistic Regression classification model.
- Evaluate model performance using classification metrics.
- Generate loan approval probabilities for new applicants.

## 3. Dataset Information

**Dataset:** `train_u6lujuX_CVtuZ9i.csv`

- Total records: 614
- Total columns: 13
- Target variable: `Loan_Status`

### Dataset Features

| Feature | Description |
|---|---|
| Loan_ID | Loan application identifier |
| Gender | Applicant gender |
| Married | Marital status |
| Dependents | Number of dependents |
| Education | Education level |
| Self_Employed | Employment status |
| ApplicantIncome | Applicant income |
| CoapplicantIncome | Co-applicant income |
| LoanAmount | Requested loan amount |
| Loan_Amount_Term | Loan repayment term |
| Credit_History | Credit history indicator |
| Property_Area | Property location category |
| Loan_Status | Loan approval status |

### Target Variable Encoding

- `Y` = 1 (Loan Approved)
- `N` = 0 (Loan Rejected)

**Note:** The original publisher and dataset source URL were not identified in the supplied notebook. Add the verified source if provided by your faculty.

## 4. Technologies and Libraries Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- Jupyter Notebook

## 5. Project Workflow

1. Imported the required Python libraries.
2. Uploaded and loaded the dataset.
3. Performed initial data inspection.
4. Checked missing values and duplicate records.
5. Performed Exploratory Data Analysis (EDA).
6. Visualized loan approval class distribution.
7. Removed the `Loan_ID` column from model features.
8. Separated independent variables (X) and target variable (y).
9. Identified numerical and categorical columns.
10. Handled missing values using SimpleImputer.
11. Applied StandardScaler to numerical features.
12. Applied OneHotEncoder to categorical features.
13. Created preprocessing pipelines using ColumnTransformer.
14. Split the dataset into training and testing sets (80:20).
15. Used stratified sampling with random_state=42.
16. Illustrated the Logistic Regression sigmoid function.
17. Trained the Logistic Regression model.
18. Examined model coefficients and intercept.
19. Generated predicted probabilities and class labels.
20. Evaluated model performance using classification metrics.
21. Compared model accuracy with a majority-class baseline.
22. Visualized the confusion matrix and ROC curve.
23. Tested the model with a sample new applicant.

## 6. Model Configuration

| Parameter | Value |
|---|---|
| Algorithm | Logistic Regression |
| Training Data | 80% |
| Testing Data | 20% |
| Random State | 42 |
| Stratification | Enabled |
| Maximum Iterations | 1000 |
| Decision Threshold | 0.5 |

## 7. Model Evaluation and Results

The trained model was evaluated on 123 test records.

### Performance Metrics

| Evaluation Metric | Score |
|---|---:|
| Accuracy | 86.18% |
| Precision | 84.00% |
| Recall | 98.82% |
| Specificity | 57.89% |
| F1-Score | 90.81% |
| ROC-AUC | 0.8523 |

### Confusion Matrix

| Actual / Predicted | Rejected | Approved |
|---|---:|---:|
| Actual Rejected | 22 | 16 |
| Actual Approved | 1 | 84 |

### Baseline Comparison

- Majority-class baseline accuracy: 69.11%
- Logistic Regression test accuracy: 86.18%

The Logistic Regression model achieved higher accuracy than the majority-class baseline.

## 8. Sample Applicant Prediction

The model was tested using the following sample applicant information:

| Feature | Value |
|---|---|
| Gender | Male |
| Married | Yes |
| Dependents | 1 |
| Education | Graduate |
| Self Employed | No |
| Applicant Income | 5000 |
| Co-applicant Income | 2000 |
| Loan Amount | 150 |
| Loan Amount Term | 360 |
| Credit History | 1 |
| Property Area | Urban |

### Prediction Output

- Predicted approval probability: **73.96%**
- Predicted result: **Loan Approved**

This is an example prediction from the trained model and does not represent an actual lending decision.

## 9. Data Visualizations

The notebook includes the following visualizations:

- Loan approval class distribution.
- Logistic Regression sigmoid function.
- Confusion matrix heatmap.
- ROC curve.
- Loan approval probability versus applicant income.

## 10. Repository Structure

```text
Loan-Approval-Prediction-Logistic-Regression-AD3203/
│
├── Loan_Approval_Prediction_Logistic_Regression.ipynb
├── train_u6lujuX_CVtuZ9i.csv
└── README.md
```

**Important:** Upload the CSV file only if its redistribution is permitted by your faculty or the dataset's license. Otherwise, provide instructions for obtaining the dataset separately.

## 11. How to Run the Project

### Option 1: Google Colab

1. Open the `.ipynb` notebook in Google Colab.
2. Run the notebook cells sequentially.
3. Upload the required CSV dataset when prompted.
4. Execute all cells.
5. Review the data analysis, evaluation metrics, visualizations, and sample prediction.

### Option 2: Local Environment

Install the required libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the project notebook and execute the cells.

**Note:** The notebook uses `google.colab.files` for dataset uploading. For local execution, replace the Google Colab upload code with a local CSV file path.

## 12. GitHub Submission

**GitHub Submission ID:** https://github.com/bhavikakadam7

**Student Roll Number:** AD3203

**Individual Repository URL:** https://github.com/bhavikakadam7/Loan-Approval-Prediction-Logistic-Regression-AD3203


## 13. Conclusion

This project successfully demonstrates the application of Logistic Regression for predicting loan approval using applicant information.

The model achieved **86.18% test accuracy** and an **ROC-AUC score of 0.8523**. Data preprocessing, feature encoding, feature scaling, model training, and evaluation were performed as part of the Machine Learning workflow.

The project provides practical experience in binary classification and predictive modelling using Python and Scikit-learn.

**Disclaimer:** This project is developed for educational purposes only. Predictions may reflect biases in historical data and should not be used as the sole basis for real-world financial or loan approval decisions.

---

**Activity:** Loan Approval Prediction  
**Roll Number:** AD3203  
**Algorithm:** Logistic Regression  
**Project Domain:** Machine Learning
Submission GitHub ID: [https://github.com/complexiota](https://github.com/complexiota)
