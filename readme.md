# Predicting the Sale Price of Bulldozers using Machine Learning

This project is an example of a machine learning model with the goal of predicting the sale price of bulldozers. 

The code for this project was developed by **Alvon Jovanus**.

## 1. Problem Definition

The problem we are trying to solve is: How well can we predict the future sale price of a bulldozer, given its characteristics and previous examples of how much similar bulldozers have been sold for?

## 2. Data

The data used in this project is downloaded from the Kaggle Bluebook for Bulldozers competition. You can download it [here](https://www.kaggle.com/c/bluebook-for-bulldozers/data).

## 3. Evaluation

The evaluation metric for this project is the RMSLE (root mean squared log error) between the actual and predicted auction prices. The goal for most regression evaluation metrics is to minimize the error. For more details on the evaluation of this project, check the [Kaggle competition page](https://www.kaggle.com/c/bluebook-for-bulldozers/overview/evaluation).

## 4. Features

Kaggle provides a data dictionary detailing all the features of the dataset. You can find this in the `Data` section of the competition page.

## 5. Modelling 

We're using the `RandomForestRegressor` from `sklearn.ensemble` to build our machine learning model. Here's a snippet of our model building process:

```python
from sklearn.ensemble import RandomForestRegressor

# Instantiate model 
model = RandomForestRegressor()

# Fit model
model.fit(X_train, y_train)

# Make predictions
preds = model.predict(X_valid)

```

For further detail, you can see the jupyter notebook file in this repository 😊.