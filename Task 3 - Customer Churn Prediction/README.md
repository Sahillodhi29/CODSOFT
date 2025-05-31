# 🧠 Customer Churn Prediction

Predicting customer churn is critical for businesses to understand why users leave and take proactive steps to retain them. In this project, I developed a machine learning model to **predict whether a customer will churn or not**, using customer behavior and demographics.

## 📌 Problem Statement

Develop a model that predicts customer churn for a subscription-based business using historical customer data, including demographics and usage behavior.

Dataset Source: [Bank Customer Churn Dataset on Kaggle](https://www.kaggle.com/datasets/shantanudhakadd/bank-customer-churn-prediction)

---

## 🔍 Objective

- Explore the dataset and perform EDA (Exploratory Data Analysis)
- Build a predictive model using classification algorithms
- Evaluate and fine-tune the model for best accuracy
- Interpret model results and generate actionable insights

---

## 🗂️ Project Structure

Task-3-Customer-Churn-Prediction/
│
├── main.ipynb # Complete code from EDA to Model Evaluation
├── requirements.txt # List of required Python libraries
├── fine_best_model.pkl # Best model
├── dataset.csv # Customer churn dataset (not uploaded due to size/Kaggle policy)
└── README.md # Project documentation


## ⚙️ Technologies Used

- **Python**
- **Pandas**, **NumPy** – Data manipulation
- **Matplotlib**, **Seaborn** – Data visualization
- **Scikit-learn** – Machine Learning (Logistic Regression, Random Forest, GridSearchCV)
- **Jupyter Notebook** – Code & analysis

---

## 📊 Exploratory Data Analysis

- Checked null values, datatypes, duplicates
- Explored numerical and categorical features
- Visualized feature correlation and churn distribution
- Encoded categorical features and scaled numerical ones

---

## 🧠 Model Building

Tried and evaluated the following models:

| Model                | Accuracy |
|---------------------|----------|
| Logistic Regression | ~77%     |
| Random Forest       | ✅ **81.85%** (Best) |
| Gradient Boosting   | ~79%     |

- **Random Forest Classifier** gave the best performance with:
  - Accuracy: **81.85%**
  - Precision (Churn Class): **0.98**
  - Recall (Churn Class): **0.11**
  - F1-Score (Churn Class): **0.20**

---

## 📈 Evaluation Metrics

- **Confusion Matrix**
- **Classification Report**
- **Accuracy, Precision, Recall, F1-score**
- **ROC-AUC Curve**

> Note: While accuracy is high, **recall for churned customers was low**, which is a common challenge in imbalanced datasets. Further optimization possible using SMOTE or cost-sensitive learning.

---

## 🧪 Future Improvements

- Apply advanced resampling techniques like **SMOTE** or **ADASYN**
- Try **XGBoost** or **CatBoost** for better performance
- Perform **Feature Selection** to reduce overfitting
- Integrate with a dashboard (Tableau/Streamlit) to visualize churn risk

---

## 🏁 Final Outcome

- ✅ Successfully predicted churn with ~82% accuracy
- 📈 Identified key features contributing to churn
- 🎯 Deployed a ready-to-tune notebook for future experimentation

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/Sahillodhi29/CODSOFT.git
