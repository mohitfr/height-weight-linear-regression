# 01 — Linear Regression: Predicting Height from Weight

A simple linear regression model that predicts a person's height from their weight using scikit-learn.

## Objective

Train a model to learn the relationship between weight and height, and evaluate how well it predicts on unseen data.

## Dataset

- File: `height_weight_lr.csv`
- Feature (Input): Weight
- Target (Output): Height

## Workflow

1. Load and explore the dataset
2. Visualize distributions and outliers
3. Check correlation between Weight and Height
4. Split into train/test sets (80/20)
5. Train a `LinearRegression` model using sklearn
6. Evaluate with MSE, RMSE, and R²
7. Plot regression line 
8. Predict height for new weight values

## Results

| Metric | Value |
|--------|-------|
| MSE | 15.8251 |
| RMSE | 3.9781 |
| R² | 0.9469 |

## How to Run

```bash
cd 01-linear-regression-height-weight
```

## Dependencies

```
pandas
numpy
matplotlib
scikit-learn
```

## Key Learnings

- How to structure a basic ML pipeline
- Difference between training and test sets
- What R² and RMSE tell us about model performance
- How to plot and interpret a regression line