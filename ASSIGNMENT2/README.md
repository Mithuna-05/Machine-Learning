# Loan Amount Prediction using Linear Regression

## Dataset
The dataset used in this experiment contains details of loan applicants, including:
- Personal income
- Employment details
- Credit score
- Property information
- And other demographic/categorical variables

### Preprocessing
- Dropped non-informative columns: `Customer ID`, `Name`, `Property ID`
- Handled missing values:
  - Numeric: filled with mean
  - Categorical: filled with mode
- Performed one-hot encoding for categorical columns
- Normalized all numeric features (excluding the target)

## Experiment Details

| Attribute                  | Details                                      |
|---------------------------|----------------------------------------------|
| **Experiment Name**       | Loan Amount Prediction (Experiment 1)        |
| **Student Name**          | Harini LV                                    |
| **Roll Number**           | 3122237001016                                |
| **Date**                  | 23-07-2025                                   |
| **Model Used**            | Linear Regression                            |
| **Dataset Size Used**     | 5,000 rows, 39 features                      |
| **Train/Test Split Ratio**| 80:20                                        |
| **Cross-Validation**      | Yes (K = 5 folds)                            |


## Results Summary

### Cross-Validation Results (K = 5)

| Fold   | MAE       | MSE           | RMSE      | R² Score |
|--------|-----------|----------------|-----------|----------|
| Fold 1 | 25323.8   | 1,195,270,000  | 34572.6   | 0.475    |
| Fold 2 | 23528.0   | 996,538,000    | 31568.0   | 0.532    |
| Fold 3 | 24752.0   | 1,157,960,000  | 34028.8   | 0.486    |
| Fold 4 | 24207.8   | 1,070,160,000  | 32713.3   | 0.513    |
| Fold 5 | 24688.1   | 1,126,780,000  | 33567.6   | 0.509    |
|**Average**| **24499.9** | **1,109,340,000** | **33,290.1** | **0.503** |

## Key Visualizations
- Loan Amount Histogram
- Income vs Loan Amount Scatter Plot
- Correlation Heatmap
- Boxplot of Income
- Actual vs Predicted Plot
- Residual Plot
- Feature Coefficients Bar Chart

## Observations
- R² Score around 0.50 indicates a moderate linear fit.
- Residuals are randomly scattered ⇒ good model fit
- Predictions closely align with actuals ⇒ decent accuracy
- Most influential features include: `Income (USD)`, `Credit Score`


## Conclusion
The linear regression model performs reasonably well on the preprocessed dataset. While the model is simple and interpretable, improvement is possible using advanced regressors (e.g., Random Forest, XGBoost).

