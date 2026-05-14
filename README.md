# 🚗 Car Price Prediction

> *Estimating market value from vehicle features — regression meets real-world pricing.*

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-RandomForest-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![Flask](https://img.shields.io/badge/Flask-Web_App-000000?style=flat-square&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Deployed](https://img.shields.io/badge/Deployed-Heroku-430098?style=flat-square&logo=heroku&logoColor=white)](https://heroku.com)

---

## What this does

Car pricing is influenced by dozens of variables — make, model, age, mileage, fuel type, transmission, and more. This project builds a regression model that learns from historical car sales data and predicts the market price of a vehicle based on its features.

Deployed as a Flask web application — enter the car details, get an estimated price instantly.

---

## The approach

```
Car Sales Dataset (datasets_33080_43333_car data.csv)
   │
   ▼
Exploratory Data Analysis
   │  ├── Price distribution and outlier analysis
   │  ├── Correlation between features and price
   │  └── Feature importance ranking
   │
   ▼
Data Preprocessing
   │  ├── Handling missing values and duplicates
   │  ├── Encoding categorical variables (fuel, transmission)
   │  ├── Feature engineering (car age from year)
   │  └── Train/test split
   │
   ▼
RandomForestRegressor
   │  ├── Ensemble of decision trees
   │  ├── Hyperparameter tuning
   │  └── Evaluation: MAE · RMSE · R²
   │
   ▼
Serialised Model (random_forest_regression_model.pkl)
   │
   ▼
Flask Web App → Live Price Estimation
```

---

## Dataset features

| Feature | Description |
|---|---|
| `Car_Name` | Make and model of the vehicle |
| `Year` | Year of manufacture |
| `Selling_Price` | Target — price at sale |
| `Present_Price` | Current ex-showroom price |
| `Kms_Driven` | Total kilometres driven |
| `Fuel_Type` | Petrol / Diesel / CNG |
| `Seller_Type` | Dealer or Individual |
| `Transmission` | Manual or Automatic |
| `Owner` | Number of previous owners |

---

## Model performance

| Metric | Description |
|---|---|
| MAE | Mean Absolute Error — average price deviation |
| RMSE | Root Mean Squared Error — penalises large errors |
| R² | Coefficient of determination — variance explained |

RandomForest was selected for its robustness to outliers, ability to handle mixed feature types, and strong performance on structured tabular data.

---

## Project structure

```
car-price-prediction/
│
├── car.ipynb                              ← Full EDA and model training
├── app.py                                 ← Flask application
├── main.py                                ← Core prediction logic
├── random_forest_regression_model.pkl     ← Serialised trained model
├── datasets_33080_43333_car data.csv      ← Car sales dataset
├── templates/                             ← HTML frontend
├── requirements.txt                       ← Dependencies
└── Procfile                               ← Heroku deployment config
```

---

## Run it locally

**Step 1 — Clone the repo**
```bash
git clone https://github.com/manojp6268/car-price-prediction.git
cd car-price-prediction
```

**Step 2 — Install dependencies**
```bash
pip install -r requirements.txt
```

**Step 3 — Run the app**
```bash
python app.py
```

Open `http://localhost:5000`, enter vehicle details, and get an estimated market price.

---

## Tech stack

- **Python** — core language
- **Scikit-learn** — RandomForestRegressor
- **Pandas / NumPy** — data processing and feature engineering
- **Flask** — web application framework
- **Heroku** — deployment platform
- **Jupyter Notebook** — model exploration and training

---

## Author

**Manoj Prakash** — Data Scientist & AI/ML Engineer
M.Sc. Data Science @ Universität Trier · ex-Oracle Cerner · ex-Huawei

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/manoj-p-a95b7b1a2)
[![Email](https://img.shields.io/badge/Email-manojp6268@gmail.com-1A2B4A?style=flat-square&logo=gmail)](mailto:manojp6268@gmail.com)
