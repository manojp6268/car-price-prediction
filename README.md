# Car Price Prediction

## Project Overview
This project aims to predict car prices based on various features using machine learning techniques. It involves data preprocessing, model training, and evaluation to ensure accurate predictions. The primary goal is to assist potential car buyers and sellers by providing estimated car prices based on input features.

## Dataset
The dataset used in this project contains a collection of car attributes and corresponding prices. It includes various features that define the characteristics of the cars, such as:
- Make and Model
- Year of manufacture
- Mileage
- Engine size
- Fuel type
- Transmission type
- Color

This dataset can be sourced from various online car sales platforms or repositories that provide historical car price records.

## Methodology
The methodology followed in this project includes:
1. **Data Collection**: Gathering relevant data from reliable sources.
2. **Data Preprocessing**: Cleaning the dataset by removing duplicates, handling missing values, and normalizing data.
3. **Feature Selection**: Selecting the most impactful features for predicting car prices using correlation analysis.
4. **Model Training**: Using the RandomForestRegressor to train the model on the training dataset.
5. **Model Evaluation**: Validating the model's performance using metrics such as Mean Absolute Error (MAE) and R-squared values.
6. **Prediction**: Using the trained model to make predictions on new car data.

## Features
- Predictive modeling of car prices using random forests
- Ability to handle a variety of car attributes
- User-friendly interface for inputting car details for price estimation

## Model Used
This project employs the **RandomForestRegressor** from the `sklearn` library to predict car prices. This model is chosen for its robustness and ability to handle complex datasets effectively.

## Usage Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/car-price-prediction.git
   cd car-price-prediction

## Install the necessary dependencies:
  ```bash
  pip install -r requirements.txt 
  ```

## Run the model:
  ```bash
  python predict.py
  ```

Input the required car features as prompted to get the predicted price.
For more detailed instructions and examples, refer to the docs folder.
