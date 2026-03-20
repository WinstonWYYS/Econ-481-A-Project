# Econ-481-A-Project

This is the final project for Econ 481 A by Yushi Yao. 

This repository contains my final project for Econ 481A. The project replicates the general regression workflow of the De Cock-style housing price project using the Ames Housing dataset from Kaggle.

The goal is to compare two regression models for housing price prediction:

- **MODEL1**: a simpler, more interpretable regression model
- **MODEL2**: a more flexible model designed for better predictive performance

The analysis is implemented in the Jupyter Notebook `Progress.ipynb`, and the dataset used in the notebook is `train.csv`.


## Project Overview

This project uses the Ames Housing dataset to study how housing characteristics such as quality, size, age, garage capacity, and neighborhood are related to sale price.

Main steps in the project include:

- data cleaning and preprocessing
- handling missing values
- feature engineering
- train/validation split
- estimating two regression models
- comparing model performance on held-out validation data
- interpreting the tradeoff between interpretability and prediction accuracy


## Files in This Repository

- `Progress.ipynb` — main notebook containing the full analysis, model estimation, and results
- `train.csv` — dataset used in the notebook
- `README.md` — project description and instructions


## Data Source

The data used in this project comes from the Ames Housing dataset, accessed through the Kaggle House Prices competition dataset:

Ames Housing / House Prices: Advanced Regression Techniques

This project uses the Kaggle training dataset as a proxy for the dataset discussed in:

De Cock, D. (2011). *Ames, Iowa: Alternative to the Boston Housing Data as an End-of-Semester Regression Project*. Journal of Statistics Education, 19(3).


## Methodology

The project follows a replication-style workflow:

1. Remove irrelevant identifiers and extreme outliers
2. Split the sample into training and validation sets
3. Preprocess numeric, ordinal, and nominal variables
4. Construct derived features such as total square footage, total bathrooms, and house age
5. Estimate:
   - a compact explanatory model (**MODEL1**)
   - a richer predictive model (**MODEL2**)
6. Compare models using validation metrics such as RMSE, MAE, bias, and mean square error


## Main Conclusion

The results show that:

- **MODEL1** is easier to interpret and performs well as a benchmark model
- **MODEL2** achieves better out-of-sample predictive performance on the validation set
- There is a clear tradeoff between interpretability and predictive flexibility
