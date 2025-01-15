# Crab Age Prediction using Linear Regression

This repository demonstrates the application of linear regression to predict the age of crabs based on their physical attributes. The project makes use of a dataset from Kaggle, which contains the physical characteristics of crabs, with the aim of helping commercial crab farmers determine the optimal harvesting time for their crabs. This can improve harvesting efficiency, reduce costs, and increase profits.

## Table of Contents

- [Objective](#objective)
- [Dataset](#dataset)
- [Features](#features)
- [Data Processing](#data-processing)
- [Orange Software Workflow](#orange-software-workflow)
- [Model Evaluation](#model-evaluation)
- [License](#license)

## Objective

The main objective of this project is to predict the age of crabs using their physical features. For crab farmers, knowing the exact age of a crab helps in determining the best time to harvest. After a certain age, crabs' growth slows down, which makes predicting their age essential to optimize harvesting time, reducing costs, and maximizing profits.

## Dataset

The dataset used in this project is the [Crab Age Prediction Dataset from Kaggle](https://www.kaggle.com/datasets/sidhus/crab-age-prediction), which contains the following features:

- **Length**: The length of the crab
- **Diameter**: The diameter of the crab's carapace
- **Height**: The height of the crab's carapace
- **Weight**: The weight of the crab
- **Age**: The target variable (age of the crab)

The dataset consists of 3,893 rows and 7 features. The "sex" (gender) variable was excluded from the model due to its categorical nature, which makes it incompatible with linear regression without preprocessing.

### Dataset Details:

- 3893 rows of data
- 7 features (excluding the "sex" variable)
- No missing data

## Features

The main features used in the model are:

- **Length**: The physical length of the crab.
- **Diameter**: The width across the crab's carapace.
- **Height**: The height of the crab's carapace.
- **Weight**: The weight of the crab.

The target variable is **Age** (in years).

## Data Processing

The data was processed to remove non-numeric features and handle any inconsistencies. The dataset was cleaned and preprocessed, ensuring no missing data.

### Feature Selection:

The target variable for the model is **Age**, and the following features are used for prediction:

- Length
- Diameter
- Height
- Weight

The **sex** variable was removed from the dataset, as it is a categorical feature and incompatible with the regression model.

## Orange Software Workflow

Orange is an open-source data mining software used in this project to create a visual workflow for the linear regression analysis. It allows for easy manipulation of data and the implementation of machine learning algorithms like Linear Regression.

### Steps:

1. Load the dataset into Orange.
2. Preprocess the data to remove the non-numeric "sex" column.
3. Set up a linear regression model to predict the "Age" based on the physical attributes.
4. Evaluate the model's performance using test data.

## Model Evaluation

The linear regression model was evaluated using a training set with 66% of the data and a test set with the remaining 34%. The evaluation metrics include:

- Mean Absolute Error (MAE)
- R-squared (R²)
- Root Mean Squared Error (RMSE)

These metrics were used to assess the model's accuracy in predicting crab age.

### Correlation:

The widget rank in Orange was used to assess the correlation between features and the target variable. The most influential features for predicting age are:

- **Weight**
- **Diameter**
- **Length**

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
