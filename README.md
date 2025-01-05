# Price Prediction for Airbnb Listings in New York

## Project Overview

This project aims to predict Airbnb listing prices in New York City using various regression models. The goal is to predict the price of a listing based on features such as property type, neighborhood, and availability. The project includes exploratory data analysis (EDA), feature engineering, model training, and performance evaluation.

### Key Highlights:

- **Dataset**: Airbnb listings data for New York City, containing information about listing features, pricing, and location.
- **Objective**: Predict the price of Airbnb listings based on various factors.
- **Models Evaluated**: Linear Regression, K-Nearest Neighbors (KNN), Random Forest, and Gradient Boosting.

## Tools & Technologies Used

- **Programming Language**: Python
- **Libraries**:
  - **Pandas**: Data manipulation and preprocessing
  - **Matplotlib & Seaborn**: Visualization of data and model results
  - **Scikit-learn**: Machine learning algorithms and performance metrics
  - **XGBoost**: Gradient Boosting model implementation
  - **Jupyter Notebooks**: For EDA and model development
  - **Pipenv**: Dependency management (using `Pipfile` and `Pipfile.lock`)

## Dataset

Dataset from [OpenDataSoft](https://public.opendatasoft.com/explore/dataset/air-bnb-listings/information/?disjunctive.neighbourhood&disjunctive.column_10&disjunctive.city) which can be downloaded [here](https://data.insideairbnb.com/united-states/ny/new-york-city/2024-04-06/data/listings.csv.gz) contains Airbnb listing details for New York City, with information such as:

- **Listing Features**: Type of property, number of rooms, and amenities.
- **Location Information**: Neighborhood, latitude, longitude, and proximity to landmarks.
- **Price**: The target variable to be predicted (listing price).

## Steps

![Model Comparison](betterRegression/steps.png)

### Pre-processing Steps:

- Handling missing values
- Encoding categorical features
- Normalizing continuous variables

## Model Evaluation & Results

The following regression models were evaluated:

| **Model**               | **rMSE** | **R-squared** | **Evaluation**                                                                    |
| ----------------------- | -------- | ------------- | --------------------------------------------------------------------------------- |
| **Linear Regression**   | 61.074   | +0.078        | Higher rMSE, limited predictive accuracy.                                         |
| **K-Nearest Neighbors** | 37.358   | -0.043        | Lower rMSE than Linear Regression but poor model fit (negative R-squared).        |
| **Random Forest**       | 35.396   | +0.091        | Moderate performance, reasonable rMSE, positive R-squared.                        |
| **Gradient Boosting**   | 34.333   | +0.118        | Best performance with lowest rMSE and highest R-squared, indicating superior fit. |

### Key Insights:

- The Gradient Boosting model provides the best predictive accuracy, making it ideal for predicting Airbnb prices.
- The other models also provided valuable insights into feature relationships but were less accurate.

## Visualizations

### 1. Model Performance Comparison

![Model Comparison](outputs/steps.png)
This visualization compares the RMSE values of various models, highlighting the superior performance of Gradient Boosting.

### 2. Price Distribution

![Price Distribution](content/New_York_City_.png)
A distribution plot of Airbnb prices in New York City, showcasing the price variation across different listings.

### 3. Interactive Heat Map

![NYC Airbnb Heat Map](outputs/nyc_airbnb_costs.html)
An interactive map showing the geographical distribution of Airbnb listings across New York City.

# How to run this project

- create pipenv virtual environment and install dependencies

  ```bash
  pip install pipenv
  ```

- run jupyter notebook within pipenv
