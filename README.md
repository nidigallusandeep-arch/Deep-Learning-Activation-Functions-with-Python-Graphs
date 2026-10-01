# Deep Learning – Activation Functions

## 📌 Project Overview

This project demonstrates the most commonly used **Activation Functions in Deep Learning** using Python, NumPy, and Matplotlib.

Activation functions introduce **non-linearity** into neural networks and help them learn complex patterns.

## 🛠️ Technologies Used

* Python
* NumPy
* Matplotlib
* Jupyter Notebook

## 📚 Activation Functions Covered

### 1. Step Function

Returns either `0` or `1`.

```python
def step_function(x):
    if x > 0:
        return 1
    else:
        return 0
```

### 2. Linear Function

```python
y = x
```

The output can range from negative infinity to positive infinity.

### 3. Sigmoid Function

```python
y = 1 / (1 + np.exp(-x))
```

**Range:** `0 to 1`

**Common use:** Binary Classification

### 4. Tanh Function

```python
y = np.tanh(x)
```

**Range:** `-1 to +1`

### 5. ReLU Function

```python
def relu(x):
    return max(0, x)
```

**Range:** `0 to infinity`

ReLU is commonly used in hidden layers of neural networks.

### 6. Leaky ReLU

```python
def leaky_relu(x):
    if x > 0:
        return x
    else:
        return 0.01 * x
```

Leaky ReLU allows a small negative value instead of making all negative values zero.

### 7. Softmax Function

```python
x = np.array([2.0, 1.0, 0.5])

exp_x = np.exp(x)
y = exp_x / np.sum(exp_x)

print(y)
```

Softmax converts multiple values into probabilities whose total is `1`.

**Common use:** Multi-class Classification

## 📊 Visualization

The project uses **Matplotlib** to visualize the behavior of different activation functions.

Each graph helps understand how the input value is transformed into an output value.

## 🎯 Activation Function Summary

| Activation Function | Output Range         | Common Use                   |
| ------------------- | -------------------- | ---------------------------- |
| Step                | 0 or 1               | Basic binary output          |
| Linear              | -∞ to +∞             | Regression                   |
| Sigmoid             | 0 to 1               | Binary Classification        |
| Tanh                | -1 to +1             | Neural Network hidden layers |
| ReLU                | 0 to +∞              | Hidden Layers                |
| Leaky ReLU          | Small negative to +∞ | Hidden Layers                |
| Softmax             | 0 to 1               | Multi-class Classification   |

## 📁 Project Structure

```text
Activation_Functions_Deep_Learning/
│
├── Activation_Functions.ipynb
├── README.md
└── graphs/
```

## 💡 Key Learning

Through this project, I learned:

* What activation functions are
* Why activation functions are important
* How to implement activation functions using Python
* How to visualize activation functions using Matplotlib
* Where different activation functions are commonly used
* Difference between ReLU, Sigmoid, Tanh, Leaky ReLU, and Softmax

## 🚀 How to Run

Clone the repository:

```bash
git clone <your-repository-url>
```

Open Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Activation_Functions.ipynb
```

Run the cells to generate the activation-function graphs.
