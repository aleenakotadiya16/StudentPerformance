# 🎓 Student Performance Predictor - ML End-to-End Project
## **📌 Objective**
This project aims to predict the Math score of students based on various demographic and academic features. It leverages several regression models and selects the best-performing one through model evaluation and hyperparameter tuning.

## **🧠 Problem Statement**
We are given a dataset containing student information such as:

Gender

Race/Ethnicity

Parental Level of Education

Lunch Type

Test Preparation Course

Reading Score (out of 100)

Writing Score (out of 100)

Our goal is to predict the Math Score (out of 100) using the above variables.

## **🛠️ Technologies Used**
Python

Pandas, NumPy, Scikit-learn

XGBoost, CatBoost, LightGBM

Matplotlib, Seaborn (for EDA and visualization)

Jupyter Notebook

Flask ( for deployment)



## **🔍 Workflow**
1. Data Collection
Dataset used: Student Performance Dataset (from open sources like Kaggle or UCI)

2. Data Preprocessing
Handling missing values

Encoding categorical variables

Feature scaling

3. Exploratory Data Analysis (EDA)
Univariate & Bivariate analysis

Correlation heatmap

Distribution plots of scores

## **4. Model Building**
We test multiple regression models:

models = {
    "Linear Regression": LinearRegression(),
    "Decision Tree": DecisionTreeRegressor(),
    "Random Forest": RandomForestRegressor(),
    "Gradient Boosting": GradientBoostingRegressor(),
    "XGBoost": XGBRegressor(),
    "CatBoost": CatBoostRegressor(verbose=False),
    "AdaBoost": AdaBoostRegressor(),
}

## **5. Model Evaluation**
Evaluation Metrics: R² Score

Train-test split used for validation

## **6. Hyperparameter Tuning**
GridSearchCV/RandomizedSearchCV used for optimizing best models

## **7. Final Model Selection**
The best model is selected based on cross-validated R² score and performance on unseen data.

## **8. Deployment**
The trained model can be deployed using Flask
