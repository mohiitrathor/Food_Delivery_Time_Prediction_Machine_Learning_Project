Food Delivery Time Prediction
Overview

This project implements an end-to-end machine learning pipeline to:

Predict delivery time (Regression)

Classify orders as Fast or Delayed (Classification)

The objective is to analyze delivery performance using order, location, traffic, and weather-related features.

Dataset Features

The dataset includes:

Customer and restaurant locations

Distance

Weather and traffic conditions

Delivery person experience

Order priority and time

Vehicle type

Ratings

Order cost and tip

Delivery time (target variable)

Feature Engineering

Extracted latitude and longitude from location strings

Computed Haversine distance

Created a Rush_Hour binary feature

Applied one-hot encoding to categorical variables

Standardized numerical features

Models Used
Linear Regression

Target: Delivery_Time

Metrics:

RMSE: 30.94

MAE: 26.52

R²: -0.035

The model shows weak predictive performance, suggesting non-linear relationships in the data.

Logistic Regression

Target: Delivery_Status (Fast / Delayed)

Metrics:

Accuracy: 0.50

F1-score: 0.47

AUC: 0.48

Performance is close to random guessing, indicating the need for more advanced models.

Tech Stack

Python
Pandas
NumPy
Matplotlib
Scikit-learn
