# Walmart-sales-prediction

## Objectives:
get an overview on sales and predict them as accurately as possible

## steps
- Understand the Dataset & cleanup (if required).
- Build Regression models to predict the sales.
- Also evaluate the models & compare their respective scores like R2, RMSE, etc.

### understanding the dataset
- I merged the datasets with pandas and cleaned it.
  - i used a right join to merge the training dataset with the feature dataset
- I performed time-series analysis on the dataset
  - i created new columns for day, month and year
  - i found the most profitable months and days.
- i engineered the features and selected the significant features for our model.
  - for the feature selection i used their p-values
  - feature engineering included ordinal encoding, one-hot encoding, and data mapping.
- I used a heatmap to see their various correlations.
- I used a piechart to display the sales made during the holiday periods.
- I used different scaling methods in scaling our data
  - i found the best performing scaler for different models.

### building regression models and evaluating them.
- I tried various regression models, the best performing being the RandomFOrest Regressor
  - its the best but require more computing power.
  - had an r2 of 0.974, and a MAE of 1443, adjusted r2 of 0.973
  - tuning its hyperparameters gave worse or similar results to it's untuned version.
  - I couldn't increase the number of iterations past a certain threshold due the limitations of my device.
- I plotted the predicted values versus the actual values.
  - my model performed alright.
