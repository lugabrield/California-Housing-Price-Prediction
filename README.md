# California Housing Price Prediction

This project implements various regression techniques to predict housing prices in California using the California Housing dataset from the 1990 U.S. Census. The dataset contains information such as median income, house age, average number of rooms, and more, which are used to predict the median house value.

## Dataset

The California Housing dataset is available from [StatLib](https://www.dcc.fc.up.pt/~ltorgo/Regression/cal_housing.html) and contains 20,640 instances with 8 numeric, predictive attributes.

## Project Structure

The project explores three main regression models:

1. **Linear Regression** (using scikit-learn)
2. **Support Vector Regression** (SVR, using scikit-learn)
3. **XGBoost Regression** (using XGBoost library)

### Model Evaluation

The models are evaluated based on the following metrics:
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**

### Techniques

- Data splitting (80% training, 20% testing)
- Hyperparameter tuning using **GridSearchCV**

## Results

| Model                 | MSE   | RMSE  |
|-----------------------|-------|-------|
| Linear Regression      | 0.555 | 0.746 |
| Support Vector Machine | 1.332 | 1.154 |
| XGBoost               | 0.216 | 0.465 |

After hyperparameter tuning, the XGBoost model showed the best performance with an MSE of 0.216 and RMSE of 0.465.

## Dependencies

- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- XGBoost

You can install the required libraries using:
```bash
pip install -r requirements.txt
