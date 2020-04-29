# Analysis-of-Crop-production-in-a-country
A Data science project aims to perform various types of analysis to understand the factors that affect the productivity of crop in a given land. It first conducts Exploratory Data Analysis (EDA) and data visualization to understand the behaviour of each feature and how they are affecting other features as well as the target variable and then performs Predictive analysis to predict which land areas are likely to produce more crop. 

## Dataset
The dataset contains information about yield from 1000 farms across a country.

Independent variable:
- Id : Identifier
- Water : the average amount of water received by hectare
- UV : the average amount of light received by hectare
- Area : the size of the farm in hectares
- Fertilizer_usage : the level of fertilization
- Pesticides : the amount of pesticides used per hectare
- Region : region code
- Catergories : comma-separated list of pesticides used

Dependent variable/ Target variable:
- Yield : total crop yield by farm

## Exploratory Data Analysis
 - Data Summaries - Attribute type, Class distribution, Mean, Median, SD, Quartile, Skewness, Kurtosis.
 - Univariate analysis.
 - Bivariate analysis and Hypothesis testing (Using Bivariate).
 
 ## Data VIsualization
 - Histogram
 - Count plot
 - QQ plot
 - Box plot
 - Scatter plot
 - Correlation matrix

## Feature Engineering
- Missing value treatment
- Outlier treatment
- Deriving new features (creating dummy variables)

## Model Building
Compare the performance for the following models:

- Linear Regression
- Random Forest
- XG Boost

## Conclusion
- Leverage the important features from XGBoost model -- Fertilizer usage 0, 1 in combination with region 6 and region 4 and having more area (Ofcourse constrained by cost of land) to improve the yield of the farm.
- Since we have a predictive model now, we have visibility into the future state of farm and we know what actions can lead to better yield, the farm management should apply cohesive actions using the model insights to improve the yield.
- We can create A/B tests by assigning more area, more relevant pesticides in the important regions as control and not have nothing in the test areas to find the incremental yield.
- Since Area is a natural limitation - obviously there is a cost constraint in terms of increasing more land for irrigation.
- Mean Absolute Error of 6.41 for XGBoost suggests that in comparison to an average yield of 58.78, our model is predicting 58.71 +/- 6.41 yield, which is pretty accurate considering so many factors involved in the model.
