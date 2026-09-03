# Mexico Real Estate Analysis

## Overview

This project analyzes residential property listings in Mexico to understand factors associated with property prices.

The project covers data cleaning, preparation, integration, descriptive analysis, and visualization using Python.

## Research Question

> **Are property prices more strongly associated with property size or location?**

## Dataset

The original data consists of three real estate datasets containing information on:

- Property type
- State
- Latitude and longitude
- Property area
- Property price

After cleaning and integration, the final dataset contains:

| Metric            |  Result |
| ----------------- | ------: |
| Property listings |   1,736 |
| Variables         |       6 |
| Missing values    |       0 |
| Median price      | $99,262 |

## Data Preparation

The raw datasets were cleaned and standardized before analysis.

Key steps included:

- Applied tidy data principles
- Cleaned and standardized property prices
- Converted MXN prices to USD
- Split latitude and longitude into separate variables
- Extracted state information
- Removed incomplete records where necessary
- Combined the three datasets using `pd.concat()`
- Validated the final dataset

## Exploratory Analysis

The cleaned dataset was analyzed using:

- Descriptive statistics
- Histograms
- Boxplots
- Scatterplots
- Regression trendlines
- State-level comparisons
- Property-type comparisons

## Key Findings

- Property prices are right-skewed.
- Property sizes are also right-skewed.
- Larger properties generally have higher prices.
- Property prices vary considerably across states.
- Property type is associated with differences in price distributions.
- The relationship between property size and price varies across locations.

## Conclusion

The analysis indicates that both **property size and location are associated with property prices**.

Property size shows a positive relationship with price, while differences across states suggest that location also plays an important role.

Further statistical analysis is required to determine which factor has the stronger relationship with property prices.

## Project Structure

```text
mexico-real-estate-analysis/
│
├── data/
│   ├── mexico-real-estate-1.csv
│   ├── mexico-real-estate-2.csv
│   ├── mexico-real-estate-3.csv
│   └── mexico-real-estate-combined-clean.csv
│
├── notebooks/
│   ├── 01_data_cleaning_preparation.ipynb
│   └── 02_visualizing_housing_data.ipynb
│
└── README.md
```
