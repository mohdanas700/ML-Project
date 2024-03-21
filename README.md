# Crop Yield Prediction

This project aims to predict crop yields based on various features such as year, average rainfall, pesticide usage, and average temperature.

## Screenshot
![Screenshot 2024-03-21 163732](https://github.com/mohdanas700/Crop-Yield-Prediction/assets/144828891/0e8242eb-21db-400c-9330-23bd829673ce)


## Dataset

The dataset used for this project contains information about crop yields across different countries. It includes the following columns:

- `Area`: Country where the crop was grown
- `Item`: Type of crop
- `Year`: Year of crop production
- `hg/ha_yield`: Yield in hectograms per hectare
- `average_rain_fall_mm_per_year`: Average rainfall in millimeters per year
- `pesticides_tonnes`: Pesticide usage in tonnes
- `avg_temp`: Average temperature

The dataset initially had 28,242 entries and 7 columns. After preprocessing, duplicates were removed, and categorical columns were transformed into numerical format. The final dataset contains 25,932 entries and 7 columns.

## Data Preprocessing

Data preprocessing steps included:
- Handling missing values
- Dropping duplicates
- Converting categorical variables to numerical format using one-hot encoding
- Scaling numerical features

## Exploratory Data Analysis (EDA)

EDA was performed to gain insights into the data:
- Frequency of crops grown in different countries
- Yield per country
- Yield per crop type

## Model Training

Four models were trained and evaluated for predicting crop yields:
- Linear Regression
- Lasso Regression
- Ridge Regression
- Decision Tree Regression

Decision Tree Regression outperformed other models with a Mean Absolute Error (MAE) of 3957.96 and an R-squared score of 0.979.

## Prediction

A predictive system was developed to predict crop yields based on user-input features. The system uses the trained Decision Tree Regression model along with preprocessing steps to make predictions.

## Usage

To use the predictive system:
1. Ensure that Python and required libraries are installed.
2. Run the provided Python script.
3. Input the required features such as Year, Rainfall, Pesticide Usage, Temperature, Country, and Crop.
4. Get the predicted yield for the given input.

## Files

- `app.py`: Python script containing the Flask web application for predicting crop yields.
- `dtr.pkl`: Pickle file containing the trained Decision Tree Regression model.
- `preprocessor.pkl`: Pickle file containing the preprocessor for feature transformation.
- `yield_df.csv`: CSV file containing the dataset used for training and prediction.

## Dependencies

- Python 3.x
- Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, Flask

## Author
**Mohd Anas**
