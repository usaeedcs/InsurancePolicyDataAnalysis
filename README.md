# Data Analysis and Feature Engineering

This project is a comprehensive data analysis and predictive modeling notebook. The main purpose of this project is to understand the relationships within the data and to build a predictive model for the `MQuotedTotalPayment` variable, which represents the quoted total payment for an insurance policy. The project uses several datasets, including `TheGeneral.csv`, `MasterQuote.csv`, and `df_AP02.csv`.

## Project Purpose and Findings

The primary goal of this project is to conduct exploratory data analysis on the provided datasets, clean and preprocess the data, and finally, build predictive models. The target variable for our models is `MQuotedTotalPayment`, a numerical value associated with the cost or payment amount provided during the insurance quote process. The specific unit or currency for this value is not clear from the provided data.

During the exploratory data analysis, we found that some variables have missing values that needed to be handled. We also found that some variables are highly skewed and some variables have a strong correlation with each other.

The predictive modeling part of the project includes Multiple Linear Regression, Ridge Regression, and Lasso Regression. After comparing these models, we found that the Lasso Regression model performed slightly better.

## Libraries Used

The project uses several Python libraries, including:

- `numpy` and `pandas` for data manipulation
- `matplotlib` and `seaborn` for data visualization
- `sklearn` for machine learning and data preprocessing
- `statsmodels` for statistical models

## Project Structure

The project is structured as follows:

1. **Data Loading**: The datasets are loaded using pandas' `read_csv` function.
2. **Exploratory Data Analysis**: The data is explored using various statistical and visualization techniques.
3. **Data Cleaning**: The data is cleaned by handling missing values and encoding categorical variables.
4. **Feature Selection**: Important features are selected using various techniques like correlation matrix and SelectKBest.
5. **Model Building**: Several models are built and evaluated, including Multiple Linear Regression, Ridge Regression, and Lasso Regression.

## How to Run

To run this project, follow these steps:

1. Clone the repository to your local machine.
2. Make sure you have all the necessary Python libraries installed. You can install them using pip:
