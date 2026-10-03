# Regression Assignment – California Housing Dataset

## Project Objective

The objective of this project is to understand and implement regression techniques in supervised learning using a real-world dataset.

The **California Housing dataset** available in the `sklearn` library is used to predict the median house value based on different housing-related features.

## Dataset

The California Housing dataset is loaded using the `fetch_california_housing` function from `sklearn`.

It contains information about housing in California along with the corresponding median house values.

## Technologies Used

* Python
* Jupyter Notebook
* Pandas
* Scikit-learn

## Project Steps

### 1. Loading and Preprocessing

The following preprocessing steps are performed:

* Load the California Housing dataset using `fetch_california_housing`.
* Convert the dataset into a Pandas DataFrame.
* Check for missing values.
* Handle missing values using mean imputation.
* Split the dataset into training and testing sets.
* Perform feature scaling using `StandardScaler`.

Feature scaling is necessary because some regression algorithms, particularly Support Vector Regression (SVR), are sensitive to differences in feature magnitudes.

### 2. Regression Algorithms

The following regression algorithms are implemented:

1. **Linear Regression**

   * Models the relationship between the input features and the target variable using a linear equation.
   * Used as a baseline regression model.

2. **Decision Tree Regressor**

   * Uses decision-tree-based splits to predict continuous values.
   * Can capture nonlinear relationships between features and house prices.

3. **Random Forest Regressor**

   * Combines multiple decision trees to produce predictions.
   * Can handle complex relationships in the dataset.

4. **Gradient Boosting Regressor**

   * Builds decision trees sequentially, with each new tree improving the errors of the previous trees.
   * Can capture complex patterns in the data.

5. **Support Vector Regressor (SVR)**

   * Finds a function that predicts the target while keeping prediction errors within a specified margin.
   * Feature scaling is important for SVR.

## Model Evaluation

The performance of all five models is evaluated using:

* **Mean Squared Error (MSE)**
* **Mean Absolute Error (MAE)**
* **R-squared Score (R²)**

### Evaluation Criteria

* Lower **MSE** indicates smaller squared prediction errors.
* Lower **MAE** indicates smaller average prediction errors.
* Higher **R²** indicates better model performance.

The results of all models are presented in a comparison table in the Jupyter Notebook.

## Model Comparison

The model with the **highest R² score** is identified as the best-performing model.

The model with the **lowest R² score** is identified as the worst-performing model among the models tested.

The comparison is based on the MSE, MAE, and R² values obtained from the test dataset.

## Conclusion

This project demonstrates the implementation and comparison of five regression algorithms on the California Housing dataset. The models are evaluated using MSE, MAE, and R² to compare their predictive performance.
