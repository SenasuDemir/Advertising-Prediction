# Advertising Prediction Project

This project explores the effect of advertising expenditures on sales figures. The goal is to determine which advertising medium—TV, Radio, or Newspaper—has the most significant impact on sales and to predict sales figures based on investment in each medium.

## Dataset Overview

The dataset contains 200 rows, each representing a different product or advertising campaign, with four columns:

- **TV**: Budget for TV advertising (in thousands of dollars).
- **Radio**: Budget for radio advertising (in thousands of dollars).
- **Newspaper**: Budget for newspaper advertising (in thousands of dollars).
- **Sales**: Sales for that campaign (in thousands of units).

### Dataset Information

- **Entries**: 200
- **Columns**: 4 (TV, Radio, Newspaper, and Sales)
- **Data Types**: Non-null float64

## Project Goals

1. **Predict Sales**: Create predictive models to estimate sales based on advertising investments.
2. **Analyze Advertising Effectiveness**: Determine which advertising medium (TV, Radio, or Newspaper) has the greatest effect on sales.

## Key Findings

- **Radio Advertising**: Has the highest impact on sales. Each additional investment unit in Radio results in the largest sales increase.
- **TV Advertising**: Provides a moderate impact on sales.
- **Newspaper Advertising**: Has the lowest impact on sales.

### Advertising Investment Impact on Sales

- **Most Effective**: Radio
- **Moderate Effect**: TV
- **Least Effective**: Newspaper

## Conclusion

To maximize sales, it is recommended to allocate the advertising budget in the following order:

1. **Radio**
2. **TV**
3. **Newspaper**

## Model Performance Summary

The following table summarizes the performance metrics of various regression models applied to this dataset. The models were evaluated based on **R-Squared**, **Root Mean Squared Error (RMSE)**, and **Mean Absolute Error (MAE)**.

| Model                   | R_Squared | RMSE     | MAE      |
|-------------------------|-----------|----------|----------|
| Gradient Boosting       | 0.984314  | 0.668991 | 0.538677 |
| XGBRegressor            | 0.984313  | 0.669011 | 0.559495 |
| DecisionTreeRegressor   | 0.964655  | 1.004222 | 0.771795 |
| Extra Tree              | 0.955874  | 1.122040 | 0.928205 |
| KNeighborsRegressor     | 0.929284  | 1.420437 | 0.949744 |
| Linear Regression       | 0.899526  | 1.693127 | 1.267680 |
| Ridge                   | 0.899522  | 1.693161 | 1.267706 |
| ElasticNet              | 0.897725  | 1.708236 | 1.277979 |
| Lasso                   | 0.896491  | 1.718508 | 1.284320 |

**Best Model**: Gradient Boosting and XGBRegressor provided the highest R-Squared values, indicating they explain the highest proportion of variance in the data.
