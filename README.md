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
