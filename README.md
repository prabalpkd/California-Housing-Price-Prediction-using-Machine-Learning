# 🏡 California Housing Price Prediction using Machine Learning

This project is a simple yet insightful Machine Learning application that predicts housing prices in California using real-world data. It involves training multiple regression models and evaluating their performance based on accuracy, error, and execution time.

---

## 📚 Dataset Description

I used the **California Housing Dataset**, available via `scikit-learn`. This dataset is derived from the 1990 U.S. Census and contains information collected from California districts.

### ✅ Features (Independent Variables):
- `MedInc` – Median income in a block group
- `HouseAge` – Median house age in a block group
- `AveRooms` – Average number of rooms per household
- `AveBedrms` – Average number of bedrooms per household
- `Population` – Block group population
- `AveOccup` – Average house occupancy
- `Latitude` – Geographical latitude of the block group
- `Longitude` – Geographical longitude of the block group

### 🎯 Target (Dependent Variable):
- `MedHouseVal` – Median house value for households in a block group (in $100,000s)

---

## ⚙️ Project Workflow

### 1. 📥 Data Loading and Preprocessing
- Loaded the dataset using `fetch_california_housing()`.
- Converted it into a Pandas DataFrame.
- Checked for missing values (no NaNs found).
- Split the data into features `X` and target `y`.

### 2. 🔀 Train-Test Split
- Used `train_test_split` from `sklearn.model_selection`.
- 80% training data, 20% testing data.
- Used `random_state = 42` for reproducibility.

---

## 🧠 Models Implemented

We trained three regression models and compared their performances.

### 🔹 Model 1: Linear Regression

✅ R² Score: 0.575

❌ Mean Squared Error (MSE): 0.555

⏱ Time Taken: 0.0057 seconds

🔍 Used as a baseline model for comparison.

###  🔹 Model 2: Gradient Boosting Regressor

✅ R² Score: 0.775

❌ Mean Squared Error (MSE): 0.294

⏱ Time Taken: 5.92 seconds

🔍 Provided better accuracy but took longer time to train.

###  🔹 Model 3: XGBoost Regressor

✅ R² Score: 0.830

❌ Mean Squared Error (MSE): 0.222

⏱ Time Taken: 0.205 seconds

🚀 Best performing model in terms of both accuracy and speed.

##  📊 Performance Summary

| Model                 | R² Score  | MSE       | Time Taken (s) |
| --------------------- | --------- | --------- | -------------- |
| Linear Regression     | 0.575     | 0.555     | 0.0057         |
| Gradient Boosting     | 0.775     | 0.294     | 5.92           |
| **XGBoost Regressor** | **0.830** | **0.222** | **0.205**      |

### 📦 Libraries Used

pandas, numpy, scikit-learn, xgboost, time

###  📌 Key Takeaways

1. Started with a basic linear model to set a baseline.
2. Improved performance using ensemble techniques like Gradient Boosting.
3. Achieved the best results using XGBoost Regressor.
4. Demonstrated how boosting algorithms outperform traditional models in regression tasks.

###  🚀 Future Enhancements

1. Tune hyperparameters using GridSearchCV or RandomizedSearchCV
2. Visualize feature importance
3. Deploy the best model using Streamlit or Flask
4. Save model using joblib or pickle for reuse

### 🙌 Acknowledgment

  Thanks to Scikit-learn for providing the real-world California Housing dataset and to the open-source community for the powerful ML tools.


#### Author
  Prabal Kumar Deka
