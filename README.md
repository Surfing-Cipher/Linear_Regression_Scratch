# 🔢 Linear Regression from Scratch — with Gradient Descent

This project demonstrates how to build a linear regression model **from scratch in Python** using **gradient descent** (without any machine learning libraries like `scikit-learn`). The goal is to understand the inner workings of linear regression by implementing the core logic manually and visualizing the model's performance.

---

## 📌 Project Highlights

* ✅ Implements **gradient descent**–based linear regression
* ✅ Uses the **Boston Housing** dataset to predict house prices (`medv`)
* ✅ Includes **training/testing split** and **loss monitoring**
* ✅ Plots a clean, aesthetically pleasing **regression line**

---

## 📁 Dataset

* **Dataset**: Boston Housing
* **Target variable**: `medv` (Median value of homes)
* **Feature used**: `rm` (Average number of rooms per dwelling)

---

## 🧮 How It Works

The model aims to learn the best-fit line `y = mx + b` by minimizing the **Mean Squared Error (MSE)** using gradient descent.

### 💡 Core Equations

* **Loss Function (MSE)**:

  $$
  E = \frac{1}{n} \sum_{i=1}^{n} (y_i - (mx_i + b))^2
  $$

* **Gradient Descent Updates**:

  $$
  m = m - \alpha \frac{\partial E}{\partial m} \quad ; \quad
  b = b - \alpha \frac{\partial E}{\partial b}
  $$

Where:

* $\alpha$ = learning rate
* $\frac{\partial E}{\partial m} = -\frac{2}{n} \sum x_i(y_i - (mx_i + b))$
* $\frac{\partial E}{\partial b} = -\frac{2}{n} \sum (y_i - (mx_i + b))$

---

## 🚀 How to Run

1. **Clone the repo**:

   ```bash
   git clone https://github.com/Surfing-Cipher/Linear_Regression_Scratch
   cd Linear_Regression_Scratch
   ```

2. **Install dependencies**:

   ```bash
   pip install pandas seaborn matplotlib
   ```

3. **Run the notebook**:
   Open the `.ipynb` file in Jupyter or VS Code and execute each cell step by step.

---

## 📊 Sample Output

```text
Epoch 0:     m = 1.56, b = 1.73, Loss = 153.22
Epoch 100:   m = 4.13, b = -10.56, Loss = 43.25
...
Epoch 1000:  m = 6.89, b = -28.74, Loss = 25.63
```

![plot](assets/fitted_line.png)

---
## 📌 Skills Demonstrated

* Python
* Data visualization (`seaborn`, `matplotlib`)
* Machine learning algorithms (from scratch)
* Code readability and modular design

---

## 📄 License

MIT License © 2025
