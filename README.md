# Jamboree Admission Chance Prediction using Machine Learning

## Project Overview
This project predicts a student's chance of admission for graduate studies using academic and profile-based features such as GRE Score, TOEFL Score, CGPA, SOP, LOR, University Rating, and Research Experience.

The goal of this project is to build a machine learning regression model that can estimate admission probability and identify the most important factors affecting admissions.

---

## Problem Statement
Jamboree is an education consultancy that helps students with higher education admissions.

This project aims to create a data-driven admission prediction model to estimate a student's probability of getting admitted based on their academic profile.

---

## Dataset Information
The dataset contains 500 student records with the following features:

- GRE Score
- TOEFL Score
- University Rating
- SOP
- LOR
- CGPA
- Research
- Chance of Admit (Target Variable)

### Dataset Summary
- Total Rows: 500
- Total Columns: 8 (after removing Serial No.)
- Missing Values: 0
- Duplicate Records: 0

---

## Tools and Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- SciPy

---

## Project Workflow

### 1. Data Loading and Cleaning
- Loaded the dataset using Pandas
- Removed the Serial No. column
- Checked for missing values, duplicates, and data types

### 2. Exploratory Data Analysis (EDA)
- Generated summary statistics
- Visualized the distribution of the target variable
- Created a correlation heatmap
- Analyzed feature relationships and trends

### 3. Data Preparation
- Defined input features (X) and target variable (y)
- Split the data into training and testing sets (80:20)

### 4. Model Building
Built and compared the following regression models:
- Linear Regression
- Ridge Regression
- Lasso Regression

Also used OLS Regression (Statsmodels) for detailed statistical interpretation.

### 5. Regression Assumption Testing
Checked important regression assumptions:
- Multicollinearity using VIF
- Residual Mean
- Linearity
- Homoscedasticity
- Normality of Residuals

### 6. Model Evaluation
Evaluated the models using:
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R2 Score
- Adjusted R2

---

## Model Performance

### Linear Regression
- MAE: 0.0427
- RMSE: 0.0609
- R2 Score: 0.8188
- Adjusted R2: 0.8051

### Ridge Regression
- MAE: 0.0429
- RMSE: 0.0610
- R2 Score: 0.8180
- Adjusted R2: 0.8041

### Lasso Regression
- MAE: 0.0432
- RMSE: 0.0617
- R2 Score: 0.8138
- Adjusted R2: 0.7997

### Best Model
- Linear Regression performed best with R2 = 0.82

---

## Key Insights
- CGPA is the most important factor affecting admission chances
- GRE Score and TOEFL Score also have a strong impact
- Research Experience gives a positive boost to admission probability
- University Rating and SOP showed lower significance in this model
- High VIF values indicate multicollinearity among some academic features

---

## Business Impact
This project can help education consultants:
- Provide realistic admission predictions to students
- Identify key profile strengths and weaknesses
- Offer personalized improvement suggestions
- Support data-driven counseling and decision-making

---

## Project Structure
Jamboree-Admission-Prediction/
│── Jamboree_Admission.csv
│── Jamboree_Admission_Prediction.ipynb
│── README.md

---

## How to Run the Project

1. Clone the repository:
git clone <your-repository-link>

2. Install required libraries:
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels scipy

3. Launch Jupyter Notebook:
jupyter notebook

4. Open the notebook file and run all cells

---

## Future Improvements
- Apply advanced models like Random Forest Regressor and XGBoost
- Perform feature engineering
- Build a simple web app for admission prediction
- Add real-time user input for predictions

---

## Conclusion
This project successfully built a machine learning regression model to predict graduate admission chances with around 82 percent accuracy (R2 = 0.82).

The analysis shows that CGPA, GRE, TOEFL, and Research Experience are the most influential factors in predicting admission probability.

This project demonstrates the use of data cleaning, EDA, regression modeling, model evaluation, and statistical diagnostics to solve a real-world education analytics problem.
