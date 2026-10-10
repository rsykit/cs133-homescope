# HomeScope: A Data-Driven House Price Prediction Tool

## Authors

- **Author 1:** Kristy Chan
- **Author 2:** Bhoomika Gupta

## Project Description
HomeScope is an interactive house price analysis and prediction project based on property sales in King County, Washington, from May 2014 to May 2015. We will combine property characteristics with Census neighborhood information, Washington housing market data, and nearby high school graduation rates. The project will explore which property and neighborhood features are associated with higher sale prices. We will compare statistical and machine learning models to predict home prices and evaluate how accurately they perform across different neighborhoods. The final interface will help users explore housing patterns, estimate a potential sale price, and understand the limitations and fairness concerns of housing price prediction.

## Project Outline and Plan
Collect four public datasets: King County house sales, Census ZIP code data, the Washington housing price index, and high school graduation rates
Clean the data, document every cleaning decision, and join the datasets
Run descriptive statistics, correlation analysis, ANOVA, and Welch's t test
Train and compare linear regression, random forest, and gradient boosting models
Build an interactive web page with a price estimator, a map, and charts
Compare prediction errors across neighborhood income groups and report limitations

## Interface Plan
The interface will be an interactive web page called HouseScope. Users will be able to enter or adjust property information such as ZIP code, living area, bedrooms, bathrooms, building grade, and year built. The interface will display an estimated sale price, the nearest high school and its graduation rate, and how the same house would be priced in other ZIP codes. It will also include an interactive map showing property prices and nearby school graduation rate data. Additional charts will show which features matter most to the model, model performance, price differences across neighborhoods, and prediction errors across income groups.

## Data Collection and Storage Plan
We will collect and organize the project data from public sources. The main property sales data will come from the King County house sales dataset. Census based ZIP code information will provide population density and median household income. Washington housing market data will provide a monthly state housing price index, and King County public school data will provide high school graduation rates for the class of 2015 and school locations. The datasets will be cleaned and joined using ZIP codes, sale months, and geographic coordinates, then stored as CSV files in the data folder. Raw data files will remain separate from cleaned and merged data so that the analysis can be reproduced.

## Data Analysis and Visualization Plan

We will analyze the relationship between property features, neighborhood characteristics, school graduation rates, and sale prices. The analysis will include descriptive statistics, correlation analysis, a comparison of prices across ZIP codes and school graduation rate groups, and statistical tests such as ANOVA and Welch's t test.

We will train and compare linear regression, random forest, and gradient boosting models to predict the log of sale price. Model performance will be evaluated using R squared, mean absolute error, and root mean squared error on held-out test data.

Visualizations will include a price map, actual versus predicted prices, feature importance, price distributions by neighborhood, and prediction error by income group.

## Repository Structure

```text
cs133-house-prices/
├── data/
│   ├── raw/              # Original data
│   ├── clean/            # Cleaned data
│   └── merged/           # Final joined data
├── src/                  # Scripts
├── notebooks/            # Analysis notebooks
├── dashboard/            # Web app
├── figures/              # Charts
├── README.md             # Project plan
├── requirements.txt      # Python packages
├── LICENSE               # MIT License
└── .gitignore            # Ignored files
```

## Responsible Use and Limitations


The model estimates patterns in historical sale data and should not be treated as a professional appraisal. The nearest high school is used as a proxy for school context and may not be the school assigned to a property. Neighborhood income and school graduation rates can also reflect historical inequality, so model predictions may reproduce existing housing disparities. The project will report these limitations and compare prediction errors across neighborhood income groups.
