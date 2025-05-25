# Numerical Optimizers from Scratch in Python
This repository contains implementations of various numerical optimization algorithms from scratch using only Python (with NumPy for vectorized operations). The project covers foundational gradient-based optimizers, advanced variants, and second-order methods for both single and multivariate optimization problems.
# Implemented Algorithms
1. Gradient Descent (GD)
Vanilla Gradient Descent: Basic iterative optimization for minimizing loss functions by updating parameters in the direction of the negative gradient.
Multivariate Support: Extended to handle vectorized operations for linear regression.

2. Gradient Descent Variants
Batch Gradient Descent: Computes gradients using the entire dataset (accurate but slow for large data).
Stochastic Gradient Descent (SGD): Updates parameters per sample (fast but noisy convergence).
Mini-Batch Gradient Descent: Balances batch and SGD by using small random subsets of data.

3. Momentum-Based Methods
Momentum: Accelerates convergence by accumulating a velocity vector in the direction of persistent reduction.
Nesterov Accelerated Gradient (NAG): "Looks ahead" to adjust momentum based on the future approximate position.

4. Adaptive Learning Rate Methods
Adagrad: Adapts learning rates per parameter using historical squared gradients (suited for sparse data).
RMSprop: Improves Adagrad by exponentially decaying the squared gradient average.
Adam: Combines Momentum and RMSprop with bias correction for adaptive learning rates.

5. Second-Order Methods
Newton’s Method: Uses exact Hessian (2nd derivative) for faster convergence but computationally expensive.
BFGS (Quasi-Newton): Approximates the Hessian iteratively to reduce computational cost.
