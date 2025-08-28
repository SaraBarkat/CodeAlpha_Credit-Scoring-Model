# 📌 Credit Score Prediction using Decision Trees

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/ScikitLearn-ML-orange?logo=scikit-learn)
![Google Colab](https://img.shields.io/badge/Google-Colab-yellow?logo=googlecolab)

This project demonstrates how to **predict credit scores** using a **Decision Tree Regressor** in Python.  
The dataset contains demographic and financial information about customers.  

👉 You can run the project directly in Google Colab:  
[**Open in Colab**](https://colab.research.google.com/drive/1ssk8NaOcvuq2eh5eefEqy3WbYg6fxu1h?usp=sharing)  

---

## 📊 Dataset

The dataset (`bankloans_with_scores.csv`) includes:

- `age` → Age of the customer  
- `education` → Education level  
- `employ` → Years employed  
- `address` → Years at current address  
- `income` → Annual income  
- `debtinc` → Debt-to-income ratio  
- `creddebt` → Credit card debt  
- `othdebt` → Other debts  
- `default` → Default indicator (0/1)  
- `credit_score` → Target variable (numeric score)  

---

## 🎯 Objective

Predict the **credit_score** using the following features:

| Feature    | Description                  |
|------------|------------------------------|
| income     | Annual income                |
| debtinc    | Debt-to-income ratio         |
| creddebt   | Credit card debt             |
| othdebt    | Other debts                  |
| age        | Age of the customer          |
| employ     | Years employed               |
| address    | Years at current address     |
| education  | Education level              |
| default    | Default indicator (0 or 1)   |

---

## ⚙️ Model Training

The model used is a **DecisionTreeRegressor** from scikit-learn.  

### Steps:
1. Load and clean the dataset  
2. Split data into training and testing sets  
3. Train the Decision Tree model  
4. Evaluate with **Mean Absolute Error (MAE)**  

📌 **Performance:**  
The trained model achieved an **MAE ≈ 3.79**, meaning predictions are on average within ~3.8 points of the actual credit score.

---

## 💾 Outputs

- `credit_scoring_model.pkl` → Trained model saved with `joblib`  
- `cleaned_credit_data.csv` → Cleaned dataset  

---

## 🚀 Possible Improvements
- Hyperparameter tuning (`max_depth`, `min_samples_split`, etc.)  
- Try other algorithms (Random Forest, Gradient Boosting, XGBoost)  
- Deploy model as an API (Flask/FastAPI) or an interactive dashboard (Streamlit)  

---

## 📝 License
This project is licensed under the **MIT License**.  
Feel free to use and modify it.  

---
