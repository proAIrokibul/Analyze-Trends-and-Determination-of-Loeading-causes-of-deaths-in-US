# Analyze-Trends-and-Determination-of-Loeading-causes-of-deaths-in-US
## Project Overview
This project explores the leading causes of death in the United States using a dataset that includes various attributes such as cause names, states, death counts, and age-adjusted death rates. The goal is to analyze trends in mortality and predict the age-adjusted death rate based on the number of deaths for different causes.

## Exploratory Data Analysis (EDA)
The EDA involved:
- Visualizing the total deaths by cause using bar plots.
- Analyzing the age-adjusted death rate distributions through box plots.
- Investigating trends over the years to understand how the leading causes of death have evolved.
- Creating heatmaps to visualize the relationship between states and causes of death.

## Machine Learning Models
Three machine learning models were applied to predict the age-adjusted death rate:

1. **Linear Regression**:
   - **Mean Squared Error (MSE)**: 51,259.11
   - **R² Score**: 0.0568
   - This model provided a baseline but showed limited predictive capability, indicating a weak linear relationship between the number of deaths and the age-adjusted death rate.

2. **Random Forest**:
   - **Mean Squared Error (MSE)**: 31,569.42
   - **R² Score**: 0.4191
   - The Random Forest model significantly improved prediction accuracy compared to linear regression, demonstrating its ability to capture non-linear relationships and interactions in the data.

3. **XGBoost**:
   - **Mean Squared Error (MSE)**: 24,323.11
   - **R² Score**: 0.5524
   - The XGBoost model yielded the best results among the three, with the lowest MSE and the highest R² score, indicating a robust predictive performance.

## Conclusion
The results suggest that while a simple linear model has limited predictive power, more advanced models like Random Forest and XGBoost can effectively predict age-adjusted death rates based on the number of deaths. This analysis can serve as a foundation for further investigations into mortality trends and potential factors influencing death rates in the United States.

