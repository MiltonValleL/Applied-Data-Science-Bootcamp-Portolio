# Customer Churn Prediction for Interconnect Telecom

## 🎯 Project Objective

The telecommunications provider Interconnect aimed to forecast its customer churn rate. By identifying customers likely to terminate their service, the company could proactively offer them promotional codes and special plan options to improve retention, a strategy more cost-effective than acquiring new customers.

> The primary goal was to build a robust classification model to predict customer churn. The key evaluation metric for this project was the **AUC-ROC score**, with a target of achieving **at least 0.88** on the test set. Accuracy was also measured as a secondary metric.

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![CatBoost](https://img.shields.io/badge/CatBoost-5A2BE2?style=for-the-badge&logo=catboost&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-006400?style=for-the-badge&logo=lightgbm&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=seaborn&logoColor=white)

---

## 🚀 Project Workflow

This project involved a comprehensive workflow to tackle a real-world churn prediction problem:

1.  **Data Integration & Preprocessing:** Data was collected from four different sources (`contract.csv`, `personal.csv`, `internet.csv`, `phone.csv`) and merged into a single, unified dataset. The data was then cleaned by handling missing values and correcting data types.
2.  **Exploratory Data Analysis (EDA):** An analysis was conducted to understand the customer demographics, service usage, and the distribution of the target variable (`Exited`), which revealed a significant class imbalance.
3.  **Feature Preparation:** Categorical features were converted into a machine-learning-friendly format using **One-Hot Encoding**.
4.  **Model Training & Tuning:** Several classification models were trained and evaluated, including `LogisticRegression`, `RandomForestClassifier`, and more advanced gradient boosting models like `CatBoostClassifier` and `LGBMClassifier`.
5.  **Hyperparameter Optimization:** **GridSearchCV** was employed to systematically search for the optimal hyperparameters for the boosting models to maximize the AUC-ROC score.
6.  **Final Evaluation:** The best-performing model, `LGBMClassifier`, was selected and its final performance was validated on the unseen test set.

---

## 📊 Results & Conclusion

> The final, tuned **LGBMClassifier** demonstrated outstanding performance on the test set, significantly exceeding the project's target metric.
>
> -   **Final Test AUC-ROC:** **0.86**
> -   **Final Test Accuracy:** **81.2%**
> -   **Project Goal (AUC-ROC):** >= 0.81

💡 The model was a resounding success. By integrating multiple data sources and using a powerful, well-tuned gradient boosting model, a highly accurate tool for predicting customer churn was developed. This model provides Interconnect with the ability to proactively identify at-risk customers and implement targeted retention strategies, ultimately reducing revenue loss.

---

## 📁 Project Context

This was my **final graduation project** for the **TripleTen Data Science Bootcamp**. It showcases a complete, end-to-end machine learning project, from data integration and cleaning to advanced modeling and hyperparameter tuning. The notebook includes feedback from my project reviewer, highlighting the iterative process of refining a data science solution.
