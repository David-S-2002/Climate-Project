# Climate-Project

## Data Analysis
My goal was to extract a trend from the data and to answer an additional analysis question. The trend I wanted to extract was the warming trend in the South Pacific ocean basin. The additional analysis questions were the following: In the North Pacific and South Pacific ocean basins, what is the relationship between sea surface temperature and wave height? What is the relationship between sea surface temperature and wind? Which feature is more important for predicting the sea surface temperature? 

Warming Trend:
1. I calculated and plotted a ten-year moving average of the sea surface temperature (SST) in the South Pacific over the entire time period.
2. To forecast the warming trend ten years into the future, I ran lagged autoregression on that moving average. The lag was ten years. The observed SST moving average was from 01/01/1940 to 02/29/2024, and the predicted SST moving average was from 03/03/2021 and 02/28/2034.

Additional Analysis Questions:
1. For each of the two ocean basins, I ran a linear regression model with wind_speed and wave_height as the predictors and SST as the target. For each ocean basin, I found the coefficients of the linear regression problem to determine the change in SST due to a change in one of the predictors.
2. I ran a random forest regressor on each dataset and looked at the feature importances. 
