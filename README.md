# Solar Energy Prediction Project

## Overview

This project focuses on predicting solar energy output using historical data. The dataset contains solar energy production records from 2010 to 2024, aggregated daily. The goal of this project is to preprocess the data, create a machine learning model, and make predictions about future solar energy output.

## Project Structure

The project is structured as follows:

- **Data Preprocessing**: 
  - The dataset contains columns such as `Date`, `From`, `To`, and `Energy(MW)`. The preprocessing steps include:
    - Splitting the data into individual components: Date, Energy, and Time intervals.
    - Converting the `Energy(MW)` from string to integer.
    - Aggregating the energy data on a daily basis.
  
- **Data Sources**:
  - Multiple datasets from 2010 to 2024 are loaded and preprocessed. These datasets are combined into a single dataset for training the model.

- **Machine Learning Model**:
  - The Keras library is used to build a neural network model for predicting solar energy output based on historical trends.

## Key Steps

1. **Loading the Data**: The data is loaded from CSV files for each year from 2010 to 2024.
2. **Preprocessing the Data**: 
   - The preprocessing function handles splitting the date, converting energy values, and grouping the data by day.
   - The preprocessed data is then concatenated across all the years.
3. **Modeling**: A machine learning model is built using Keras to predict the solar energy output for future dates.

## Requirements

- Python 3.x
- Keras
- Numpy
- Pandas

