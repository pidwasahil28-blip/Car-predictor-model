
# Car Price Prediction Model 🚗

## Overview
This repository contains a Machine Learning project that predicts the selling price of used cars. Built using Python and Scikit-Learn, the model utilizes a Linear Regression algorithm integrated within a robust data preprocessing pipeline. This project demonstrates core data science workflows including data cleaning, feature engineering, and building machine learning pipelines.

## Dataset
The model is trained on the `quikr_car.csv` dataset, which contains raw data for used cars with the following features:
* **name:** The specific model name of the car.
* **company:** The manufacturing brand.
* **year:** The year of purchase.
* **Price:** The selling price of the car (Target Variable).
* **kms_driven:** The total kilometers the car has been driven.
* **fuel_type:** The type of fuel used (e.g., Petrol, Diesel, LPG).

## Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Scikit-Learn
* **Environment:** Jupyter Notebook

## Project Workflow
1. **Data Cleaning:** Handled missing values, filtered out invalid entries, removed non-numeric characters from numeric columns (`Price`, `kms_driven`), and properly formatted data types.
2. **Data Preprocessing:** Implemented a Scikit-Learn `ColumnTransformer` to apply `OneHotEncoder` to categorical features (`name`, `company`, `fuel_type`).
3. **Model Pipeline:** Constructed a machine learning `Pipeline` connecting the data preprocessor directly to a `LinearRegression` model. This ensures clean, sequential data transformations and simplifies making predictions on new data.
4. **Evaluation:** Evaluated model performance using the R-squared (R²) regression metric.

## How to Run the Project
1. Clone this repository to your local machine:
   ```bash
   git clone <this repository>
2.pip install pandas numpy scikit-learn matplotlib jupyter in bash 
3.jupyter notebook
