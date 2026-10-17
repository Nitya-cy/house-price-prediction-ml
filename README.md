# house-price-prediction-ml
House price prediction using machine learning, feature engineering, and hyperparameter tuning.
# House Price Prediction Using Machine Learning

## Project Overview

This project predicts residential house prices using machine learning regression techniques. It involves data preprocessing, exploratory data analysis, feature engineering, model training, and hyperparameter tuning to estimate house prices from property characteristics.

## Dataset

- **Source:** [Kaggle – House Prices: Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data)
- **Dataset size:** 1,460 records
- **Target variable:** `SalePrice`
- **Problem type:** Supervised learning – Regression

## Technologies Used

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook

## Machine Learning Workflow

1. Loaded and explored the housing dataset.
2. Analysed missing values and duplicate records.
3. Performed exploratory data analysis to understand relationships between features and house prices.
4. Handled missing values and encoded categorical variables.
5. Engineered features such as `TotalSF`, `TotalBathrooms`, `TotalPorchSF`, `HouseAge`, and `RemodAge`.
6. Split the dataset into training and testing sets.
7. Trained and evaluated a Decision Tree Regressor.
8. Used GridSearchCV with cross-validation to tune model hyperparameters.
9. Evaluated the model using MAE, RMSE, and R² score.

## Model and Hyperparameter Tuning

The project used a Decision Tree Regressor and GridSearchCV to identify suitable hyperparameters.

**Best hyperparameters:**

- `max_depth`: 7
- `max_leaf_nodes`: 50
- `min_samples_leaf`: 10
- `min_samples_split`: 5

## Model Results

| Evaluation Metric | Result |
|---|---:|
| Cross-validation R² score | 0.7647 |
| Test R² score | 0.8249 |
| Training R² score | 0.8826 |
| Mean Absolute Error (MAE) | 22,691.35 |
| Root Mean Squared Error (RMSE) | 36,645.44 |

The tuned Decision Tree Regressor achieved a test R² score of approximately **0.825** in the reported experiment.

MAE represents the average absolute prediction error, while RMSE gives greater weight to larger errors. Both error metrics are expressed in the target variable's price units.

## Key Learnings

- Data cleaning and missing-value analysis
- Exploratory data analysis and data visualization
- Categorical encoding and feature engineering
- Regression model training and evaluation
- Hyperparameter tuning using GridSearchCV
- Model validation using cross-validation and regression metrics

## How to Run

1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. Download the dataset from the Kaggle link above.
4. Update the dataset file path in the notebook to match your local setup.
5. Open the notebook in Jupyter and run the cells in order.

## Disclaimer

This project is intended for educational purposes. Predictions are based on historical housing data and should not be considered current market valuations.

