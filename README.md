# Turbofan_Life_Prediction

# Turbofan Engine Remaining Useful Life Prediction

This project involves predicting the Remaining Useful Life (RUL) of a turbofan engine using various machine learning techniques.

## Table of Contents
- [Introduction](#introduction)
- [Libraries and Initial Setup](#libraries-and-initial-setup)
- [Data Loading](#data-loading)
- [Data Inspection and Cleaning](#data-inspection-and-cleaning)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Feature Engineering and Data Preprocessing](#feature-engineering-and-data-preprocessing)
- [Model Training and Evaluation](#model-training-and-evaluation)

## Introduction

Predicting the Remaining Useful Life (RUL) of machinery is critical in industries such as aerospace, manufacturing, and automotive. This project utilizes data from the NASA Prognostics Data Repository to predict the RUL of a turbofan engine using machine learning techniques.

## Libraries and Initial Setup

**Imported Libraries:**
- pandas: for data manipulation and analysis.
- numpy: for numerical operations.
- matplotlib: for plotting and visualization.
- seaborn: for advanced data visualization.
- sklearn: for machine learning models and preprocessing.

**Initial Setup:**
- Setting the random seed for reproducibility.
- Filtering warnings for cleaner output.

## Data Loading

**Column Names for Datasets:**
- Defined the column names for the training and testing datasets.

**Loading Data from GitHub URLs:**
- Loading the training, testing, and RUL datasets from specified GitHub URLs using pandas.

## Data Inspection and Cleaning

**Shape of Datasets:**
- Checking the dimensions of the loaded datasets to ensure correct loading.

**Checking for NaN Values:**
- Verifying the presence of any NaN values in the datasets to ensure data quality.

## Exploratory Data Analysis (EDA)

**Statistical Description:**
- Using descriptive statistics to summarize the central tendency, dispersion, and shape of the dataset’s distribution.

**Data Visualization:**
- Visualizing data distributions and relationships using plots to understand the dataset better.

## Feature Engineering and Data Preprocessing

**Scaling Data:**
- Standardizing the data to ensure that each feature contributes equally to the model training process.

**Splitting Data:**
- Dividing the data into training and testing sets to facilitate model evaluation.

## Model Training and Evaluation

**Training RandomForestRegressor:**
- Training a RandomForestRegressor model on the training dataset.
- Evaluating the model using metrics such as Mean Squared Error (MSE) and R-squared to assess performance.
