# House Price Prediction Using Linear Regression and Elastic Net

## Project Overview
This project implements a complete machine learning modeling workflow to predict house prices using linear regression techniques. The focus is on interpretability, robust validation, and understanding the key factors that influence property prices.

## Workflow
- Data loading and exploratory data analysis (EDA)
- Feature engineering and creation of derived features
- Pipeline-based preprocessing using scikit-learn
- Model training with Linear Regression and Elastic Net
- Cross-validation for model stability assessment
- Model comparison and final model selection
- Evaluation on a held-out test set
- Feature importance analysis and interpretation

## Models Used
- **Linear Regression**
- **Elastic Net Regression** (default and tuned via cross-validation)

## Model Selection
Both Linear Regression and Elastic Net achieved nearly identical performance across training, cross-validation, and test datasets. Given the negligible differences in MAE, RMSE, and R², Linear Regression was selected as the final model due to its simplicity, interpretability, and computational efficiency.

## Test Set Performance
The final model demonstrated stable and unbiased predictions on the test set. Error metrics remained consistent with training and cross-validation results, indicating good generalization and no evidence of overfitting or underfitting.

## Feature Importance
Feature importance was derived from standardized model coefficients to identify the key drivers of house prices. Results indicate that amenities, layout efficiency, and location-related features have a stronger impact on property value than raw size alone.

## Data
The dataset used in this project was obtained from Kaggle and is included in the repository for reproducibility.

**Data path:** 
data/real_estate_dataset.csv



## Tech Stack
- Python
- pandas, NumPy
- scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook
- GitHub

## How to Run
1. Clone or download the repository
2. Ensure the dataset is located in the `data/` directory
3. Open the notebook and run all cells from top to bottom

## Project Level
**Beginner–Intermediate**  
Skills demonstrated include regression modeling, feature engineering, pipeline construction, cross-validation, model evaluation, and interpretability.

## Future Work
- Explore non-linear models for comparison
- Refactor feature engineering into reusable modules
- Add uncertainty estimation or prediction intervals
- Extend validation across multiple random splits

