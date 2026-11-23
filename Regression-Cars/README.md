**Original repo date:** 04.02.2022 – 20.05.2022

---

# Regression-Cars
Predicting car sale prices with **Random Forest Regression** and tuning its hyperparameters with **Grid Search**.

[Notebook with step-by-step explanations (in Turkish)](Regression%20Cars.ipynb)
<br>
[Code only](RFCcars.py)

## Dataset

[cars.csv](cars.csv) contains 963 car sales. The features are `age`, `gender`, `miles`, `debt` and `income`, and the target is the sale price (`sales`).

## Steps

1. Feature scaling with `StandardScaler` and a 75% / 25% train-test split
2. Training a `RandomForestRegressor` with 50 trees
3. Evaluating the model with 10-fold cross-validation
4. Searching for the best hyperparameters with `GridSearchCV`
5. Measuring the final result with the R² score

## Results

| Metric | Value |
|---|---|
| 10-fold cross-validation (mean R²) | 0.89 |
| R² score on the test set | **0.91** |
| Best parameters (Grid Search) | `criterion='mse'`, `max_features='sqrt'`, `n_estimators=250` |
