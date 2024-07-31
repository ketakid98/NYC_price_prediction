# NYC_price_prediction

Project Overview

This project aims to predict real estate prices in New York City using various machine learning models. The dataset includes information on property sales in NYC, with features such as land and gross square footage, building class, and location details. The goal is to create a robust model that accurately predicts sale prices based on these features.

Dataset

The dataset used in this project is nyc-rolling-sales.csv, which contains records of real estate transactions in NYC. The dataset includes columns such as:

BOROUGH: Borough code
NEIGHBORHOOD: Neighborhood name
BUILDING CLASS CATEGORY: Category of the building
TAX CLASS AT PRESENT: Current tax class
BLOCK: Block number
LOT: Lot number
BUILDING CLASS AT PRESENT: Current building class
ZIP CODE: Zip code
RESIDENTIAL UNITS: Number of residential units
COMMERCIAL UNITS: Number of commercial units
TOTAL UNITS: Total units
LAND SQUARE FEET: Land square footage
GROSS SQUARE FEET: Gross square footage
YEAR BUILT: Year the building was built
SALE PRICE: Sale price
SALE DATE: Date of sale

Data Preprocessing

Data preprocessing steps include:

1.Dropping Irrelevant Columns: Removed columns that are not useful for prediction, such as Unnamed: 0, APARTMENT NUMBER, etc.

2.Handling Missing Values: Filled missing values for numeric features with the mean or using appropriate methods.

3.Encoding Categorical Variables: Converted categorical variables into category type and encoded them as numerical codes.

4.Normalization: Applied normalization to features like LAND SQUARE FEET and GROSS SQUARE FEET.

5.Feature Engineering: Extracted additional features from SALE DATE such as year, month, quarter, and day.


Models Used
The project explores various machine learning models, including:

1.Random Forest Regressor: Used for feature ranking and price prediction.
2.Neural Networks: Built using Keras and TensorFlow for capturing complex relationships in the data.
3.Quantile Regression: Implemented using Statsmodels to understand the effect of features at different quantiles of sale prices.
