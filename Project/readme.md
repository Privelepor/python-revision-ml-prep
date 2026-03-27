# Bike Sharing Linear Regression Project

This repository contains a **mini machine learning project** demonstrating **linear regression** on the London bike-sharing dataset. The project attempts to predict both the **season** and the **number of bikes rented (`cnt`)** based on historical data.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Feature](#features)

## Project Overview
The goal of this project is to build and evaluate a **linear regression model** to predict bike-sharing demand. The workflow includes:

- Data preprocessing and feature engineering
- Training a linear regression model on bike count (`cnt`) and season
- Evaluating model performance
- Visualizing feature relationships and model results

This project highlights practical issues such as **poor convergence** and limitations of linear regression on categorical/complex targets.

## Dataset
The dataset `london_merged.csv` contains daily bike-sharing counts and weather/seasonal features in London. It includes:

- `season`: Season (0: Winter, 1: Spring, 2: Summer, 3: Fall)
- `t1`: Temperature (normalized)
- `t2`: "Feels like" temperature
- `hum`: Humidity
- `windspeed`: Wind speed
- `cnt`: Count of total bike rentals
- `timestamp`: Date and time

Additional temporal features were derived for the model: `year`, `month`, `day`, `hour`, `minute`.

## Features
The features used for the regression model include:

- Weather: `t1`, `t2`, `hum`, `windspeed`
- Temporal: `year`, `month`, `day`, `hour`, `minute`
- Target variables:
  - `cnt` (continuous)
  - `season` (categorical/ordinal)
