# House Price Prediction using Linear Regression

## Project Overview

This project focuses on predicting house prices using Machine Learning. The Ames Housing dataset from Kaggle was used to build a regression model that predicts the sale price of residential properties based on various house characteristics.

The project demonstrates a complete machine learning workflow, starting from data exploration and preprocessing to model training, evaluation, visualization, and model comparison.

## Objective

The main objective of this project is to:

- Explore and understand the housing dataset.
- Analyze the distribution of house prices.
- Identify important features related to house prices.
- Handle missing values.
- Encode categorical variables using One-Hot Encoding.
- Build a Linear Regression model.
- Evaluate the model using MSE, RMSE, and R².
- Visualize actual and predicted house prices.
- Analyze model residuals and coefficients.
- Compare Linear Regression with Ridge Regression.

## Dataset

The project uses the **Ames Housing Dataset** from Kaggle's House Prices: Advanced Regression Techniques competition.

The training dataset contains:

- **1,460 rows**
- **81 columns**

The target variable is:

```text
SalePrice


Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Jupyter Notebook

Machine Learning Workflow
1. Data Loading

The dataset was loaded using Pandas and examined using basic DataFrame operations.

2. Exploratory Data Analysis

The dataset was analyzed using:

Shape and column information
Data types
Missing-value analysis
Descriptive statistics
SalePrice distribution
Correlation analysis
Correlation heatmap
3. Feature Selection

Important potential predictors included:

OverallQual
GrLivArea
GarageCars
GarageArea
TotalBsmtSF
1stFlrSF
FullBath
YearBuilt
Neighborhood
LotArea
4. Data Preprocessing

Numerical missing values were handled using median imputation.

Categorical missing values were handled using the most frequent value.

Categorical variables were converted into numerical variables using One-Hot Encoding.

The Id column was removed because it is an identifier rather than a meaningful house characteristic.

5. Train-Test Split

The dataset was divided into:

80% training data
20% testing data

A random_state of 42 was used to make the split reproducible.

6. Linear Regression

A Linear Regression model was trained using a Scikit-learn preprocessing and modeling pipeline.

7. Model Evaluation

The Linear Regression model achieved the following results on the test dataset:

Metric	Result
MSE	979,376,460.09
RMSE	31,294.99
R² Score	0.8723

The R² score indicates that the model explains approximately 87.23% of the variation in house sale prices in this test set.

8. Model Visualization

The project includes:

Actual vs Predicted House Prices plot
Residual Plot
Correlation Heatmap

These visualizations help evaluate the relationship between the input features, actual prices, predicted prices, and prediction errors.

9. Coefficient Analysis

The coefficients of the Linear Regression model were analyzed to understand the direction of association between transformed features and predicted house prices.

10. Ridge Regression

As a bonus experiment, Ridge Regression was also implemented.

Results with alpha=1.0:

Metric	Ridge Regression
MSE	1,194,778,185.40
RMSE	34,565.56
R² Score	0.8442
Project Structure
House_Price_Prediction/
│
├── house_price_prediction.ipynb
├── train.csv
├── test.csv
├── data_description.txt
├── sample_submission.csv
└── README.md
Conclusion

This project demonstrates an end-to-end machine learning workflow for a regression problem. It covers data exploration, missing-value handling, feature selection, categorical encoding, model training, evaluation, visualization, coefficient analysis, and comparison with a regularized regression model.

The project provided practical experience with Python, Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn while demonstrating how machine learning can be applied to predict residential property prices.

Future Improvements

Possible future improvements include:

Feature engineering
Hyperparameter tuning
Cross-validation
Log transformation of the target variable
Testing Random Forest and Gradient Boosting models
Comparing additional regression algorithms
Further analysis of outliers and skewed features