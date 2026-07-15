# HR Employee Attrition Analysis & Prediction

## Project Status: ML Phase Complete ✅

## Overview
End-to-end data science project analyzing and predicting 
employee attrition using IBM HR Analytics dataset. 
The project covers data cleaning, exploratory data analysis, 
and machine learning modelling to identify at-risk employees.

## Dataset
- Source: IBM HR Analytics Employee Attrition (Kaggle)
- Size: 1,470 employees | 35 features
- Target: Predict whether an employee will leave or stay

## Tools & Technologies
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Machine Learning (Scikit-learn)
- MySQL
- Git & GitHub

## Project Phases

### Phase 1: Data Cleaning ✅
- Loaded raw dataset (1,470 rows, 35 columns)
- Removed 3 redundant columns (EmployeeCount, StandardHours, Over18)
- Confirmed zero null values and zero duplicates
- Created AttritionFlag (0/1) for ML modelling
- Created EducationLabel for visualization

### Phase 2: Exploratory Data Analysis ✅
- Created 11 analytical visualizations
- Key Findings:
  - Overall attrition rate: 16%
  - Overtime employees show 3x higher attrition (30% vs 10%)
  - Sales department has highest attrition rate
  - Age group 18-25 most vulnerable segment
  - Low salary band shows highest attrition
  - Bad work-life balance leads to 31.25% attrition
  - Low job satisfaction leads to 22.84% attrition
  - Distance from home positively correlated with attrition

### Phase 3: Machine Learning ✅
- Applied Label Encoding on 7 categorical features
- Performed 80/20 train-test split with stratification
- Applied StandardScaler for feature scaling
- Models built and compared:

| Model | Accuracy | AUC Score |
|-------|----------|-----------|
| Logistic Regression | 87.41% | 0.806 |
| Random Forest + SMOTE | 79.93% | — |

- Selected Logistic Regression as final model
- Applied SMOTE to handle class imbalance (84:16 ratio)
- Top attrition predictors identified via feature importance:
  1. Stock Option Level
  2. Job Satisfaction
  3. Monthly Income
  4. Environment Satisfaction
  5. Age

### Phase 4: Power BI Dashboard (Planned)
### Phase 5: Business Report (Planned)

## Key Business Insights
- Overtime is the single biggest controllable attrition driver
- Stock options are the strongest retention tool
- First year employees are highest risk — onboarding is critical
- Sales department needs immediate retention strategy
- Low salary band requires compensation review

## ML Results
- Final Model: Logistic Regression
- Accuracy: 87.41%
- AUC Score: 0.806
- Correctly identified 18 out of 47 at-risk employees
- Reason for selection: Higher accuracy and F1 score vs Random Forest

## Repository Structure
