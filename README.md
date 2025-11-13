**Algerian Forest Fire Prediction – Machine Learning Project**

This project presents a complete end-to-end machine learning workflow to analyze and predict forest fire occurrence using the **Algerian Forest Fires Dataset**. The project includes data cleaning, preprocessing, feature analysis, model training, and evaluation using multiple regression techniques.

**Project Overview**

The primary goal of this project is to predict the occurrence and behavior of forest fires based on meteorological and environmental variables.
We implemented and compared multiple regression models:

- Linear Regression
- Lasso Regression
- Ridge Regression
- ElasticNet Regression

Each model’s performance was measured using **R² Score and MSE**, followed by visual comparisons and insights

**Dataset Description**

**Dataset Used:** Algerian_forest_fires_cleaned_dataset.csv (244 records)

**Key Features**

- Temperature (°C)
- Relative Humidity (%)
- Wind Speed (km/h)
- Rain (mm/m²)
- FFMC, DMC, DC, ISI – Fire Weather Indices

**Target Variable:**

- 1 → Fire
- 0 → No Fire

**Data Preprocessing**

The preprocessing pipeline includes:

- Handling missing & duplicate values
- Encoding categorical variables (region, class)
- Normalization & feature scaling
- Merging data from two regions into one dataset
- Correlation heatmap analysis to identify multicollinearity

**Modeling & Algorithms Used**

We trained four supervised machine learning regression models:

**Linear Regression** : Baseline model to understand linear relationships.
**Lasso Regression** : (L1 Regularization) - Helps with feature selection and coefficient shrinkage.
**Ridge Regression** : (L2 Regularization) - Mitigates multicollinearity and improves model stability.
**ElasticNet Regression** : (L1 + L2) - Balances feature elimination and coefficient shrinkage.

**Model Performance Summary**

**Ridge & ElasticNet performed the best overall.**

      Model	         R² Score (Approx.)	        Remarks

    Linear Regression	       ~0.91	          Good baseline performance
    Lasso Regression	       ~0.89	          Simplifies model by reducing coefficients
    Ridge Regression	       ~0.93	          Best stability & performance
    ElasticNet Regression	       ~0.92	          Balanced regularization



**Results & Insights**

- Fire Weather Indices (FFMC, DMC, DC, ISI) are the strongest predictors.
- Temperature and wind speed increase fire likelihood.
- Humidity and rainfall reduce fire risk.
- Regularization is crucial due to correlated environmental features.
- Best performing models: Ridge and ElasticNet.

**Conclusion**

This project demonstrates how regression-based ML models can effectively predict **forest fire behavior** using environmental data.
The analysis helps authorities improve fire prediction, prevention, and resource management strategies.
