# 🧹 Data Cleaning Project: Big Five Personality Dataset Overview
This project demonstrates a full professional data cleaning workflow using Python and Pandas.
The dataset contains more than 1 million responses to a personality questionnaire, including survey answers, country data, and technical metadata.

The cleaning process focused on ensuring data integrity, handling missing values, correcting data types, and preparing the dataset for analysis.

## 🧹 Cleaning Steps
1.Loaded tab-separated raw CSV data into Pandas.
2.Handled missing values:
    . Filled missing country entries with "Unknown".

3.Dropped incomplete survey responses:
    . Removed rows with missing answers in survey fields (EXT, EST, AGR, CSN, OPN).

4.Standardized data types:
    . Converted dateload to proper datetime format.
    .Converted latitude and longitude (lat_appx_lots_of_err,long_appx_lots_of_err) to numeric float values, coercing invalid entries to NaN.

5.Checked for and removed duplicate rows.

6.Verified final data quality:
    . Ensured 0 missing values in survey fields.
    .Ensured correct data types across all columns.

## Results

.Final dataset: 1,013,558 complete responses
.110 fully cleaned columns
.Clean and structured dataset ready for statistical analysis, machine learning, or dashboard creation.

## Technologies Used

.Python 3
.Pandas
.Jupyter Notebook

## Files Included
data cleaning.ipynb: Full cleaning script
data-final-cleaned.csv: Cleaned dataset ready for use
README.md: Project documentation

## Notes
    . 13,721 participants were missing latitude/longitude information. this is left as missing to preserve data integrity.
    . No missing survey responses remain after cleaning.

