Airbnb Data Cleaning and Exploratory Analysis

Project Overview
This project involves cleaning, preprocessing, and analyzing a dataset of Airbnb listings in New York City. The goal is to prepare the raw data for further modeling and to perform preliminary exploratory data analysis (EDA) to derive key insights, such as average pricing, distribution of listing types, and high-demand neighborhoods.

The key data cleaning challenges addressed include converting currency strings to numeric formats, correcting illogical data entries, and handling missing values.

💾 Dataset
The primary dataset used is Airbnb_Data.csv, which contains over 100,000 listings with 26 features, including pricing, location coordinates, host information, review metrics, and more.


🛠️ Data Cleaning and Preprocessing Steps
The following critical steps were executed to ensure data quality:

Duplicate Removal: All duplicate records were identified and removed.

Currency Conversion: The price and service fee columns were cleaned by removing '$' and ',' characters, then converted to the float data type.

Column Renaming: Columns were renamed for clarity (e.g., price to price_$ and service fee to service_fee_$).

Date Formatting: The last review column was converted to a proper datetime object, handling various formats.

Data Correction: A spelling error in the neighbourhood group column (brookln was corrected to Brooklyn).

Outlier Handling: Listings with an illogical availability 365 greater than 365 were removed.

Missing Values: All rows containing any missing (NaN) values were dropped, resulting in a significantly smaller but complete dataset for specific analyses.

