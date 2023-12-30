# SDSS Star Classification

## Overview

This Jupyter notebook uses the k-Nearest Neighbors (k-NN) algorithm to classify celestial objects from the Sloan Digital Sky Survey (SDSS) as stars, galaxies, or quasars. Here's a brief breakdown:

## Exploratory Data Analysis (EDA)

### Dataset

The dataset contains 100,000 observations with 17 features and a class column. Features include celestial coordinates and photometric filter readings. You can find the data [here](https://classic.sdss.org/dr7/).

### What the Script Does

- **Null Check:** Ensures a clean start by identifying null values.
- **Data Overview:** Quick insights into the dataset's shape, data types, and initial rows.
- **Class Distribution:** A bar chart shows how celestial objects are distributed among classes.

## The K-NN Journey

### Algorithm Basics

- **Data Prep:** Converts class string values to numerical format.
- **Feature Selection:** Picks key features for predicting the class.
- **Train-Test Split:** Divides the dataset for training and testing.
- **Normalization:** Uses min-max normalization for consistent scales.

### Model Training

- **Optimal K:** Explores different k values and plots test accuracy for each.
- **Fine-Tuning:** Configures the model with the best k.

### Performance Metrics

- **Confusion Matrix:** Illustrates model predictions for an unbalanced dataset.
- **Classification Report:** Provides precision, recall, and F1-score metrics.

## Visualizing Results

- **t-SNE Dimensionality Reduction:** Reduces data to 2D for visualizing predictions.
- **Scatter Plot:** A simple scatter plot visually represents model predictions.

## Requirements

- Python 3.x
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Acknowledgments

- Thanks to the [Sloan Digital Sky Survey](https://classic.sdss.org/dr7/) for providing the dataset.
