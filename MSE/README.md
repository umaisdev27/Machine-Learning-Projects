
---

# 📊 Mean Squared Error (MSE) & Linear Regression

This project demonstrates the implementation of **Mean Squared Error (MSE)**, **Residual Sum of Squares (RSS)**, and the use of **Gradient Descent** to minimize error in linear regression models. We also explore 3D visualizations to understand the cost function surface.

---

## 📐 Mathematical Formulations

### Residual Sum of Squares (RSS)

$$
RSS = \sum_{i = 1}^{n} \left( y^{(i)} - h_\theta(x^{(i)}) \right)^2
$$

### Mean Squared Error (MSE)

$$
MSE = \frac{1}{n} \sum_{i = 1}^{n} \left( y^{(i)} - h_\theta(x^{(i)}) \right)^2
$$

Or equivalently:

$$
MSE = \frac{1}{n} \sum_{i = 1}^{n} \left( y - \hat{y} \right)^2
$$

---

## 📈 Linear Regression

We implemented a basic linear regression model to fit a line through the data by minimizing the MSE.

<p align="center">
  <img width="562" height="438" alt="Linear Regression Plot" src="https://github.com/user-attachments/assets/d1485f27-af4b-4773-8e5b-4e8842144fa0" />
</p>

---

## 🔁 Partial Derivatives (Gradient Descent)

To minimize the MSE, we use the **partial derivatives** with respect to the parameters $\theta_0$ and $\theta_1$:

### Gradient with respect to $\theta_0$:

$$
\frac{\partial MSE}{\partial \theta_0} = -\frac{2}{n} \sum_{i=1}^{n} \left( y^{(i)} - \theta_0 - \theta_1 x^{(i)} \right)
$$

### Gradient with respect to $\theta_1$:

$$
\frac{\partial MSE}{\partial \theta_1} = -\frac{2}{n} \sum_{i=1}^{n} \left( y^{(i)} - \theta_0 - \theta_1 x^{(i)} \right) \cdot x^{(i)}
$$

---

## 🧠 3D Cost Function Visualization

The following plot shows the surface of the cost function (MSE) across different values of $\theta_0$ and $\theta_1$:

<p align="center">
  <img width="462" height="438" alt="image" src="https://github.com/user-attachments/assets/5ca6a461-aee5-4848-b8b2-bfc7e3657ddf" />



---

## ✅ Final Optimized Regression

The graph below represents the result after applying gradient descent optimization to minimize the MSE.

<p align="center">
  <img width="462" height="438" alt="image" src="https://github.com/user-attachments/assets/cf1bd496-bfc2-455d-ae30-9ddef6371831" />



</p>

---

### 🚀 Summary

* Implemented linear regression using MSE as cost
* Used gradient descent for optimization
* Visualized the cost surface in 3D
* Explored the impact of different parameter values on cost

---

