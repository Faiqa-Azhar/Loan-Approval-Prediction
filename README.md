# Loan Approval Prediction using Logistic Regression

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Logistic%20Regression-green)
![Status](https://img.shields.io/badge/Project-Completed-success)

## Project Overview

This project predicts whether a loan application will be **approved or rejected** using **Machine Learning**. The system uses **Logistic Regression**, a supervised learning algorithm suitable for binary classification problems.

The project includes complete data preprocessing, missing value handling, categorical encoding, feature scaling, dataset balancing using SMOTE, model training, evaluation, visualization, and model saving.


## Objectives

- Predict loan approval status
- Preprocess and clean loan data
- Handle missing values
- Encode categorical features
- Balance dataset using SMOTE
- Train Logistic Regression model
- Evaluate model performance
- Visualize model accuracy
- Save trained model


## Technologies Used

### Language
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Imbalanced-Learn (SMOTE)
- Joblib


## Dataset Information

The dataset contains applicant details such as:

- Gender
- Marital Status
- Dependents
- Education
- Employment Status
- Applicant Income
- Co-applicant Income
- Loan Amount
- Loan Term
- Credit History
- Property Area

### Target Variable

`Loan_Status`

- **1 → Approved**
- **0 → Rejected**


## Machine Learning Workflow

### 1. Load Dataset
Dataset is loaded using Pandas.

```python
df = pd.read_csv(file_path)
```

### 2. Data Preprocessing
- Remove unnecessary columns (`Loan_ID`)
- Handle missing values
- Encode categorical variables
- Encode target labels (`Y → 1`, `N → 0`)

### 3. Handle Imbalanced Data
Dataset balancing is performed using **SMOTE**.

### 4. Feature Scaling
Features are normalized using:

```python
StandardScaler()
```

### 5. Train-Test Split
Dataset is divided into:

- **80% Training Data**
- **20% Testing Data**

### 6. Model Training
The project uses only:

### Logistic Regression

A suitable algorithm for binary classification tasks.

### 7. Model Evaluation
Performance is evaluated using:

- Accuracy Score
- Log Loss
- Classification Report
- Confusion Matrix

### 8. Accuracy Visualization
A **line graph** compares:

- Training Accuracy
- Testing Accuracy

to analyze model performance.

### 9. Save Model

```python
joblib.dump(model, 'loan_approval_model.pkl')
```


##  Project Output

The project generates:

✅ Loan approval predictions  
✅ Training & testing accuracy  
✅ Classification report  
✅ Confusion matrix  
✅ Accuracy line graph  
✅ Saved trained model (`.pkl`)


## Project Structure

```text
Loan-Approval-Prediction/
│── loan_data_1.csv
│── loan_prediction.ipynb
│── loan_approval_model.pkl
│── README.md
```


## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/loan-approval-prediction.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```


## Run the Project

```bash
python loan_prediction.py
```

Or run the Jupyter Notebook.


## Conclusion

This project successfully implements a **Loan Approval Prediction System using Logistic Regression**. The model predicts loan approval based on applicant information after applying preprocessing techniques such as missing value handling, categorical encoding, SMOTE balancing, and feature scaling.

The Logistic Regression model provides reliable prediction performance and demonstrates how Machine Learning can improve decision-making in loan approval systems.


## Author

**Faiqa Azhar**  
Data Science Student
