**HomeScope: A Data Driven House Price Prediction Tool**

**Authors**
Author 1: Kristy Chan
Author 2: Bhoomika Gupta

**Project Description**

HomeScope is an interactive house price analysis and prediction project based on property sales in King County, Washington, from May 2014 to May 2015. We will combine property characteristics with Census neighborhood information, Washington housing market data, and nearby high school graduation rates. The project will explore which property and neighborhood features are associated with higher sale prices. We will compare statistical and machine learning models to predict home prices and evaluate how accurately they perform across different neighborhoods. The final interface will help users explore housing patterns, estimate a potential sale price, and understand the limitations and fairness concerns of housing price prediction.




**Data Analysis and Visualization Plan**

We will analyze the relationship between property features, neighborhood characteristics, school graduation rates, and sale prices. The analysis will include descriptive statistics, correlation analysis, a comparison of prices across ZIP codes and school graduation rate groups, and statistical tests such as ANOVA and Welch’s t test. We will train and compare linear regression, random forest, and gradient boosting models to predict the log of sale price. Model performance will be evaluated using R squared, mean absolute error, and root mean squared error on held out test data. Visualizations will include a price map, actual versus predicted prices, feature importance, price distributions by neighborhood, and prediction error by income group.

**Repository Structure**

cs133-house-prices/
├── data/
│   ├── raw/              # original data
│   ├── clean/            # cleaned data
│   └── merged/           # final joined data
├── src/                  # scripts
├── notebooks/            # analysis notebooks
├── dashboard/            # web app
├── figures/              # charts
├── README.md             # project plan
├── requirements.txt      # Python packages
├── LICENSE               # MIT License
└── .gitignore            # ignored files

**Responsible Use and Limitations**

The model estimates patterns in historical sale data and should not be treated as a professional appraisal. The nearest high school is used as a proxy for school context and may not be the school assigned to a property. Neighborhood income and school graduation rates can also reflect historical inequality, so model predictions may reproduce existing housing disparities. The project will report these limitations and compare prediction errors across neighborhood income groups.
