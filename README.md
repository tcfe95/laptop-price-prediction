# Laptop Price Prediction using Regression Models

##  Project Overview

This project aims to predict laptop prices using multiple regression models.
The objective is to determine which model best captures the relationship between hardware specifications and laptop price.

---

##  Dataset

- File: `laptop_price.csv`
- Type: Structured dataset (CSV)
- Target Variable: Price
- Features include:
  - Brand
  - RAM
  - Storage
  - Processor
  - GPU
  - Screen Size
  - Weight
  - Operating System

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn
- Google Colab

---

## 🧠 Models Implemented

The following models were trained and compared:

| Model | R² Score |
|-------|----------|
| Linear Regression | 0.623 |
| Ridge Regression | **0.877** |
| Lasso Regression | 0.853 |
| Decision Tree | 0.628 |
| Random Forest | 0.739 |

---

## 📈 Best Model

✅ **Ridge Regression achieved the highest performance (R² = 0.877)**

This indicates that regularization significantly improved the model’s ability to generalize by reducing overfitting.

---

## 🔎 Key Steps

1. Data Cleaning
2. Handling Missing Values
3. One-Hot Encoding
4. Feature Scaling
5. Train/Test Split
6. Model Training
7. Performance Comparison

---

##  Business Insight

This model can be used in:
- E-commerce platforms
- Pricing optimization
- Market analysis
- Hardware value estimation

The strong performance of Ridge Regression shows that regularization plays an important role when dealing with correlated features.

---

##  How to Run

1. Install dependencies:
```
pip install -r requirements.txt
```

2. Open:
```
laptop_prediction.ipynb
```

---

## 👨‍💻 Author

Data Science Student  
Interested in Machine Learning and Predictive Modeling
