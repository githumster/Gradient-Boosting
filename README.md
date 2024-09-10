# Gradient Boosting Implementation

This project focuses on the manual implementation of one of the most powerful machine learning algorithms — **Gradient Boosting**. The primary goal was to develop the boosting model from scratch and tune its parameters to achieve optimal performance.



## Dataset

The model was trained and evaluated using the `bank_data.csv` dataset, which contains information related to bank marketing campaigns and is commonly used for binary classification tasks. You can download the dataset from the following link:

- [bank_data.csv](https://www.dropbox.com/s/uy27mctxo0gbuof/bank_data.csv?dl=0)

## Project Overview

The following tasks were completed in this project:

1. **Implementation of Gradient Boosting**  
   Developed a custom gradient boosting model. The `Boosting` class was designed with the following key features:
   - **Base model**: A customizable base model class with user-defined hyperparameters.
   - **n_estimators**: Number of base models to train.
   - **Learning rate**: Controls the contribution of each model.
   - **Subsample**: Fraction of the training data used to fit each base model.
   - **Early stopping**: Stops training if validation performance does not improve over a specified number of rounds.
   - **Performance Plotting**: Generates a plot showing model performance over iterations.

2. **Training and Evaluation**  
   The model was trained and evaluated on different sets. We explored the effect of base model depth (1 to 30, with a step of 2) on performance, using the ROC-AUC metric to assess the results.

3. **Hyperparameter Tuning**  
   Used **Optuna** to fine-tune the hyperparameters of both the gradient boosting and the base models to optimize validation performance.


The performance was evaluated across various base model depths, and the best model depth was determined based on the trade-off between training and testing accuracy.

## Code Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/githumster/gradient-boosting.git
