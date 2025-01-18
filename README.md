# Bulldozer Sale Price Prediction

This repository contains an implementation of a machine learning model for predicting the sale prices of bulldozers. The project was developed as part of a Kaggle competition and achieved a **Root Mean Squared Logarithmic Error (RMSLE)** of **0.24**.

## Dataset

The dataset consists of three main files provided by the Kaggle competition:

- **Train.csv**: The training set, which contains data through the end of 2011. This dataset is used to train the model.
- **Valid.csv**: The validation set, containing data from January 1, 2012, to April 30, 2012. Predictions are made on this set throughout the majority of the competition, and the public leaderboard score is calculated based on this dataset.
- **Test.csv**: The test set, containing data from May 1, 2012, to November 2012. This dataset is used to determine the final ranking for the competition.

## Features

The dataset includes a wide range of features such as:

- **MachineID**: Unique identifier for each bulldozer.
- **SaleDate**: The date of sale.
- **ProductGroup**: The product category of the bulldozer.
- **Enclosure**: Type of enclosure (e.g., Open, EROPS, etc.).
- **YearMade**: The year the bulldozer was manufactured.

These features are used to predict the target variable, **SalePrice**, which represents the bulldozer's sale price.

## Requirements

- Python 3.8+
- Scikit-Learn 1.0+
- Pandas 1.3+
- NumPy 1.21+
- Matplotlib/Seaborn for visualization (optional)

Install the required packages with:

```
pip install scikit-learn pandas numpy matplotlib seaborn
```

## Model Pipeline

The implementation includes the following steps:

1. **Data Preprocessing**:
    - Handling missing values.
    - Encoding categorical variables.
    - Feature scaling and date feature extraction.
2. **Model Training**:
    - Training a Gradient Boosting model (e.g., XGBoost, LightGBM) or Random Forest.
3. **Evaluation**:
    - Calculating the RMSLE on the validation set to measure performance.

## Results

The model achieved an RMSLE of **0.24** on the validation set, demonstrating its effectiveness in predicting bulldozer sale prices.

## References

1. [Kaggle Bulldozer Price Prediction Competition](https://www.kaggle.com/)
2. Scikit-Learn Documentation: [https://scikit-learn.org](https://scikit-learn.org/)
