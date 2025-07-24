
# Vehicle Price Analysis and Prediction with Multiple Linear Regression

## Description
This R project develops a multiple linear regression model to predict used car selling prices based on features such as make, model, fuel type, transmission, and owner type. :contentReference[oaicite:0]{index=0}

## Table of Contents
1. [Repository Structure](#repository-structure)  
2. [Requirements](#requirements)  
3. [Installation](#installation)  
4. [Usage](#usage)  
5. [Dataset](#dataset)  
6. [Objectives](#objectives)  
7. [Methodology](#methodology)  
8. [Tools & Libraries](#tools--libraries)  
9. [Key Findings](#key-findings)  
10. [Conclusion](#conclusion)  
 

## Repository Structure
├── analysis_and_prediction.R      # R script performing regression analysis and predictions  
├── analysis_and_prediction.Rmd    # R Markdown report with EDA, modeling steps, and results  
└── README.md                      # Project documentation (this file)  

All files are located in the root of the repository. ([GitHub][1])

## Requirements

* **R** (version 4.0 or higher)
* **RStudio** (optional, for interactive development)
* The following R packages:

  * `tidyverse` (`dplyr`, `ggplot2`, `readr`, etc.)
  * `caret` for model training and evaluation
  * `mice` for handling missing data
  * `glmnet` and `xgboost` for advanced regression techniques
  * Other CRAN packages as needed for statistical analysis and data preprocessing ([GitHub][1])

## Installation

1. **Clone** the repository:

   ```bash
   git clone https://github.com/5526-michelegit/Vehicle-Price-Analysis-and-Prediction-Regression.git
   cd Vehicle-Price-Analysis-and-Prediction-Regression
   ```
2. **Install** required R packages. In an R console or RStudio:

   ```r
   install.packages(c(
     "tidyverse", "caret", "mice", "glmnet", "xgboost", 
     "readr", "ggplot2", "dplyr"
   ))
   ```

## Usage

1. **Run the analysis script** in R to preprocess data, build the regression model, and generate predictions:

   ```r
   source("analysis_and_prediction.R")
   ```
2. **Render the detailed report** (includes code, EDA, model diagnostics, and visualizations):

   ```r
   rmarkdown::render("analysis_and_prediction.Rmd")
   ```
3. **Review outputs** in the generated HTML (or PDF) report for full methodology and results. ([GitHub][1])

## Dataset

The project uses a comprehensive used cars dataset containing attributes such as fuel type, transmission, owner type, mileage, engine size, and power. Variables with inconsistent units (e.g., torque) were excluded to ensure comparability. ([GitHub][1])

## Objectives

* Preprocess and clean the dataset: ensure correct data types, handle missing values, and remove irrelevant columns.
* Conduct exploratory data analysis (EDA) to understand variable distributions, outliers, and relationships.
* Engineer features (dummy variables, transformations) and select predictors to optimize model performance.
* Build and refine a multiple linear regression model using backward elimination (AIC) and multicollinearity checks.
* Evaluate model accuracy with metrics such as R², Adjusted R², and RMSE on training and test sets. ([GitHub][1])

## Methodology

1. **Data Preprocessing**: Adjust data types, impute missing values with `mice`, and normalize measurements.
2. **Exploratory Data Analysis (EDA)**: Visualize distributions, detect outliers, and assess correlations among predictors.
3. **Feature Engineering**: Convert categorical variables to dummy indicators; apply transformations to meet regression assumptions.
4. **Model Building**: Fit a full multiple linear regression model, then perform backward selection based on AIC and VIF diagnostics.
5. **Model Evaluation**: Compute R², Adjusted R², and RMSE on hold-out data; validate residual plots and assumptions. ([GitHub][1])

## Tools & Libraries

* **R** programming language
* **Tidyverse** for data manipulation and visualization
* **caret** for model training and cross-validation
* **mice** for multiple imputation of missing data
* **glmnet** and **xgboost** for regularized and boosted regression models
* **rmarkdown** for report generation ([GitHub][1])

## Key Findings

* Car age, engine power, and brand significantly influence selling price.
* The final model achieved an Adjusted R² of approximately 0.8577, explaining a large portion of price variability.
* Diagnostic checks confirmed that model assumptions (linearity, homoscedasticity, normality) were met. ([GitHub][1])

## Conclusion

By following a rigorous workflow—data cleaning, EDA, feature engineering, model selection, and validation—this project delivers a robust multiple linear regression model for used car price prediction. The approach can guide sellers in pricing decisions and help buyers assess market value. ([GitHub][1])
