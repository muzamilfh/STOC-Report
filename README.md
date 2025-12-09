
# 1. Introduction

-   The aim of this intermediate report is to explore determinants of income in South Austria.

-   We focus on data management and descriptive statistics before conducting regression modelling.

-   The response variable is net employment income (`py010n`).

-   Explanatory variables include gender, citizenship, household size, and age.

-   For the intermediate report we restrict to data management and descriptive statistics.

## 

# 2. Data collection and description

-   Source: EU-SILC (European Union Statistics on Income and Living Conditions), Austria.

-   Type of data: survey data, representative sample of private households.

-   Data format: cross-sectional microdata with social, demographic, and income information.

-   Variables used:

    -   `py010n` — employment income (numeric)

    -   `age` — age in years (numeric)

    -   `hsize` — household size (categorical converted to numeric)

    -   `gender` — male / female (categorical)

    -   `citizenship` — grouped nationality categories (categorical)

    -   `region` — Austrian federal region

-   Missing value handling:

    -   Keep only positive values of income (`py010n > 0`)

    -   Convert `hsize` to numeric

    -   Remove observations with missing values

-   Subsetting:

    -   Only individuals living in **Styria** and **Carinthia** (South Austria, NUTS-1 region)
