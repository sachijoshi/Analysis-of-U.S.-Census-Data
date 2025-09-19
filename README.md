# Analysis-of-U.S.-Census-Data

### This project analyzes the patterns of population relocation within states and across states in the United States, using demographic and mobility data. The goal is to examine how different variables, such as marital status, education level, and citizenship status, impact the mobility rate in different regions and states.

## Project Overview
### This analysis uses two datasets: one for control data (moved_same_state.csv) and one for variant data (moved_between_states.csv). The goal is to evaluate the factors influencing mobility rates, comparing states and regions across several dimensions like education, marital status, and citizenship.

## Data Description
### The datasets contain population statistics for different states and regions in the U.S., focusing on:
#### - Demographics: Marital status, education, and citizenship data.
#### - Mobility: Relocation within states and across states.
#### The variables used for analysis include:
#### - Total Population
#### - Never Married
#### - Married
#### - Total U.S. Citizens (Naturalized)
#### - Total Non-Citizens
#### - Relocated within State
#### - Relocated between States

# Analysis Steps
## Data Overview and Quality Assessment
### - Data Loading: The datasets are loaded from CSV files using Pandas.
### - Data Overview: Basic data information such as the number of rows and columns.
### - Descriptive Statistics
### - Descriptive statistics are calculated to give an overview of the distribution of key demographic variables and the relocation data for both control and variant datasets.
### - Missing Values: Missing values are checked and summarized.
### - Descriptive Statistics: Basic statistical information (e.g., mean, median, standard deviation) is provided for key columns.

# Visualizations
## Various visualizations are generated to better understand the data:
### 1. Distribution of relocation within and between states.
### 2. Correlation between relocation within and between states.
### 3. Top 10 states by total relocation.

# Statistical Testing
## T-tests are performed to assess the statistical significance of various comparisons:
### 1. California vs New York: within-state vs between-state mobility.
### 2. Comparison between U.S. citizens and non-citizens regarding mobility.
### 3. Educational mobility rates in different regions.

# Predictive Modeling
## A simple linear regression model is used to predict mobility rates based on demographic factors like marital status and citizenship.
### - Model Features: Marital status (Never Married, Married), Total U.S. Citizens (Naturalized).
### - Target Variable: Mobility ratio (relocation between states / relocation within state).

# Key Findings
## 1. Statistical Significance Tests:
### - CA vs NY within-state vs between-state mobility: p = 0.202 (not significant)
### - CA vs NY naturalized vs non-citizen mobility: p = 0.377 (not significant)
### - Northeast vs South education mobility: p = 0.896 (not significant)
### - Mountain vs South Atlantic marital status: p = 0.700 (not significant)
## 2. Key Observations:
### - Most comparisons show no statistically significant differences.
### - Small sample sizes (n=2 in many tests) limit statistical power.
### - Large p-values suggest true differences may not exist.
## 3. Data Quality Notes:
### - Analyses are based on aggregated state/regional data.
### - Assumptions of normal distribution for t-tests.
### - Small sample sizes may limit generalizability of the results.
