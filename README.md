# 💻 Laptop Price Prediction using Regularized Regression Models

An end-to-end Machine Learning regression project designed to predict laptop prices based on hardware specifications. This repository benchmarks multiple linear and non-linear regression algorithms, highlighting the critical role of regularization techniques in handling highly correlated features.

---

## 📌 Project Overview

In the computer hardware market, pricing strategies are driven by complex combinations of specifications. The goal of this project is to build a reliable predictive model that captures the mathematical relationship between a laptop's hardware components and its final market price.

By evaluating multiple estimators, this project demonstrates:
* **Feature Engineering:** Handling categorical text variables with high cardinality.
* **Regularization Mechanics:** Overcoming overfitting caused by standard Ordinary Least Squares (OLS) estimation when using dummy variables.
* **Model Selection:** Benchmarking models using statistical metrics ($R^2$ Score).

---

## 📊 Dataset & Features

* **Data Source:** `laptop_price.csv` (Structured tabular dataset)
* **Target Variable:** `Price` (Continuous numerical variable)

### Core Features Evaluated:
* **Categorical:** Brand, Processor (CPU Type), GPU, Operating System.
* **Numerical:** RAM (GB), Storage Capacity (GB/TB), Screen Size (Inches), Weight (kg).

---

## 🛠️ Tech Stack & Dependencies

* **Language:** Python
* **Data Pipelines:** Pandas, NumPy
* **Machine Learning:** Scikit-learn
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** Google Colab / Jupyter Notebooks

---

## ⚙️ End-to-End Pipeline Workflow

1. **Exploratory Data Analysis (EDA):** Visualizing price distributions and identifying feature correlations.
2. **Data Cleansing:** Handling missing values and parsing unit strings (e.g., extracting numbers from "8GB" or "1.5kg").
3. **Feature Engineering & Encoding:** Implementing **One-Hot Encoding** for categorical attributes.
4. **Feature Scaling:** Applying standard scaling to numerical inputs to ensure uniform variance before regularization.
5. **Validation Strategy:** Utilizing a Stratified Train/Test Split.
6. **Model Benchmarking:** Training and optimizing 5 different regression architectures.

---

## 🧠 Models Benchmarked & Evaluation

The models were evaluated using the **Coefficient of Determination ($R^2$ Score)** on the test set:

| Regression Model | $R^2$ Score | Performance Status |
| :--- | :---: | :--- |
| **Ridge Regression (L2)** | **0.877** | 🏆 **Top Performer** |
| Lasso Regression (L1) | 0.853 | High Performance |
| Random Forest Regressor | 0.739 | Moderate Overfitting |
| Decision Tree Regressor | 0.628 | Baseline Non-Linear |
| Linear Regression (OLS) | 0.623 | Poor Generalization (High Variance) |

### 🔍 Key Engineering Insight:
Standard **Linear Regression (OLS)** suffered from high variance due to multicollinearity introduced by One-Hot Encoding. Introducing **Ridge Regression (L2 Regularization)** penalized large coefficients, effectively mitigating overfitting and boosting the $R^2$ score significantly to **0.877**.

---

## 📈 Real-World Business Applications

This predictive engine can be leveraged for:
* **E-commerce Dynamic Pricing:** Automating price suggestions for third-party sellers based on laptop specs.
* **Market Competitive Analysis:** Identifying undervalued or overvalued hardware configurations in the current market.
* **Procurement Optimization:** Helping corporate IT departments estimate hardware value and optimize bulk-purchasing budgets.

---

## 🚀 How to Run the Project Local Layout

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/laptop-price-prediction.git](https://github.com/your-username/laptop-price-prediction.git)
   cd laptop-price-prediction
