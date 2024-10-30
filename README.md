# Project Title: Analysis of Trends and Determination of Leading Causes of Death in the United States

## Project Overview
This project focuses on identifying and analyzing the leading causes of death across the United States. Using a comprehensive dataset containing information on causes of death, state-level breakdowns, and annual death counts, the primary objectives are to uncover trends in mortality over time and to develop predictive models for the age-adjusted death rate based on total deaths for each cause. By leveraging various machine learning models, the analysis aims to enhance our understanding of mortality patterns and provide insights into public health risks associated with different causes of death.

## Exploratory Data Analysis (EDA)

1. **Total Deaths by Cause Visualization**:  
   To understand which causes of death contribute most significantly to overall mortality, bar plots were used to display the total number of deaths attributed to each cause. This approach highlighted the most prevalent causes of death, allowing for a comparative analysis between conditions like heart disease, cancer, and respiratory illnesses.

2. **Age-Adjusted Death Rate Distributions**:  
   Age-adjusted death rates were analyzed across various causes using box plots, offering a view into the distribution and variability of death rates across states and years. This approach allowed for insights into the most and least variable causes, shedding light on disparities in death rates between regions and among different causes.

3. **Trend Analysis Over Time**:  
   To explore how the leading causes of death have shifted over time, line plots and time series analysis were employed. This helped reveal patterns and potential shifts in mortality due to advances in healthcare, changes in lifestyle, or public health policies. For instance, a decrease in mortality from certain diseases over time may indicate successful interventions or improvements in treatment.

4. **State and Cause Relationship Heatmap**:  
   A heatmap was generated to visualize the relationship between states and the leading causes of death. This provided an understanding of geographic variations in mortality, with certain causes of death showing higher or lower frequencies depending on the state. This spatial analysis helped highlight regions with higher mortality risks for specific causes, potentially guiding resource allocation and targeted public health interventions.

## Machine Learning Models
To predict the age-adjusted death rate based on the number of deaths for different causes, three machine learning models were applied and evaluated:

1. **Linear Regression**:  
   - **Mean Squared Error (MSE)**: 51,259.11  
   - **R² Score**: 0.0568  
   Linear regression was chosen as the baseline model, given its simplicity and interpretability. However, the high MSE and low R² score indicated that the relationship between the number of deaths and the age-adjusted death rate was weakly linear at best. This result highlighted that age-adjusted death rates are influenced by factors beyond mere death counts, such as demographic variables or healthcare quality.

2. **Random Forest**:  
   - **Mean Squared Error (MSE)**: 31,569.42  
   - **R² Score**: 0.4191  
   The Random Forest model demonstrated substantial improvement over linear regression by capturing non-linear patterns within the data. This model’s ability to accommodate complex interactions between variables led to better predictive accuracy, as shown by the lower MSE and higher R² score. The Random Forest results suggest that cause-specific and state-level factors might influence the age-adjusted death rate in non-linear ways, which could be further explored.

3. **XGBoost**:  
   - **Mean Squared Error (MSE)**: 24,323.11  
   - **R² Score**: 0.5524  
   XGBoost provided the best performance among the models, achieving the lowest MSE and the highest R² score. Its gradient-boosting technique, which iteratively improves predictive accuracy by minimizing errors, proved highly effective in this context. This model’s success underscores the complexity of the underlying relationships, suggesting that certain causes of death and state-specific variables might have nuanced influences on the age-adjusted death rate that simpler models cannot capture.

## Conclusion
The analysis shows that advanced machine learning models, particularly XGBoost, can significantly improve the accuracy of age-adjusted death rate predictions when compared to simpler linear approaches. The findings suggest that mortality patterns in the United States are influenced by a complex interplay of factors beyond raw death counts, such as demographic trends, state-level health resources, and cause-specific mortality risks. This project not only offers insights into historical mortality trends but also lays the groundwork for predictive modeling that could support targeted interventions to address specific health risks and improve public health outcomes across different regions in the United States. Future work could expand on these insights by incorporating additional socioeconomic or demographic factors and testing other machine learning models to further refine the predictions.
