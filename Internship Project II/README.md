The task in this project was to predict the "Accident risk index" for an insurance company. Since this is a Regression problem, the metric used is 
"Root mean squared error". The lower the RMSE value, the better is our model's prediction.

## Data Manipulation.
1. Handling missing values for categorical features.
2. Extracting features from the Date-Time column.
3. EDA and outlier checking for numerical features.
4. Dropping features with low variance.

## Data Cleaning
Cleaning the categorical features by removing punctuations and empty strings before the preprocessing step.

## Data Preprocessing
1. Cyclical Encoding - For Date-Time features.
2. Catboost Encoder - For Categorical features with high cardinality.
3. One Hot Encoding -  For Categorical features with very low cardinality.
4. Normalization - For Numerical features.

## Models (with hyperparametre tuning) [Randomized SearchCV]
1. Random Forest 
2. Light Gradient Boosting Regressor.

## Results
LGB Regressor gave the best result with a RMSE = 0.3213
