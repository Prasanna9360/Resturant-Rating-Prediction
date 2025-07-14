# 🍽️ Restaurant Rating Prediction using Machine Learning

This project builds a machine learning model to **predict the aggregate rating of restaurants** using various features like service rating, food rating, price, cuisine, and more.

---

## 🎯 Objective

To develop a regression model that can predict the **aggregate rating** (on a scale from 0 to 2) of a restaurant based on its characteristics.

---

## 🧪 Dataset

The dataset used is sourced from a **multi-file restaurant dataset** that includes:
- `geoplaces2.csv`: Restaurant details (location, price, etc.)
- `rating_final.csv`: User ratings (target column)
- `chefmozcuisine.csv`: Cuisine types per restaurant

> All files were merged and preprocessed to form the final dataset for modeling.

---

## 🧹 Preprocessing Steps

1. Merged `rating_final`, `geoplaces2`, and `chefmozcuisine` on `placeID`.
2. Selected relevant columns:
   - `food_rating`, `service_rating`, `price`, `area`, `franchise`, `Rcuisine`
3. Handled missing values by replacing with `'Unknown'`.
4. Encoded categorical columns using `LabelEncoder`.
5. Split dataset into **training (80%)** and **testing (20%)**.

---

## 🤖 Model Used

- **Algorithm**: Linear Regression
- **Library**: `scikit-learn`

```python
from sklearn.linear_model import LinearRegression
model = LinearRegression()
model.fit(X_train, y_train)
