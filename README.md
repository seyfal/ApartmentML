# Apartment Price Prediction

This repository contains code for predicting apartment prices using machine learning techniques. The dataset used is a collection of apartment listings with various features such as size, number of bedrooms, bathrooms, location, and amenities.

## Dataset

The dataset contains the following columns:

- `id`: A unique identifier for each apartment listing (not used as a feature)
- `category`: The category of the listing (not used as a feature)
- `title`: The title of the listing (not used as a feature)
- `body`: The description of the listing (not used as a feature)
- `amenities`: The amenities offered by the apartment (not used as a feature)
- `bathrooms`: The number of bathrooms in the apartment (feature)
- `bedrooms`: The number of bedrooms in the apartment (feature)
- `currency`: The currency of the listed price (not used as a feature)
- `fee`: Additional fees associated with the listing (not used as a feature)
- `has_photo`: Indicates whether the listing has a photo (not used as a feature)
- `pets_allowed`: Indicates whether pets are allowed in the apartment (feature)
- `price`: The listed price of the apartment (target variable)
- `price_display`: The displayed price format (not used as a feature)
- `price_type`: The type of price (e.g., monthly, weekly) (not used as a feature)
- `square_feet`: The area of the apartment in square feet (feature)
- `address`: The address of the apartment (not used as a feature)
- `cityname`: The city where the apartment is located (feature)
- `state`: The state where the apartment is located (feature)
- `latitude`: The latitude coordinate of the apartment (feature)
- `longitude`: The longitude coordinate of the apartment (feature)
- `source`: The source of the listing (not used as a feature)
- `time`: The time when the listing was posted (not used as a feature)

## Data Preprocessing - Subject to Change

The code provided in the Python file performs the following data preprocessing steps:

1. Loading the dataset from a CSV file.
2. Dropping irrelevant columns.
3. Handling missing values in the `bathrooms`, `bedrooms`, `latitude`, `longitude`, `pets_allowed`, `cityname`, and `state` columns.
4. One-hot encoding categorical features (`pets_allowed`, `cityname`, and `state`).
5. Splitting the data into training and test sets.
6. Ensuring no NaN values are present in the training and test sets.

## Models

The repository currently includes the following models:

### 1. Linear Regression

A simple linear regression model is implemented as a baseline. The code evaluates the model's performance using mean squared error (MSE) and R² score.

### 2. Random Forest Regression

A random forest regression model is also implemented, and its performance is evaluated using MSE and R² score. The code demonstrates that the random forest model outperforms the linear regression model for this dataset.

## Getting Started

1. Clone the repository:

```
git clone https://github.com/your_username/apartment-price-prediction.git
```

2. Install the required Python packages:

```
pip install -r requirements.txt
```

3. Navigate to the desired notebook (e.g., `paste.txt`) and run the cells.

## Future Work

Future work may include:

- Exploring other machine learning models, such as gradient boosting or neural networks.
- Conducting more extensive feature engineering and selection.
- Investigating the impact of different hyperparameters on model performance.
- Deploying the best-performing model as a web application or API.

## Acknowledgments

- https://archive.ics.uci.edu/dataset/555/apartment+for+rent+classified
