# 📈 3D Visualization of a Non-Linear Function

This project demonstrates the 3D visualization of a non-linear function involving an exponential decay based on the squared distance from the origin.

---

## 🔣 Function Definition

We define the function:

$$
f(x, y) = \frac{1}{r + 1}, \quad \text{where} \quad r = 3^{-x^2 - y^2}
$$

This function resembles a **smooth bump** centered at the origin, and is useful for testing gradients and 3D plots.

---

## 🌀 Step 1: Basic Visualization

First, we visualized the function without any gradient or derivatives. This gives us an idea of the shape and distribution of the surface:

<img width="1190" height="1190" alt="Initial Surface Plot" src="https://github.com/user-attachments/assets/20cb2278-3f5b-41b0-9e0f-a3b376575094" />

---

## ✍️ Step 2: Adding Derivatives

We then introduced partial derivatives to observe the **gradient** of the function.

### Partial Derivative with respect to `x`:
$$
\frac{\partial f}{\partial x} = \frac{2x \ln(3) \cdot 3^{-x^2 - y^2}}{\left(3^{-x^2 - y^2} + 1\right)^2}
$$

### Partial Derivative with respect to `y`:
$$
\frac{\partial f}{\partial y} = \frac{2y \ln(3) \cdot 3^{-x^2 - y^2}}{\left(3^{-x^2 - y^2} + 1\right)^2}
$$

We constructed:
- `x` component → $\frac{\partial f}{\partial x}$
- `y` component → $\frac{\partial f}{\partial y}$
- `z` component → $f(x, y)$

---

## ⚙️ Step 3: Optimization & Performance

Initially, we used **symbolic computation** (via `sympy`) for differentiation, but it was **too slow** for larger grids.

So, we switched to **numerical derivative functions** and created **2D arrays** using `NumPy`, which greatly improved performance.

---

## 📊 Final Graph

After optimizing the calculations, we plotted the full 3D surface including gradients:

<img width="1190" height="1190" alt="Final Gradient Surface Plot" src="https://github.com/user-attachments/assets/2a10c0bd-c111-43f4-a9d3-31b4ed58b14c" />

---

## 🛠️ Tools & Libraries

- Python
- NumPy
- Matplotlib (for 3D plotting)
- SymPy (initial symbolic derivatives)

---


