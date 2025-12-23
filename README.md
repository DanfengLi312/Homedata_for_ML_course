# House Price Prediction

## Overview

This project builds and compares multiple statistical and machine learning models to predict residential house prices based on structural characteristics, location-related variables, and economic indicators. The goal is to evaluate model performance, interpretability, and robustness across different modeling approaches.

The project was developed as an end-to-end data science workflow, including data cleaning, feature engineering, model training, validation, and performance comparison.


## Motivation

Accurate house price prediction is a classic and practical problem in applied statistics and machine learning. This project aims to:
	•	Understand how different modeling assumptions affect prediction accuracy
	•	Compare linear models with regularization to tree-based and ensemble methods
	•	Balance predictive performance with interpretability


## Data

The dataset contains housing-related variables such as:
	•	Property characteristics (e.g., living area, number of bedrooms, age)
	•	Neighborhood or location indicators
	•	Sale conditions and transaction timing

## Data Processing
	•	Removed duplicates and invalid observations
	•	Handled missing values using imputation or deletion when appropriate
	•	Encoded categorical variables
	•	Standardized numerical variables for models sensitive to scale


## Methods

The following models were implemented and compared:
	•	Ordinary Least Squares (OLS) – baseline linear regression
	•	Ridge Regression – L2 regularization to reduce variance
	•	LASSO Regression – L1 regularization for feature selection
	•	Random Forest – non-linear ensemble tree model
	•	XGBoost – gradient boosting framework optimized for performance

## Model Training
	•	Data split into training and validation sets
	•	Hyperparameters tuned using cross-validation
	•	Models evaluated on the same validation dataset for fair comparison



## Evaluation Metrics

Model performance was assessed using:
	•	RMSE (Root Mean Squared Error)
	•	MAE (Mean Absolute Error)
	•	R² (Coefficient of Determination)

Lower RMSE and MAE indicate better predictive accuracy, while higher R² reflects stronger explanatory power.


## Results

Key findings from model comparison:
	•	LASSO achieved strong predictive performance while maintaining interpretability
	•	Tree-based models (Random Forest and XGBoost) captured non-linear relationships and interactions
	•	Ensemble models generally outperformed simple linear regression but required more tuning

Overall, model selection involved a trade-off between accuracy, complexity, and interpretability.


## How to Run
	1.	Clone the repository
	2.	Install required dependencies
	3.	Run the main script or notebook for model training and evaluation

git clone <repository-url>
cd house-price-prediction



## Key Takeaways
	•	Regularization improves generalization in high-dimensional settings
	•	Non-linear models capture complex patterns but may sacrifice interpretability
	•	Model comparison is essential before deployment


## Author

Danfeng Li
University of Illinois Urbana-Champaign


## License

This project is for academic and educational purposes only.
