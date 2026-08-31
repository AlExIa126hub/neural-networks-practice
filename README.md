# Neural Network from Scratch with NumPy

This project implements a small **feedforward neural network from scratch using NumPy**, with the goal of understanding how the mathematical concepts behind neural networks translate into code.

The network is designed for a simple binary classification problem and is trained using **backpropagation, the chain rule, and gradient descent**, without using machine learning libraries such as TensorFlow, PyTorch, or scikit-learn.

---

# Project Structure

The project follows the mathematical workflow used to train a neural network:

1. Data preparation
2. Network initialization
3. Forward propagation
4. Cost calculation
5. Backpropagation
6. Gradient descent
7. Iterative training
8. Convergence-based stopping

---

# Dataset

A small artificial dataset was created to simulate a real machine learning problem.

The network uses two input features:

- `study_hours`
- `sleep_hours`

and predicts whether a student passed:

- `0` → did not pass
- `1` → passed

The dataset contains four training examples.

| Study Hours | Sleep Hours | Passed |
|-------------|-------------|--------|
| 2.0 | 6.0 | 0 |
| 5.0 | 7.0 | 1 |
| 3.0 | 5.5 | 0 |
| 7.0 | 8.0 | 1 |

The input matrix is transposed so that each **column represents one training example**, following the mathematical convention used throughout the project.

---

# Neural Network Architecture

The implemented network contains:

- **2 input features**
- **1 hidden layer**
- **3 hidden neurons**
- **1 output neuron**

The architecture can be represented as:

```text
Input Layer          Hidden Layer          Output Layer

  x₁ ──────────────→   ○
                       │
  x₂ ──────────────→   ○ ───────────────→  ŷ
                       │
                       ○
