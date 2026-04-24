# Project1
"I've been working on a data cleaning and preprocessing project using the Google Play Store dataset. My main goal was to prepare this raw data for future analysis or model building. To achieve this:

  * Started by loading the googleplaystore.csv file and conducting an initial inspection to understand its structure and contents.
  * Identified and removed duplicate entries to ensure data uniqueness.
  * Systematically checked for missing values across all columns and devised strategies to handle them.
  * Performed several crucial data transformations:
  * Converted the 'Size' column from string representations (e.g., '19M') into numerical values in kilobytes.
  * Cleaned the 'Installs' column by removing special characters like '+' and ',' and converted it to a numerical type.
  * Refined the 'Android Ver' column by removing the 'and up' suffix and filled in any missing entries with the most frequent version.
  * Managed the 'Rating' column by first dropping an obvious outlier (a rating of 19) and then filling the remaining missing ratings with the mean value.

Finally, I implemented a function to detect outliers in numerical columns like 'Size' using the IQR method, which is a good preparation for further data validation."


# Project 2

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


# Project 3

Zomato Restaurant Data Analysis in Bangalore

The primary goal of this project was to gain insights into the restaurant landscape of Bangalore using Zomato data. Specifically, I aimed to understand key characteristics such as restaurant ratings, popular chains, operational models (online ordering, table booking), types of cuisines and restaurants, cost structures, and geographical distribution. Identifying top-performing and underperforming restaurants, as well as customer preferences, was also a key objective to provide actionable insights.

Steps Taken:
* Data Loading and Initial Inspection: Loaded the Zomato dataset and performed an initial check of its structure and content using head(), columns, and shape
* Data Cleaning: Addressed missing values, particularly in the 'rate' column, and transformed the 'rate' and 'approx_cost(for two people)' columns into appropriate numeric data types by removing non-numeric characters and converting them.
* Rating Analysis: Calculated and visualized the average ratings of restaurants, identifying the top-rated establishments and analyzing the overall distribution of ratings.
* Restaurant Chain Analysis: Identified and visualized the top restaurant chains based on the number of outlets.
* Operational Analysis: Examined the proportion of restaurants that accept online orders and table bookings through pie charts.
* Restaurant Type Distribution: Explored the different types of restaurants and their prevalence in Bangalore.
* Voting and Rating Correlation: Analyzed restaurants based on the number of votes they received, identifying both highly-rated restaurants with many votes and those with many votes but low ratings.
* Location Analysis: Determined the locations with the highest concentration of restaurants.
* Cuisine Preferences: Identified and visualized the top 10 most popular cuisines.
* Cost Distribution Analysis: Examined the distribution of 'approx_cost(for two people)' to understand typical pricing.
* Custom Query Function: Developed a function to filter restaurants based on custom criteria including location, restaurant type, and maximum cost, demonstrating its use to find casual dining options in Whitefield under Rs. 1000 with a good rating.

Conclusions:
* Byg Brewski Brewing Company, Asia Kitchen By Mainland China, and Punjab Grill were among the best-rated restaurants.
* Cafe Coffee Day, Onesta, Empire Restaurant, Just Bake, and Kanti Sweets emerged as the top restaurant chains.
* Approximately 66.9% of restaurants accept online orders, while about 85.8% offer table bookings.
* 'Byg Brewski Brewing Company' and 'The Black Pearl' were highly rated based on the number of votes.
* Restaurants like 'Lazeez' and 'Tandoor Hut' had a high number of votes but low ratings, indicating potential areas for improvement.
* BTM and Koramangala 5th Block are the locations with the highest density of restaurants.
* North Indian and Chinese cuisines are the most popular among Bangalore residents.
* The majority of restaurants have an approximate cost for two people ranging from Rs. 500 to Rs. 1000.
