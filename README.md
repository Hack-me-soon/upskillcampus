# Turbofan Engine Remaining Useful Life Prediction

This project involves predicting the Remaining Useful Life (RUL) of a turbofan engine using various machine learning techniques. The data used in this project is sourced from the NASA Prognostics Data Repository.

## Table of Contents
- [Introduction](#introduction)
- [Links](#Links)
- [Libraries and Initial Setup](#libraries-and-initial-setup)
- [Data Loading](#data-loading)
- [Data Inspection and Cleaning](#data-inspection-and-cleaning)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Feature Engineering and Data Preprocessing](#feature-engineering-and-data-preprocessing)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction

Predicting the Remaining Useful Life (RUL) of machinery is critical in industries such as aerospace, manufacturing, and automotive. Accurate RUL predictions can help in proactive maintenance scheduling, reducing downtime, and avoiding catastrophic failures. This project utilizes turbofan engine data to develop and evaluate a machine learning model for RUL prediction.

## Links

- **Project Code Link** https://github.com/Hack-me-soon/upskillcampus/blob/main/Turbofan_Life_Prediction.ipynb

## Libraries and Initial Setup

**Imported Libraries:**
- **pandas:** Used for data manipulation and analysis. It provides data structures like DataFrame, which is ideal for handling structured data.
- **numpy:** A fundamental package for numerical operations in Python. It supports large multi-dimensional arrays and matrices, along with a collection of mathematical functions to operate on these arrays.
- **matplotlib:** A plotting library used for creating static, animated, and interactive visualizations in Python.
- **seaborn:** A data visualization library based on matplotlib that provides a high-level interface for drawing attractive and informative statistical graphics.
- **sklearn (scikit-learn):** A machine learning library in Python that features various classification, regression, and clustering algorithms, including support vector machines, random forests, gradient boosting, k-means, and DBSCAN.

**Initial Setup:**
- Setting the random seed ensures that the results are reproducible. By fixing the random seed, we make sure that the random processes in our code (like data shuffling) produce the same results every time.
- Filtering warnings helps in maintaining a cleaner output, which is particularly useful when running notebooks to avoid cluttering with unnecessary warning messages.

## Data Loading

**Column Names for Datasets:**
- Defined the column names for the training and testing datasets to ensure proper labeling and easy access of data columns during analysis.

**Loading Data from GitHub URLs:**
- The datasets for training, testing, and RUL are loaded from specified GitHub URLs using the `pd.read_csv()` function from pandas. This function reads a comma-separated values (CSV) file into a DataFrame.

## Data Inspection and Cleaning

**Shape of Datasets:**
- Checking the dimensions of the datasets (`dftrain`, `dfvalid`, and `y_valid`) ensures that they have been loaded correctly and helps in understanding the structure of the data.

**Checking for NaN Values:**
- Verifying the presence of any NaN values in the datasets is crucial as NaNs can cause issues during model training. Ensuring data quality by checking and handling NaNs appropriately is an essential step.

## Exploratory Data Analysis (EDA)

**Statistical Description:**
- Using descriptive statistics to summarize the central tendency (mean, median), dispersion (standard deviation, variance), and shape of the dataset’s distribution (min, max, quartiles). This provides a quick overview of the data and highlights any anomalies or outliers.

**Data Visualization:**
- Visualizing data distributions and relationships using plots helps in understanding the data better. For instance, plotting the sensor readings over time can show trends, while scatter plots can reveal correlations between different features. Visualization tools used include:
  - **Histogram:** To visualize the distribution of a single variable.
  - **Boxplot:** To show the spread and skewness of the data.
  - **Heatmap:** To visualize the correlation matrix and identify strongly correlated features.

## Feature Engineering and Data Preprocessing

**Scaling Data:**
- Standardizing the data to ensure that each feature contributes equally to the model training process. This is achieved using the `StandardScaler` from sklearn, which scales the data to have a mean of 0 and a standard deviation of 1.

**Splitting Data:**
- Dividing the data into training and testing sets to facilitate model evaluation. This step ensures that we have separate datasets for training the model and for evaluating its performance on unseen data. Typically, a portion of the data is set aside as the testing set (e.g., 20-30%), and the rest is used for training.

## Model Training and Evaluation

**Training RandomForestRegressor:**
- A RandomForestRegressor is trained on the training dataset. Random Forest is an ensemble learning method that operates by constructing multiple decision trees during training and outputting the average prediction of the individual trees. It helps in improving the predictive accuracy and controlling overfitting.
- **Model Evaluation:**
  - **Mean Squared Error (MSE):** Measures the average of the squares of the errors, i.e., the average squared difference between the estimated values and actual value.
  - **R-squared (R²):** Indicates how well the independent variables explain the variability of the dependent variable. An R² of 1 indicates that the regression predictions perfectly fit the data.

## Conclusion

This project on predicting the Remaining Useful Life (RUL) of a turbofan engine has been an incredibly enriching experience. By delving into the intricacies of data science and machine learning, I have gained a deeper understanding of various concepts and techniques that are critical in real-world applications. Here are some key takeaways from the project:

1. **Understanding the Data:**
   - Working with the NASA Prognostics Data Repository provided a hands-on experience with real-world data. The process of loading, inspecting, and cleaning the data underscored the importance of thorough data preparation.

2. **Exploratory Data Analysis (EDA):**
   - Performing EDA allowed me to uncover valuable insights and patterns within the data. Visualizing the data distributions and relationships helped in understanding the underlying structure and informed the feature engineering process.

3. **Feature Engineering and Preprocessing:**
   - Scaling the data and engineering relevant features were crucial steps in preparing the data for modeling. This ensured that the model could learn effectively from the data.

4. **Model Training and Evaluation:**
   - Training a RandomForestRegressor and evaluating its performance using metrics such as Mean Squared Error (MSE) and R-squared (R²) provided a solid foundation in regression modeling. The ensemble method of Random Forest proved effective in handling the complexity of the data.

5. **Practical Application:**
   - The project highlighted the practical importance of RUL prediction in industries like aerospace and manufacturing. Accurate RUL predictions can lead to proactive maintenance scheduling, reducing downtime and preventing catastrophic failures.

6. **Learning and Growth:**
   - This project has been one of the greatest learning experiences of my journey with Upskill Campus. The structured approach to problem-solving and the emphasis on practical applications have significantly enhanced my data science and machine learning skills.

I am proud to have successfully completed this project and am grateful for the guidance and resources provided by Upskill Campus. The knowledge and skills gained through this project will undoubtedly be valuable in my future endeavors in the field of data science and machine learning.
