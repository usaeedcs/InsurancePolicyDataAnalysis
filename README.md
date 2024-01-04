# Insurance Policy Indicator using Python

This project is a comprehensive data analysis and predictive modeling notebook. The main purpose of this project is to understand the relationships within the data and to build a predictive model for the insurance policy data. The project uses several datasets, including `TheGeneral.csv`, `MasterQuote.csv`, and `df_AP02.csv`.

## Project Purpose and Findings

The primary goal of this project is to conduct exploratory data analysis on the provided datasets, clean and preprocess the data, and finally, build predictive models. The target variable for our models is `MQuotedTotalPayment`, a numerical value associated with the cost or payment amount provided during the insurance quote process. The specific unit or currency for this value is not clear from the provided data.

During the exploratory data analysis, we used various statistical and visualization techniques to understand the data. We used pair plots, histograms, and heatmaps to visualize the relationships between variables and to identify potential outliers. We also used descriptive statistics to understand the central tendency, dispersion, and distribution shape of the dataset.

We found that some variables have missing values that needed to be handled. We used a greedy approach for imputation, where we found all columns having numeric data type and imputed them by mean, and similarly, we found all categorical data and imputed it by the most common one.

We also found that some variables are highly skewed and some variables have a strong correlation with each other. We used feature scaling to standardize the range of independent variables or features of data. We also used feature selection techniques like correlation matrix and SelectKBest to select the most important features for our models.

The predictive modeling part of the project includes Multiple Linear Regression, Ridge Regression, Lasso Regression, Decision Tree Regressor, Random Forest Regressor, and Logistic Regression. We used cross-validation to estimate the performance of these models and to avoid overfitting. We also used GridSearchCV for hyperparameter tuning to improve the performance of our models.

After comparing these models, we found that the Random Forest Regressor model performed slightly better with an accuracy score of 0.85, indicating that 85% of the variance in the `MQuotedTotalPayment` can be predicted from the input features.

The results of the analysis provided valuable insights into the factors that influence the quoted total payment for an insurance policy. For instance, the driver's history, the type of coverage, and the number of drivers were among the most significant factors.

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
5. **Model Building**: Several models are built and evaluated, including Multiple Linear Regression, Ridge Regression, Lasso Regression, Decision Tree Regressor, Random Forest Regressor, and Logistic Regression.

## How to Run

To run this project, follow these steps:

1. Clone the repository to your local machine.
2. Make sure you have all the necessary Python libraries installed. You can install them using pip:
