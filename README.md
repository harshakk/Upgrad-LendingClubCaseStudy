# UpGrad - Lending Club Case Study
> Lending Club, is consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:
1. If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
2. If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company

 The objective is to use Exploratory Data Analysis to understand how consumer attributes and loan attributes influence the tendency of default. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as
 1. Denying the loan
 2. Reducing the amount of loan
 3. Lending (to risky applicants) at a higher interest rate

Determine consumer attributes (features/factors) and loan attributes from the historical data that correlate to:
1. Higher chances of loan being fully paid
2. Higher chances of loan being paid, but with some missed/delayed payments
3. Higher chances of load being defaulted upon / Charged-off



## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
Steps followed 
1. Load required libraries
2. Load dataframe
    A. Review and set the index columns if needed
3. Data Review and Cleanup
    A. Remove unwanted columns / features with nulls - Columns having high percentage of missing values (>40 or 50%): directly discard those columns from the analysis - insights based on these are not reliable
    B. Remove rows with invalid values
4. Data Cleanup and Feature Selection Strategies
    A. Narrow down features that may have impact on exploratory data analysis
    B. Standardize feature values
    C. Columns having missing values under acceptable range can be imputed (replace with some values)
    D. For numerical features prefer to use mean or median, for categorical columns prefer to use mode
    E. If we have very less missing values (<1%) in a column, in that case we can drop rows as well
5. Check the need for derived metrics
    A. Type Driven Metrics - Steven's Typology - Nominal, Ordinal, Interval and Ratio
    B. Business Driven Metrics
    C. Data Driven Metrics
6. Univariate and Segmented Univariate Analysis
    A. Identify Ordered and Unordered Categorical Variables
    B. Identify Quantitative Variables
    C. Plot the values using MatplotLib and identify outliers
    D. Perform Univariate, Segmented Univariate Analysis on the selected features
    E. Perform (Categorical) Bivariate Analysis on the selected features
    F. Identify Positive and Negative Correlations between features

## Conclusions
1. Borrowers are more likely to default when they take loans for a 60-month term.
2. Borrowers with a 'Verified' loan status tend to take higher loan amounts with a 60-month tenure, increasing the risk of default.
3. Borrowers who rent their homes and take loans for debt consolidation purposes have a higher probability of default.
4. Borrowers with an annual income in the range of 0 to 20000 are more prone to defaulting.
5. Borrowers who take loan amounts in the range of 0 to 14000 have a higher default rate.
6. Borrowers receiving interest rates between 15-20% are at a higher risk of default.
7. Borrowers taking loans for small businesses are more likely to default.
8. Borrowers with lower grade (e.g., F < G) are at an increased risk of default.
9. Borrowers with subgrades F5, G3, or G5 are more likely to default


## Technologies Used
- Python
- Matplotlib
- Numpy
- Pandas
- Seaborn


## Acknowledgements
Give credit here.
- This project was delivered as part of a Study Group exercise within UpGrad

## Contact
Created by [@githubusername] - feel free to contact me!

