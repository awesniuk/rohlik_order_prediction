
# Rohlik Orders Forecasting Challenge - Ensemble Model

This notebook presents an ensemble model solution for the Rohlik Orders Forecasting Challenge on Kaggle. The goal of this competition is to predict the number of orders for different warehouses over a future period.

Competition: https://www.kaggle.com/competitions/rohlik-orders-forecasting-challenge

**Approach:**

The solution utilizes an ensemble approach combining several machine learning models, including:

* **Prophet:** Time series forecasting model for capturing seasonality and trend.
* **RandomForestRegressor:** Ensemble model based on decision trees.
* **XGBRegressor:** Gradient boosting model with regularization.
* **LGBMRegressor:** Gradient boosting model with leaf-wise tree growth.
* **CatBoostRegressor:** Gradient boosting model with categorical feature handling.
* **LinearRegression:** Simple linear regression model.
* **AdaBoostRegressor:** Ensemble model based on boosting weak learners.
* **DecisionTreeRegressor:** Basic decision tree model.
* **GradientBoostingRegressor:** Ensemble model based on gradient boosting.

These models are trained individually and their predictions are combined using a meta-model (Linear Regression) to produce the final forecast.

**Data Processing:**

The notebook includes various data processing steps such as:

* Handling missing values.
* Feature engineering (e.g., adding lagged features, cyclical encoding).
* Data transformation (e.g., mapping holiday names).

**Evaluation:**

The model is evaluated using Mean Absolute Percentage Error (MAPE). The notebook provides MAPE scores for individual warehouses and an aggregated MAPE score across all warehouses.

**Visualization:**

The notebook includes visualizations to illustrate:

* Orders over time by warehouse.
* Model predictions vs actual values.

**How to Use:**

1. Ensure you have the necessary libraries installed (e.g., prophet, scikit-learn, xgboost, lightgbm, catboost).
2. Download the competition data and place it in the appropriate directory.
3. Run the notebook cells sequentially.

**Further Improvements:**

* Explore other feature engineering techniques.
* Experiment with different model architectures and hyperparameters.
* Consider using a more sophisticated meta-model.
* Implement cross-validation for robust model evaluation.

This notebook provides a solid foundation for tackling the Rohlik Orders Forecasting Challenge. Feel free to adapt and improve upon this solution to achieve even better results!
