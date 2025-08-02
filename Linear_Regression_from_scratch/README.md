
# 📊 Linear Regression from Scratch

This project demonstrates how to build a **Linear Regression model from scratch using NumPy** and compare its performance with **Scikit-learn's LinearRegression**. The dataset used is the **Diabetes Dataset** from Scikit-learn.

---

## 🚀 Features

- Implements Linear Regression manually using:
  - Gradient Descent
  - Mean Squared Error loss
  - Analytical computation of gradients
- Trains the model and prints loss at intervals
- Evaluates model performance using **R² Score**
- Compares with Scikit-learn’s implementation
- Visualizes actual vs predicted values using Matplotlib

---

## 📁 Dataset

- **Source**: `sklearn.datasets.load_diabetes`
- **Target**: Disease progression metric
- **Features**: 10 (age, sex, BMI, blood pressure, etc.)

---

## 📌 Requirements

```bash
pip install numpy pandas scikit-learn matplotlib
```

---

## 🧠 Training

The training function:
- Initializes weights and bias
- Runs gradient descent for `1,000,000` epochs
- Updates weights using computed gradients
- Logs training loss every `1000` steps

---

## 📉 Evaluation

- Metric used: **R² Score**
- Compared with Scikit-learn model’s MSE
- Visual comparison of predicted vs actual values using scatter and line plots

---

## 📈 Output Sample

- Prints weight and bias during training
- Plots prediction vs actual for one feature

---

## 🔍 Code Structure

- `predict(X, w, b)` — Prediction function
- `compute_loss(y_true, y_pred)` — Mean Squared Error
- `compute_gradients(...)` — Derivative-based updates
- `train(...)` — Runs the training loop
- `r2_score(...)` — Manual R² score implementation

---

## 📷 Visualization

- Compares predictions on the first feature (`X[:, 0]`)
- Red line: predicted values
- Blue dots: actual data points

---

## ✅ Conclusion

This notebook provides a clear understanding of how linear regression works internally, and gives a side-by-side comparison with Scikit-learn's black-box implementation.
