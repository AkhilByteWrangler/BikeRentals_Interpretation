# BikeRentals_Interpretation

## Project Overview 🚴‍♂️

This project focuses on analyzing **bike rental patterns** using weather data, with a particular emphasis on interpreting how various features like **temperature**, **humidity**, and **windspeed** impact bike rentals.

We leverage **Random Forests** to build a predictive model and use advanced interpretation techniques to understand the relationships between features and predictions, including:

- **Partial Dependence Plots (PDP)**
- **Individual Conditional Expectation (ICE) Plots**
- **Accumulated Local Effects (ALE) Plots**

These techniques help explain how the model makes predictions and offer insights into how different weather conditions influence bike-sharing behaviors.

---

## Features Analyzed

- **Temperature**: How warmer or colder days affect bike rentals.
- **Humidity**: The impact of sticky, humid weather on biking trends.
- **Windspeed**: How windy days influence the decision to rent a bike.

---

## Techniques Used 🛠️

1. **Random Forest Regressor**: 
   - A machine learning model that helps predict daily bike rentals based on weather and seasonal features.

2. **PDP (Partial Dependence Plot)**:
   - Helps visualize the average effect of a single feature (like temperature) on bike rentals, holding all other features constant.

3. **ICE (Individual Conditional Expectation) Plot**:
   - Shows how individual predictions respond to changes in a feature, revealing variability across different data points.

4. **ALE (Accumulated Local Effects)**:
   - Similar to PDP, but more accurate when features are correlated. ALE shows how local changes in a feature impact predictions.

---
## Dataset 📊

We used the [Bike Sharing Dataset](https://archive.ics.uci.edu/ml/datasets/bike+sharing+dataset) from the UCI Machine Learning Repository. This dataset contains daily records of bike rentals, including:

- **Weather-related features** like temperature, humidity, and windspeed.
- **Time-related features** like the season, and whether it's a working day or not.
- **Bike rental count** (`cnt`): The total number of bike rentals on a particular day.

The dataset provides valuable insights into how environmental and temporal factors influence bike rental behavior.

### Dataset Features:
- **temp**: Normalized temperature in Celsius (ranging from 0 to 1).
- **atemp**: Normalized "feels-like" temperature.
- **hum**: Normalized humidity level.
- **windspeed**: Normalized windspeed.
- **season**: Categorical variable representing the season (1: Winter, 2: Spring, 3: Summer, 4: Fall).
- **workingday**: Whether the day is a working day (0: Holiday or weekend, 1: Working day).
- **count**: Total number of bikes rented on that day (this is our target variable).

You can download the dataset manually from the link above or let the Jupyter notebook fetch it for you automatically.

---

## Visualizations 📈

This project provides a series of visualizations to interpret the model's behavior:

- **Partial Dependence Plots (PDP)**: Visualize how changing one feature impacts bike rentals, keeping other features constant.
- **Individual Conditional Expectation (ICE) Plots**: Show how individual instances in the dataset react to changes in a feature.
- **Accumulated Local Effects (ALE) Plots**: A more robust version of PDP that accounts for feature correlations and shows how local changes in a feature impact predictions.

---

## How to Run 🏃‍♂️

To run this project, click on this button:

[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AIPI-590-XAI/Duke-AI-XAI/blob/dev/templates/template.ipynb)
   

