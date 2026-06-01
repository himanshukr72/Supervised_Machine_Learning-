# Supervised_Machine_Learning-
This repo contains all the concept related labs which i performed on supervised machine learning


# Employee Attrition Prediction using Machine Learning

## Project Overview

Employee attrition is a major concern for organizations due to the costs associated with recruitment, training, and loss of productivity. This project aims to predict whether an employee is likely to leave the organization using supervised machine learning classification techniques.

The analysis evaluates multiple machine learning models and identifies the most effective approach for predicting employee attrition. The insights generated can help Human Resource (HR) departments implement targeted retention strategies and improve workforce stability.

---

## Business Objective

The primary objective of this project is to:

- Predict employee attrition (Yes/No)
- Identify the key factors influencing employee turnover
- Compare multiple classification models
- Recommend the best-performing model for deployment
- Provide actionable HR recommendations for employee retention

---

## Dataset

**Dataset:** IBM HR Analytics Employee Attrition & Performance Dataset

### Dataset Information

- Total Records: 1,470
- Features: 35
- Target Variable: `Attrition`

### Target Classes

| Value | Meaning |
|---------|---------|
| Yes | Employee Left |
| No | Employee Stayed |

### Key Features

- Age
- MonthlyIncome
- JobRole
- OverTime
- WorkLifeBalance
- JobSatisfaction
- EnvironmentSatisfaction
- YearsAtCompany
- TotalWorkingYears
- DistanceFromHome

---

## Project Workflow

### 1. Data Understanding

- Dataset exploration
- Feature analysis
- Target variable inspection

### 2. Data Preprocessing

- Missing value analysis
- Removal of non-informative features
- Label encoding of categorical variables
- Feature scaling
- Train-test split

### 3. Exploratory Data Analysis (EDA)

- Attrition distribution
- Overtime vs Attrition
- Job Satisfaction analysis
- Monthly Income analysis
- Correlation heatmap

### 4. Model Development

The following classification algorithms were implemented:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Gradient Boosting Classifier

### 5. Model Evaluation

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### 6. Feature Importance Analysis

Random Forest feature importance was used to identify the most influential predictors of attrition.

---

## Technologies Used

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn


## Results

The machine learning models were evaluated using Accuracy, Precision, Recall, and F1-Score.

| Model | Accuracy | Precision | Recall | F1 Score |
|---------|---------|---------|---------|---------|
| Logistic Regression | 0.8450 | 0.5157 | 0.3905 | 0.4444 |
| Decision Tree | 0.7823 | 0.3143 | 0.3143 | 0.3143 |
| Random Forest | 0.8496 | 0.6410 | 0.1190 | 0.2008 |
| Gradient Boosting | 0.8428 | 0.5093 | 0.2619 | 0.3459 |

### Best Performing Model

Based on the evaluation metrics, **Logistic Regression** achieved the highest F1-Score (0.4444), indicating the best balance between Precision and Recall for identifying employee attrition.

Although Random Forest achieved the highest Accuracy (84.96%), its Recall was significantly lower, making it less effective at detecting employees who are likely to leave.

Therefore, **Logistic Regression is recommended as the final model for employee attrition prediction**.

---

## Feature Importance Analysis

Feature importance analysis identified the following variables as the most influential predictors of employee attrition:

| Rank | Feature | Importance |
|--------|---------|------------|
| 1 | MonthlyIncome | 0.0831 |
| 2 | Age | 0.0824 |
| 3 | DistanceFromHome | 0.0657 |
| 4 | DailyRate | 0.0624 |
| 5 | MonthlyRate | 0.0577 |
| 6 | HourlyRate | 0.0565 |
| 7 | YearsInCurrentRole | 0.0479 |
| 8 | NumCompaniesWorked | 0.0433 |
| 9 | JobRole | 0.0429 |
| 10 | TotalWorkingYears | 0.0425 |

### Interpretation

- Employees with lower income levels were more likely to leave the organization.
- Employee age was a significant factor influencing attrition behavior.
- Longer commuting distances were associated with increased turnover.
- Compensation-related variables (DailyRate, MonthlyRate, HourlyRate) played an important role in employee retention.
- Career progression indicators such as YearsInCurrentRole and TotalWorkingYears influenced attrition likelihood.
- Employees who had worked at multiple companies previously showed higher attrition tendencies.

---

## Key Findings

### Finding 1
Monthly income was the most influential feature, suggesting that compensation plays a major role in employee retention.

### Finding 2
Age and total work experience significantly affected employee turnover patterns.

### Finding 3
Employees living farther from the workplace were more likely to leave.

### Finding 4
Employees with a history of working at multiple organizations demonstrated higher attrition risk.

### Finding 5
Role-specific characteristics and career growth opportunities influenced employee retention decisions.

---

## Business Recommendations

### 1. Review Compensation Policies
Evaluate salary competitiveness and compensation packages to improve retention among high-risk employees.

### 2. Improve Employee Career Development
Create clear promotion paths and professional growth opportunities to increase engagement.

### 3. Support Employees with Long Commutes
Consider hybrid work options, transportation benefits, or flexible schedules.

### 4. Focus on Early Attrition Prevention
Implement onboarding and mentoring programs for employees in their early years with the organization.

### 5. Develop Data-Driven Retention Strategies
Use predictive analytics to proactively identify employees at risk of leaving and intervene before attrition occurs.

---
