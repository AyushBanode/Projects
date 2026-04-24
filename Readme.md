#Project 2
This project aims to analyze the Zomato restaurant dataset to understand various characteristics of restaurants, including their ratings, costs, and other attributes. The goal is to preprocess and clean the raw data, perform exploratory data analysis to uncover key insights, and prepare the dataset for potential future modeling or deeper investigation into restaurant performance and customer preferences.


  * Data Acquisition: Loaded the Zomato dataset, ensuring robust parsing by handling bad lines and using the Python engine.
  * Data Cleaning & Preprocessing:
  * Removed irrelevant columns (e.g., url, address, phone, menu_item, listed_in(type), listed_in(city)).
  * Cleaned and standardized the 'rate' column by dropping missing values, converting non-numeric entries ('NEW', '-') to 0, and casting to float.
  * Processed 'approx_cost(for two people)' by removing commas and converting it to a float data type.

Exploratory Data Analysis (EDA):
  * Calculated and displayed average ratings for restaurants, identifying top-rated establishments.
  * Visualized the distribution of restaurant ratings to understand their spread.
  * Performed a normality test on the 'rate' distribution.
  * Defined a helper function to detect outliers using the Interquartile Range (IQR) method.
