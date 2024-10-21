California House Price Prediction

This project predicts housing prices in California using the California Housing Dataset. The dataset includes various features like location, number of rooms, population, and proximity to the ocean. The project utilizes different machine learning models, including RandomForestRegressor, with hyperparameter tuning using GridSearchCV to optimize performance.

Project Overview

The primary goal of this project is to build a regression model that predicts house prices in California based on features such as the number of rooms, population, and proximity to the ocean.

Tech Stack

Python: Data processing, analysis, and model development.
Pandas: For data manipulation and cleaning.
NumPy: For numerical computations.
Matplotlib & Seaborn: Used for data visualization and analysis of correlations.
Scikit-learn:
Used for building and evaluating machine learning models.
RandomForestRegressor: Primary model for prediction.
GridSearchCV: Used for hyperparameter tuning.
Jupyter Notebook: Interactive environment for developing and testing the model.
Dataset

The dataset contains 20,640 instances with the following features:

longitude: The longitudinal coordinate of the location.
latitude: The latitudinal coordinate of the location.
housing_median_age: The median age of the houses.
total_rooms: Total number of rooms in the district.
total_bedrooms: Total number of bedrooms in the district.
population: Population of the district.
households: Total number of households in the district.
median_income: Median income of the district.
ocean_proximity: Proximity of the location to the ocean (categorical).
The target variable is:

median_house_value: The median house value of the district.
Features Engineering

Log Transformation: Applied log transformation on skewed features like total_rooms, total_bedrooms, population, and households to reduce skewness.
Categorical Encoding: Converted the ocean_proximity categorical feature into one-hot encoded variables using pd.get_dummies().
New Features:
bedroom_ratio: The ratio of bedrooms to total rooms.
households_rooms: The ratio of total rooms to households.
Model Training

The following steps were taken to train the machine learning models:

Data Splitting: The dataset was split into training and testing sets using train_test_split.
Feature Scaling: The features were standardized using StandardScaler.
Model Selection: The primary model used was RandomForestRegressor.
Hyperparameter Tuning: Grid search was performed using GridSearchCV to find the best hyperparameters for n_estimators, max_features, and max_depth.
Model Evaluation: The performance of the model was evaluated using Mean Squared Error (MSE) and R-squared metrics.
Results

The optimized RandomForestRegressor model achieved the following performance:
Test Set R-squared: -0.1002
Test Set MSE: (calculated based on your evaluation)
