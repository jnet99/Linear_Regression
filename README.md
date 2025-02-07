# ML_Linear_Regression
```
Summary of Linear Regression Code Assignment
In this assignment, I implemented a Python function called linear_regression to perform polynomial regression on training data and evaluate the model on test data. The function was designed to handle datasets with varying degrees of polynomial features and incorporate L2 regularization. Below is an overview of my implementation and results:

1. Code Structure
The code is split into two files:
linear_regression_main.py: This file sets up the dataset paths, hyperparameters (degree and lambda), and calls the linear_regression function.

linear_regression.py: This file contains the core implementation of the polynomial regression algorithm, including feature transformation, weight calculation, and evaluation.

2. Key Steps in the Implementation
- Data Loading and Preprocessing:
The training and test datasets were loaded using numpy.loadtxt.

The input features (X_train and X_test) and target outputs (y_train and y_test) were separated from the loaded data.

- Polynomial Feature Transformation:

    A helper function, polynomial_features, was implemented to transform the input features into polynomial features based on the specified degree.

    For example:
        * If degree = 1, the features remained linear.
        * If degree = 2, squared terms were added for each feature.
        * If degree = 3, cubic terms were added, and so on.

This transformation allowed the model to fit polynomial functions of varying complexity to the data.




![Linear_regression_f3_3_1](https://github.com/user-attachments/assets/31f19961-61cb-4b26-a595-b7d75a20e5ab)
