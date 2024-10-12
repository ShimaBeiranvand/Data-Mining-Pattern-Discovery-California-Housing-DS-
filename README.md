# Data Mining & Pattern Discovery: California Housing Dataset

## Overview

This project focuses on applying data mining techniques to the California Housing dataset, which is widely used for research and educational purposes in understanding housing market dynamics. The goal is to extract meaningful patterns and insights that can inform predictions about housing prices and other related metrics.

## Objectives

- **Data Exploration**: Understand the structure and characteristics of the dataset.
- **Pattern Discovery**: Identify patterns and trends in housing prices based on various features.

## Dataset Description

Explanation of features:

    MedInc: Median income in block group.
    HouseAge: Median house age in block group.
    AveRooms: Average number of rooms per household.
    AveBedrms: Average number of bedrooms per household.
    Population: Population in block group.
    AveOccup: Average number of occupants per household.
    Latitude: Latitude of block group.
    Longitude: Longitude of block group.

The target variable is MedHouseVal, which represents the median house value in $100,000s.


## Methodology

1. **Data Preprocessing**:
   - Handle missing values , outliers , duplicate data and wrong data type.
   - Normalize and label encoding data as necessary.
     
2. **Creating New Features**:
   - ExtraRooms: counting the number of rooms except the bedrooms
   - ExNecRooms: whether the house has necessary rooms (kitchen and restroom) or not
   - AveSurf: measuring the average house area
   - NumHouse: counting the number of houses in the block
     
3. **Exploratory Data Analysis (EDA)**:
   - visualize data distribution with histograms.
   - showing relationships between features using correlation matrix.
   - finding outlier data points with z-score , iqr , box plot , isolation forrest , dbscan.

4. **Feature Selection**:
   - selecting omportant features with pca

## Tools and Technologies

- **Programming Language**: Python 3.9
- **Libraries**: 
  - Pandas 
  - NumPy 
  - Matplotlib and Seaborn 
  - Scikit-learn

## Conclusion

The Data Mining & Pattern Discovery project utilizing the California Housing dataset aims to uncover valuable insights into the housing market. By employing various data mining techniques, this project not only enhances understanding of market dynamics but also equips stakeholders with predictive tools for better decision-making in real estate investments. 

## Getting Started

To run this project, clone the repository and follow these steps:

1. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

2. Load the dataset:
   ```python
   import pandas as pd
   df = pd.read_csv('address/of/california_housing.csv')
   ```
3. Run the cells to explore data!
