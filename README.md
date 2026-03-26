# 🧠 End-to-End Regression Modeling: From Scratch with Bias–Variance and Regularization

## 📌 Overview
This project implements an end-to-end machine learning regression pipeline from scratch using Python and NumPy, focusing on understanding core ML concepts rather than relying on high-level libraries.

The work explores linear, polynomial, and kernel-based regression models, along with key ideas such as:
- Bias–variance tradeoff  
- Model complexity  
- Regularization (Ridge)  
- Generalization via cross-validation  

---

## 🚀 Key Features

- Implemented Ordinary Least Squares (OLS) using:
  - Normal Equation  
  - Gradient Descent (with convergence tracking)

- Built Polynomial Regression (degree 2–10) from scratch  
- Performed feature standardization within CV folds  
- Used 10-fold Cross-Validation (with fixed seed for reproducibility)  
- Evaluated models using:
  - RMSE  
  - MAE  
  - R²  

- Implemented:
  - Ridge Regularization  
  - Robust Regression  
  - Learning Curves (data ablation study)

- Compared results with scikit-learn baselines

---

## 📊 Experiments & Analysis

### Linear vs Polynomial Regression
- Linear regression works well for simple datasets with low complexity  
- Polynomial models capture nonlinear patterns but risk overfitting  

Best polynomial degree selected via CV:
- Optimal: d = 6 (lowest RMSE)  
- Selected: d = 2 (via one-standard-error rule for simplicity & generalization)  

---

### Bias–Variance Tradeoff
- Linear models → high bias, low variance  
- Higher-degree polynomials → low bias, high variance  
- Increasing training data reduces variance and improves generalization  

---

### Learning Curves (Data Ablation)
- Training sizes: 20%, 40%, 60%, 80%  
- Observations:
  - Training error increases with more data  
  - Test error decreases and stabilizes  
  - Polynomial models initially overfit but improve with more data  

---

### Model Evaluation
- Used 10-fold cross-validation (random_state=42)  
- Reported metrics as mean ± standard deviation  
- Visualized:
  - Model fits  
  - Degree vs RMSE  
  - Learning curves  

---

### Comparison with scikit-learn
- Compared custom implementations with:
  - LinearRegression  
  - PolynomialFeatures + LinearRegression  

Findings:
- Similar performance overall  
- Minor differences due to numerical precision and implementation details  

---

## 🛠️ Tech Stack

- Python  
- NumPy  
- Matplotlib  
- scikit-learn (used only for validation & benchmarking)  

---



## 📈 Key Learnings

- Implementing models from scratch builds deeper intuition  
- Cross-validation is critical for reliable evaluation  
- Simpler models often generalize better  
- Regularization helps control overfitting  

---

## 🔗 Future Improvements

- Extend to multivariate regression  
- Add kernel regression  
- Optimize gradient descent (momentum, Adam)  
- Deploy as a web app  

---

## 👩‍💻 Author
Nandini Devaraj  
MS Computer Science | AI/ML Engineer  
