# Time Series Forecasting for Taxi Orders

## 🎯 Project Objective

The "Sweet Lift" taxi company collected historical data on taxi orders at airports. To optimize driver dispatch and vehicle allocation, they needed a model to forecast the number of taxi orders for the upcoming hour.

> The primary business goal was to build a time series forecasting model with a Root Mean Square Error (RMSE) value of no more than **48** on the test set.

---

## 📊 Data Source

The historical data on taxi orders was provided by the project stakeholder. The dataset is publicly available for download.

-   **Source:** [taxi.csv](https://practicum-content.s3.us-west-1.amazonaws.com/datasets/taxi.csv?etag=11687de0e23962e5a11c9d8ae13eb630)

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Statsmodels](https://img.shields.io/badge/Statsmodels-11557c?style=for-the-badge&logo=statsmodels&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-006400?style=for-the-badge&logo=lightgbm&logoColor=white)

---

## 🚀 Project Workflow

The project was approached using a standard time series forecasting methodology:

1.  **Data Preparation:** The initial dataset was loaded, its chronological order was verified, and the data was **resampled** into one-hour intervals to match the forecasting horizon.
2.  **Time Series Analysis (EDA):** The resampled time series was analyzed to identify underlying patterns. The series was decomposed into its **trend**, **seasonality**, and **residual** components.
3.  **Feature Engineering:** To prepare the data for machine learning models, several time-based features were created:
    -   **Calendar Features:** Hour of the day, day of the week, etc.
    -   **Lag Features:** Past values of the time series were used as predictors.
    -   **Rolling Mean:** A rolling mean was calculated to create a smoothed feature representing the recent trend.
4.  **Data Splitting:** The data was split into training, validation, and test sets, carefully maintaining the chronological order.
5.  **Model Training & Evaluation:** Several regression models were trained, including `LinearRegression`, `RandomForestRegressor`, and `LightGBM`, and evaluated on the validation set using the RMSE metric.
6.  **Final Testing:** The best-performing model (`LightGBM`) was evaluated on the unseen test set to determine its final predictive accuracy.

---

## 📊 Results & Conclusion

> The final evaluation on the test set confirmed that the **LightGBM** model delivered the best performance, achieving a final RMSE score that met the business requirement.
>
> -   **Final RMSE Score:** **39.9**
> -   **Project Goal:** <= 48

💡 The model successfully met the project's objective. By creating robust time-based features, the `LightGBM` model was able to effectively learn the patterns in the historical data and produce accurate forecasts, providing the company with a valuable tool for operational planning.

---

## 📁 Project Context

This project was completed as part of the **TripleTen Data Science Bootcamp**. The accompanying Jupyter Notebook (`.ipynb`) includes the original feedback and comments from my project reviewer. It demonstrates my ability to handle time series data, perform feature engineering specific to time-based problems, and build predictive forecasting models.

