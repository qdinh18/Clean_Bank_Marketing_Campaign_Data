# Bank Marketing Data Engineering Project

## Project Overview
This project focuses on engineering a dataset from a bank marketing campaign for further analysis and modeling. The primary tasks include cleaning, transforming, and splitting the data into logical components for ease of use in downstream processes such as data warehousing, ETL pipelines, or machine learning workflows.

## Dataset
The dataset used is **bank_marketing.csv**, which contains details about bank clients, marketing campaigns, and economic indicators. The project transforms this raw data into three distinct, well-structured datasets:
- **Client Data**: Information about the bank’s clients (e.g., age, job, education).
- **Campaign Data**: Data on interactions between the bank and clients during marketing campaigns.
- **Economic Data**: Economic variables such as the consumer price index and Euribor rate, relevant to the campaign period.

## Data Engineering Process

1. **Data Loading**:
   The dataset is loaded into memory using the `pandas` library for data manipulation.

2. **Data Splitting**:
   The original dataset is split into three smaller, domain-specific DataFrames:
   - **Client DataFrame**: Contains fields like `client_id`, `age`, `job`, `marital status`, and credit-related information.
   - **Campaign DataFrame**: Includes the number of contacts during campaigns, duration, previous outcomes, and more.
   - **Economic DataFrame**: Tracks economic indicators like `consumer_price_index` and `euribor_three_months`.

3. **Data Cleaning**:
   - Missing and unknown values are handled.
   - Categorical fields are transformed into numerical or boolean types for better integration into data pipelines or analytics workflows.
   - Dates are formatted correctly, and unnecessary columns are removed.

4. **Data Export**:
   The cleaned and transformed data is exported into three CSV files for further usage:
   - `client.csv`
   - `campaign.csv`
   - `economics.csv`


