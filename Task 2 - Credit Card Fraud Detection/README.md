# 🛡️ Task 2: Credit Card Fraud Detection Using Machine Learning

## 📌 Overview

This project is part of my machine learning internship where the goal was to build a high-performance fraud detection model using transaction data. The objective was to identify fraudulent credit card transactions with high accuracy, leveraging a variety of features such as transaction amount, geolocation, and time-based attributes.

> ✅ Final Model Achieved **99.78% Accuracy** using Random Forest Classifier.

---

## 📂 Dataset Information

The dataset contains historical credit card transaction data with the following key features:

- `amt`: Transaction amount
- `lat`, `long`: Geolocation of the user
- `city_pop`: Population of the city
- `age`: Age of the customer
- `transaction_hour`, `day_of_week`: Extracted from timestamp
- `category_*`: Encoded merchant categories

---

## 🧠 ML Workflow

The steps followed:

1. **Data Preprocessing**
   - Dropped irrelevant or high-cardinality columns (like `trans_date_trans_time`, merchant name)
   - Extracted `hour` and `day_of_week` from timestamp
   - Binned `amt` into quantile-based categories
   - Encoded categorical columns using Label Encoding

2. **Model Training**
   - Tested multiple models: Logistic Regression, Decision Tree, Random Forest, etc.
   - Used train-test split to evaluate performance
   - Tracked accuracy of each model for comparison

3. **Best Model**
   - Random Forest Classifier was the best performer with:
     ```
     ✔️ Accuracy: 99.78%
     ```

4. **Model Saving**
   - Saved the final trained model as `best_model.pkl` using `joblib`

---
