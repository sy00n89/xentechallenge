# Xente_Credit_Scoring_Challenge
***
## Ecommerce Loan Default Prediction
This repository contains code for predicting individuals’ loan default based on e-commerce transactions with given datasets. The project involves data preprocessing, feature engineering, and training a logistic regression model to successfully produce an accurate prediction. 

***
## Overview
Xente is a Ugandan e-commerce and financial service application that allows its users to make payments, get loans, and shop online. With given datasets including a sample of unique e-commerce transactions, the goal of this project is to predict loan default based on ecommerce transactions data. The dataset includes information on ecommerce transactions and associated loans, including whether or not a customer defaulted on their loan: 

Train.csv: E-commerce transactions and associated loans used to train the model.
Test.csv: E-commerce transactions and associated loans excluding customer loan default status, excluding additional loan-associated variables used to test the model.
unlinked_masked_final.csv: E-commerce transactions not linked to any other loans but associated with customers that have loan-linked e-commerce transactions. 

***
## Dependencies
Before running the code, ensure you have the following libraries installed:

- [`google.colab`](https://pypi.org/project/google-colab/): For interacting with Google Colab (if using Colab).
- [`pandas`](https://pandas.pydata.org/): For data manipulation and analysis.
- [`numpy`](https://numpy.org/): For numerical operations.
- [`scikit-learn`](https://scikit-learn.org/): For machine learning tasks.
- [`matplotlib`](https://matplotlib.org/) (optional): For plotting visualizations.

Install the dependencies using:

```
bash
pip install google-colab pandas numpy scikit-learn matplotlib
Help
```
If you encounter any issues or have questions about using this codebase for Ecommerce Loan Default Prediction, consider the following:

## Common Issues

 **Dependency Installation:** Ensure that you have installed all the required dependencies listed in the 'Prerequisites' section. Use the provided installation command to install them.

```
bash
pip install google-colab pandas numpy scikit-learn matplotlib
```

## Authors
names and contact info

## Version History
### Version 1.0.0 (2024-02-16)
- Initial release.
- Implemented data loading for Train, Test, and unlinked_masked_final datasets.
- Conducted basic data exploration and information display.
- Performed data preprocessing, including handling null values and feature engineering.
- Trained a logistic regression model on the training dataset.
- Evaluated the model's accuracy on the test dataset.
