# 03 — Ridge & Lasso Regression: Predicting FWI from Weather & Fire Indices

Predicting the **Fire Weather Index (FWI)** from weather and fire danger rating features using Ridge and Lasso regression — and understanding why regularization matters.

## Objective

Build and compare Ridge and Lasso regression models to predict FWI, while learning how regularization controls overfitting and performs feature selection.

## Dataset

- **File:** `algerian_forest_fires.csv`
- **Source:** UCI Machine Learning Repository — Algerian Forest Fires Dataset
- **Region:** Two regions of Algeria — Bejaia and Sidi-Bel Abbes (June–September 2012)
- **Total Samples:** 244 (122 per region)

### Features Used

| Feature | Description |
|---------|-------------|
| `Temperature` | Daily max temperature (°C) |
| `RH` | Relative Humidity (%) |
| `Ws` | Wind Speed (km/h) |
| `Rain` | Rainfall (mm) |
| `FFMC` | Fine Fuel Moisture Code |
| `DMC` | Duff Moisture Code |
| `DC` | Drought Code |
| `ISI` | Initial Spread Index |
| `BUI` | Build Up Index |

### Target

| Feature | Description |
|---------|-------------|
| `FWI` | **Fire Weather Index** — overall fire danger rating |

## Why Ridge and Lasso?

Plain linear regression can overfit when features are correlated. Both methods add a **penalty term** to prevent this:

| Model | Penalty | Effect |
|-------|---------|--------|
| **Ridge** | Sum of squared coefficients (L2) | Shrinks all coefficients — keeps all features |
| **Lasso** | Sum of absolute coefficients (L1) | Drives some coefficients to zero — automatic feature selection |

## Workflow

1. Load and clean the dataset (handle the two-region structure)
2. EDA — distributions, correlation heatmap, FWI vs each feature
3. Preprocess — drop date/class columns, scale features with `StandardScaler`
4. Train/test split (75/25)
5. Train Ridge regression — tune alpha with cross-validation
6. Train Lasso regression — tune alpha with cross-validation
7. Compare Ridge vs Lasso vs plain Linear Regression
8. Analyze feature coefficients — see what Lasso zeroed out
9. Evaluate with MSE, RMSE, and R²

## Results

| Model | MSE | RMSE | R² |
|-------|-----|------|----|
| Linear Regression | *(fill)* | *(fill)* | *(fill)* |
| Ridge | *(fill)* | *(fill)* | *(fill)* |
| Lasso | *(fill)* | *(fill)* | *(fill)* |

## How to Run

```bash
cd 03-ridge-lasso-fwi
jupyter notebook ridge_lasso_regression.ipynb
```

## Dependencies

```
pandas
numpy
matplotlib
scikit-learn
```

## Key Learnings

- Why regularization is needed when features are correlated
- How Ridge and Lasso differ in their penalty approach
- How Lasso acts as a built-in feature selector
- Why feature scaling is essential before applying regularization
- How alpha controls the strength of the penalty