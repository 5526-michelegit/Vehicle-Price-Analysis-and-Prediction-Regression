# Predicting Used Car Prices with Multiple Linear Regression

This R project aims to develop a multiple linear regression model to predict the selling price of used cars based on various features. We utilize a comprehensive dataset that includes details such as car make, model, fuel type, transmission type, owner type, and more, aiming to identify the most significant predictors of a car's selling price.

## Overview

### Dataset
The dataset contains information about used cars listed for sale, including attributes like fuel type, transmission, owner type, mileage, engine size, and power. Some variables, like mileage and torque, were removed from the analysis due to comparability issues or inconsistent measurement units.

### Objectives
- To preprocess and clean the dataset, ensuring accurate types for each variable and removing unnecessary columns.
- To convert unit measurements and deal with missing values appropriately.
- To explore the dataset, identifying significant predictors and examining the distribution of variables.
- To develop a multiple linear regression model that accurately predicts the selling price of a used car.
- To validate the model's performance using statistical metrics and test it on unseen data.

## Methodology

1. **Data Preprocessing**: We adjusted data types, handled missing values, removed irrelevant columns, and converted units of measurement to ensure consistency and accuracy in our analysis.
   
2. **Exploratory Data Analysis (EDA)**: We conducted a detailed EDA to understand the distribution of the target variable (selling price) and the predictors. This included examining outliers, analyzing the distribution of numerical and categorical variables, and checking for multicollinearity.

3. **Feature Engineering**: We transformed some variables to better fit the linear regression assumptions, created dummy variables for categorical predictors, and performed feature selection to reduce model complexity without sacrificing predictive power.

4. **Model Building**: We developed multiple linear regression models, starting with a full model including all predictors and then refined it using backward elimination based on the AIC criterion and checking for multicollinearity.

5. **Model Evaluation**: We evaluated the model's performance using R-squared, Adjusted R-squared, and RMSE metrics on both training and test sets. We also performed diagnostic checks to validate the assumptions of linear regression.

6. **Predictive Analysis**: Finally, we applied our optimized model to a test set to evaluate its predictive accuracy and examined the residuals to ensure that no significant violations of our model assumptions were present.

## Tools and Libraries Used
- R programming language
- Tidyverse packages (`dplyr`, `ggplot2`, `readr`, etc.) for data manipulation and visualization
- `caret` for model building and evaluation
- `mice` for handling missing data
- `glmnet` and `xgboost` for advanced regression techniques
- Various other CRAN packages for statistical analysis and data preprocessing

## Key Findings
- The selling price of used cars is significantly influenced by the car's age, power, and certain brands.
- The model demonstrates a good fit with an Adjusted R-squared value of 0.8577, indicating that it can explain a significant portion of the variance in the selling prices.
- Diagnostic checks confirmed that the final model met the key assumptions of linear regression, ensuring the reliability of the predictions.

## Conclusion
Through careful data preparation, rigorous EDA, and methodical model building and evaluation, we developed a robust linear regression model that can predict the selling prices of used cars with a high degree of accuracy. This model can be a valuable tool for sellers to price their cars competitively and for buyers to ensure they are getting fair value for their purchases.

For more details on our methodology, findings, and code, please refer to the full project documentation included in this repository.
