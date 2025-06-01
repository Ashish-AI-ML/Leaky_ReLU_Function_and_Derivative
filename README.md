# ⚡ Leaky ReLU Function and Derivative – Visualization and Guide

This project demonstrates the **Leaky ReLU** activation function, its **derivative**, and explains its advantages compared to the standard ReLU. It includes a visualization, Python implementation, and key use cases in deep learning.

---

## 📘 What is Leaky ReLU?

**Leaky ReLU (Rectified Linear Unit)** is an activation function designed to overcome the **dying ReLU problem** — where ReLU neurons become inactive and stop learning due to zero gradients.

### 🔣 Mathematical Definition

\[
f(x) =
\begin{cases}
x & \text{if } x \geq 0 \\
\alpha x & \text{if } x < 0
\end{cases}
\]

- \( \alpha \): Small constant (usually 0.01)
- \( x \): Input to the neuron

---

## 🔁 Derivative of Leaky ReLU

\[
f'(x) =
\begin{cases}
1 & \text{if } x \geq 0 \\
\alpha & \text{if } x < 0
\end{cases}
\]

- Gradient is always non-zero ⇒ helps prevent neurons from "dying."

---

## 📈 Visualization

This project visualizes:
- The Leaky ReLU function
- Its derivative
- A comparison with standard ReLU

You’ll gain insights into:
- How Leaky ReLU behaves over different input ranges
- Why it's more robust in training deep networks

---

## 🧠 Why Use Leaky ReLU?

| Problem with ReLU       | Leaky ReLU Advantage               |
|-------------------------|------------------------------------|
| Gradient = 0 for \( x<0 \) | Gradient = \( \alpha \), keeps learning |
| Dead neurons             | Keeps units partially active       |
| Sparse activation only   | Allows negative signal flow        |

---

