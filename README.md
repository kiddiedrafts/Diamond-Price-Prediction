# Diamond Price Prediction

This project implements a linear regression model to predict diamond prices based on various features. The dataset used is the Diamonds dataset from the `seaborn` library.

## Features

The model uses the following features for prediction:
- **Price:** Price in US dollars (\$326--\$18,823)
- **Carat:** Weight of the diamond (0.2--5.01)
- **Cut:** Quality of the cut (Fair, Good, Very Good, Premium, Ideal)
- **Color:** Diamond color, from J (worst) to D (best)
- **Clarity:** A measurement of how clear the diamond is (I1 (worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (best))
- **x:** Length in mm (0--10.74)
- **y:** Width in mm (0--58.9)
- **z:** Depth in mm (0--31.8)
- **Depth:** Total depth percentage (43--79)
- **Table:** Width of the top of the diamond relative to the widest point (43--95)


## Data Preprocessing

The following preprocessing steps are performed:
1. Removing outliers based on the interquartile range (IQR)
2. Encoding categorical variables to numeric values for model training

## Model Training

The linear regression model is trained using the preprocessed dataset, and its performance is evaluated using R² scores on both training and test sets.

## Model Performance

The model achieved the following R² scores:
- **Training Set:** 0.9109
- **Test Set:** 0.9111

## Requirements

To run this project, you'll need the following Python libraries:
- `pandas`
- `seaborn`
- `scikit-learn`
