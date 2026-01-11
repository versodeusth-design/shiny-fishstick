This project performs an Exploratory Data Analysis (EDA) on a real-world house prices dataset.
The goal is to understand the data structure, clean missing and inconsistent values, engineer useful features, and extract meaningful insights about house prices and locations.

This project is intended as a portfolio-ready EDA project and a learning reference for future data science and machine learning work.
Note:The CSV where i found the data is too heavy to upload here.
A) Objectives

Understand the structure and quality of the dataset

Handle missing values and optimize memory usage

Extract numerical features from text data

Analyze which factors influence house prices the most

Identify the most expensive locations

Visualize price distributions and location-based trends

B) Dataset

The dataset contains information about houses, including:

Price (in rupees)

C)Location

Area details (carpet area, super area, descriptions)

Property features (bathrooms, balconies, furnishing, etc.)

 Note: The dataset is messy and incomplete, reflecting real-world data.

️D)Tools & Libraries Used

Python

pandas – data manipulation

numpy – numerical operations

matplotlib – data visualization

re (regex) – text feature extraction

E) Key Steps Performed
1. Data Inspection

Checked data types, missing values, and memory usage

Identified columns with excessive missing data

2. Data Cleaning

Dropped columns with more than 40% missing values (except important ones)

Filled missing numerical values using the median

Filled missing categorical values using the mode

Removed rows with missing target values (Price (in rupees))

3. Feature Engineering

Extracted numeric square footage (area_sqft) from text descriptions using regex

Converted low-cardinality object columns to category to optimize memory

4. Exploratory Data Analysis (EDA)

Analyzed price distribution (identified right-skewness)

Used log transformation for better visualization

Grouped prices by location to find the top 10 most expensive areas

Calculated correlations between numerical features and house price

F) Key Insights

House prices are heavily right-skewed, which is common in real estate data

Location plays a major role in determining house prices

Extracted area features can provide additional explanatory power

Proper data cleaning significantly improves analysis reliability

G) Project Structure
house-prices-eda/
├── data/
│   └── house_prices.csv
├── notebooks/
│   └── house_prices_eda.ipynb
├── README.md
├── requirements.txt

H) How to Run This Project

Clone the repository

Install dependencies:

pip install -r requirements.txt


Open the notebook:

jupyter notebook


Run cells sequentially to reproduce the analysis

I) Next Steps

Apply feature scaling and outlier handling

Build predictive models (Linear Regression, Random Forest, etc.)

Combine with cloud workflows (AWS, S3, SageMaker)

Use as a foundation for advanced data science projects

 Author

Odonell Versailles
Aspiring Data Scientist | Python | Data Analysis | AWS
