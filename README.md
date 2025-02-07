# ML_Linear_Regression
```
Summary of Linear Regression Code Assignment
In this assignment, I implemented a Python function called linear_regression to perform polynomial regression on training data and evaluate the model on test data. The function was designed to handle datasets with varying degrees of polynomial features and incorporate L2 regularization. Below is an overview of my implementation and results:

## Repository Structure
- `data/`: Contains datasets used for testing (e.g., `f1.txt`, `boston_housing_training.txt`).
- `gifs/`: Contains GIFs visualizing model predictions for different parameters.


**1. Code Structure**
The code is split into two files:
    **linear_regression_main.py:** This file sets up the dataset paths, hyperparameters (degree and lambda), and calls the linear_regression function.
    **linear_regression.py**: This file contains the core implementation of the polynomial regression algorithm, including feature transformation, weight calculation, and evaluation.

**linear_regression.py:**
- Data Loading: Loads training and test data using numpy.loadtxt.
- Feature Transformation: Converts input features into polynomial features based on degree.
- Weight Calculation: Computes weights using the pseudo-inverse method (numpy.linalg.pinv) with   optional L2 regularization (lambda).
- Training Output: Prints learned weights (e.g., w0=%.4f, w1=%.4f).
- Test Evaluation: Predicts target values for test data and prints:
        Object ID, predicted output, target value, and squared error.

**Key Features**
- Supports polynomial regression for degrees 1–10.
- Incorporates L2 regularization to control overfitting.
- Handles datasets like Boston Housing and 1D datasets (f1.txt, f2.txt, f3.txt).

**Testing and Output**
Created GIFs to visualize how predictions change with different degree and lambda values.
![Linear_regression_f3_3_1](https://github.com/user-attachments/assets/b768d38b-14c4-46ac-a2ad-316be6630771)

**Insights**
- Higher degree allows fitting complex patterns but risks overfitting without regularization.
- Regularization (lambda > 0) smooths predictions and improves generalization.

```
