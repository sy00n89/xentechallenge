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
Ensure following datasets are downloaded in your accessible location in order to successfully run the code. 

The code provided in this respiratory uses Google Drive to store csv files. 
- Train.csv
- Test.csv
- unlinked_masked_final.csv

## Troubleshooting

### Issue: Finding Matching Keys between Train.csv and unlinked_masked_final.csv

#### Problem Description:

During the data preprocessing phase, one of the challenges encountered was establishing a connection between the `Train.csv` and `unlinked_masked_final.csv` datasets. Unlike typical datasets with explicit linking columns, these datasets did not have direct indicators of a common key.

#### Solution:

To address this challenge, assumptions and custom columns were introduced to establish potential connections between the two datasets. Here's a brief overview of the approach:

1. **Customer Identification:**
   - Leveraged assumptions based on customer information to identify potential connections.
   - Created custom columns to link customers across the datasets.

2. **Transaction-Level Matching:**
   - Explored transaction-level details to establish associations between transactions in `Train.csv` and `unlinked_masked_final.csv`.
   - Assumed certain patterns or characteristics that might indicate a connection.

#### Recommendations:

1. **Review Custom Columns:**
   - Examine the custom columns introduced during data preprocessing for potential connections.
   - Ensure these assumptions align with the characteristics of the datasets.

2. **Explore Additional Features:**
   - Consider exploring additional features or creating new custom columns if the initial assumptions do not yield satisfactory connections.
   - Iterate on the data preprocessing steps based on insights gained from the datasets.

3. **Collaborate and Seek Feedback:**
   - Collaborate with team members or seek feedback from domain experts to refine the assumptions.
   - Utilize discussions or forums to share experiences and learn from the community.

Data preprocessing challenges often involve a degree of creativity and domain knowledge. Feel free to adapt the approach based on the specifics of your datasets and project requirements.


## Common Issues

 **Dependency Installation:** Ensure that you have installed all the required dependencies listed in the 'Prerequisites' section. Use the provided installation command to install them.

```
bash
pip install google-colab pandas numpy scikit-learn matplotlib
```

## Authors
[Gwonwoo (Justin) Cha] 


[SungChun Lee] 


[Siwoo (Reese) Yoon] (https://github.com/sy00n89)

## Version History
### Version 1.0.0 (2024-02-16)
- Initial release.
- Implemented data loading for Train, Test, and unlinked_masked_final datasets.
- Conducted basic data exploration and information display.
- Performed data preprocessing, including handling null values and feature engineering.
- Trained a logistic regression model on the training dataset.
- Evaluated the model's accuracy on the test dataset.
