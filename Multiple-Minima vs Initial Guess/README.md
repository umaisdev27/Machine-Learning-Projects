# 📉 Multiple Minima & The Impact of Initial Guess

This project demonstrates the behavior of a mathematical function with **multiple minima**, and how the choice of **initial guess** can influence the result of optimization techniques such as gradient descent.

---

## 🧠 Function Definition

We are analyzing the following function:

$$
f(x) = x^4 - 4x^2 + 5
$$

This function has **multiple minima**, which makes it a great example to explore the effects of different starting points in optimization algorithms.

---

## 🔍 Visualizing the Function

### 📊 Full Plot Showing Multiple Minima

Here is the graph of the function, clearly showing its **two minima**:

<img width="1235" height="479" alt="Multiple Minima Graph" src="https://github.com/user-attachments/assets/6a6aa548-786c-48b6-ac85-d9f80affb186" />

---

## 🚀 Effect of Initial Guesses

### ✅ Initial Guess: `x = 0.2`

Starting near the **right-side minimum**, we observe the following optimization path:

<img width="1381" height="499" alt="Initial Guess = 0.2" src="https://github.com/user-attachments/assets/a7a8fe4d-a441-41c6-9ac4-ad16078eddff" />

### 🔁 Initial Guess: `x = -0.2`

Starting near the **left-side minimum**, the optimization leads to:

<img width="1381" height="499" alt="Initial Guess = -0.2" src="https://github.com/user-attachments/assets/412d1985-fe6c-4ba7-9569-7b8a6f73216d" />

---

## 🧩 Conclusion

This experiment highlights how initial guesses can steer optimization algorithms toward **different local minima**. In real-world problems with complex landscapes, choosing a good starting point can make all the difference!

---

## 🛠️ Tech Stack

- Python (Matplotlib, NumPy)
- Jupyter Notebook
- Basic Gradient Descent Implementation

---



