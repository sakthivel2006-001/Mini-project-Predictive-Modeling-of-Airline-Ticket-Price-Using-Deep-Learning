# Mini-project-Predictive-Modeling-of-Airline-Ticket-Price-Using-Deep-Learning
Predictive Modeling of Airline Ticket Price Using DL
### Name : SAKTHIVEL S

## Predictive Modeling of Airline Ticket Prices Using Deep Learning
### Table of Contents

Project Overview
Objectives
Dataset
Features
Methodology
Model Architecture
Installation
Usage
Results
Future Scope
References

## Project Overview

Airline ticket prices fluctuate dynamically due to factors such as demand, seasonality, route, airline, and market competition. This project leverages deep learning techniques to predict airline ticket prices based on historical data and relevant features. By accurately forecasting ticket prices, travelers and agencies can make informed purchase decisions, and airlines can optimize revenue management strategies.

## Objectives
1.Collect and preprocess historical airline fare data.
2.Identify key factors affecting ticket prices.
3.Develop a deep learning model (LSTM, MLP, or CNN) for price prediction.
4.Compare deep learning model performance with baseline machine learning models.
5.Provide an interactive interface or dashboard for visualizing predictions.
6.Evaluate the system using metrics such as MAE, RMSE, and MAPE.

## Dataset
The dataset contains historical airline fare information including:

## Feature	Description
query_time	Timestamp of the price observation
origin	Departure airport code
destination	Arrival airport code
departure_date	Flight departure date
return_date	Flight return date (if applicable)
carrier	Airline operating the flight
cabin	Cabin class (Economy, Business)
stops	Number of stops
price	Ticket fare (target variable)
days_to_departure	Days between query and departure
holiday_flag	Indicator for local holidays/events

## Features

Categorical Features: Airline, origin, destination, cabin class

Numerical Features: Days to departure, price history, rolling statistics

Time Features: Day of week, month, seasonality

External Features (Optional): Holiday/event flags, competitor prices, fuel price index

## Methodology

Data Preprocessing: Handle missing values, encode categorical variables, normalize numerical features.

Feature Engineering: Generate lag features, route embeddings, time features, and rolling statistics.

Model Training: Train deep learning models (LSTM, MLP, CNN) to capture temporal and nonlinear patterns.

Evaluation: Use metrics like MAE, RMSE, and MAPE to compare with baseline regression models.

Deployment (Optional): Create a dashboard or API to predict ticket prices in real time.

## Model Architecture

Embeddings: For categorical variables (carrier, origin, destination).

LSTM Layer: To capture temporal dependencies in historical price data.

Dense Layers: For numerical and embedded features.

Output: Predicts ticket price (single-step or multi-horizon).

Loss Function: Huber Loss (robust to outliers)
Metrics: MAE, RMSE
