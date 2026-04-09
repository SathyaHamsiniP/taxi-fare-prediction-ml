# Taxi Fare Prediction using Machine Learning

This project implements a regression-based machine learning pipeline to predict taxi trip total fare amount (`total_amount`) using trip-level features such as distance, timestamps, passenger count, surcharge components, and location identifiers. The workflow includes data preprocessing, feature engineering, exploratory data analysis, model training, and performance evaluation.

## Problem Statement

The objective of this project is to estimate taxi trip fares based on trip characteristics. The task is formulated as a supervised regression problem in which multiple machine learning models are trained and compared to identify the most effective predictor.

## Dataset Description

The dataset contains 10,000 taxi trip records with 17 features describing trip details, payment information, surcharge components, and timestamps.

### Numerical Features

- passenger_count
- trip_distance
- extra
- tip_amount
- tolls_amount
- congestion_surcharge
- improvement_surcharge
- Airport_fee

### Categorical Features

- payment_type
- store_and_fwd_flag
- VendorID
- RatecodeID
- PULocationID
- DOLocationID

### Datetime Features

- pickup_datetime
- dropoff_datetime

## Data Preprocessing

The following preprocessing steps were performed:

- conversion of timestamp columns into datetime format
- inspection of negative trip durations
- identification of extreme trip distance values
- analysis of anomalous passenger counts
- verification of negative surcharge and monetary entries
- separation of categorical and numerical features

These steps ensured improved data consistency prior to model training.

## Feature Engineering

Additional temporal features were derived from timestamp variables:

- trip_duration
- pickup_hour
- pickup_day_of_week
- pickup_month

These features helped capture temporal travel patterns affecting fare estimation.

## Exploratory Data Analysis

Exploratory analysis included:

- descriptive statistics of numerical variables
- inspection of outliers in trip distance
- validation of anomalous passenger counts
- examination of surcharge distributions
- analysis of negative fare-related entries

Insights from exploratory analysis guided preprocessing and modeling decisions.

## Models Implemented

The following regression models were trained and evaluated:

- Linear Regression
- Ridge Regression
- Random Forest Regressor
- Gradient Boosting Regressor
- K-Nearest Neighbors Regressor

## Evaluation Metrics

Model performance was evaluated using:

- Root Mean Squared Error (RMSE)
- R-squared (R² Score)

These metrics were used to compare predictive performance across models.

## Technology Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## Key Outcomes

This project demonstrates:

- construction of an end-to-end regression pipeline
- feature engineering from temporal variables
- handling of real-world transportation dataset inconsistencies
- comparison of multiple regression algorithms
- evaluation using appropriate regression performance metrics

## Project Walkthrough

A walkthrough video explaining preprocessing steps, feature engineering decisions, and model evaluation can be added here:

[Project Walkthrough Video](https://drive.google.com/file/d/1iLqfur7UNXqYHQCmsysQfKWxsYdH-aJm/view?usp=sharing)
