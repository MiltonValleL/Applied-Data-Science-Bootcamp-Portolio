# Classification Model for Megaline's Tariff Plan Recommendations

## 🎯 Project Objective

The mobile carrier Megaline discovered that many of its subscribers were using outdated legacy plans. To boost profitability and customer satisfaction, the company aimed to develop a model that could analyze subscriber behavior and recommend one of two new, more suitable plans: 'Smart' or 'Ultra'.

> The primary goal of this project was to build a classification model with the highest possible accuracy, meeting a minimum threshold of **0.75** on the test set to be considered a viable solution for the business.

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=seaborn&logoColor=white)

---

## 🚀 Project Workflow

The project was executed following a structured machine learning workflow:

1.  **Exploratory Data Analysis (EDA):** An initial analysis was conducted to understand the data, check for inconsistencies, and visualize the relationships between variables using a correlation matrix and pair plots.
2.  **Data Splitting:** The dataset was partitioned into three sets: a training set (60%), a validation set (20%), and a test set (20%) to ensure a robust and unbiased model evaluation.
3.  **Model Training & Hyperparameter Tuning:** Two different classification models were trained: `DecisionTreeClassifier` and `RandomForestClassifier`. Hyperparameter tuning was performed for each model to identify the configuration that yielded the highest accuracy on the validation set.
4.  **Model Evaluation & Selection:** After tuning, the performance of the best Decision Tree and Random Forest models was compared. The model with the superior accuracy was selected for final testing.
5.  **Sanity Checks:** The final chosen model was subjected to a series of sanity checks (e.g., comparing its performance against a trivial model) to confirm that it was learning meaningful patterns from the data.

---

## 📊 Results & Conclusion

> The final evaluation on the unseen test set demonstrated that the tuned **RandomForestClassifier** was the superior model, achieving an **accuracy of 80.4%**.
>
> -   **Random Forest Accuracy:** 80.4%
> -   **Decision Tree Accuracy:** 77.8%

💡 The `RandomForestClassifier` was selected as the final solution. Its higher accuracy is attributed to its ensemble nature, which combines multiple decision trees to produce a more robust and generalizable result, effectively reducing the risk of overfitting.

---

## 📁 Project Context

This project was completed as part of the **TripleTen Data Science Bootcamp**. The accompanying Jupyter Notebook (`.ipynb`) includes the original feedback and comments from my project reviewer. I have chosen to include this to provide valuable insight into my learning process and my ability to iterate on and improve my work based on constructive feedback, a key skill for any data scientist.


---

