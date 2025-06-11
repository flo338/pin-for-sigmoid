# Physics-Informed Neural Networks (PINN)

This project demonstrates by a small example how neural networks can be guided by physical laws to solve differential equations.

## Problem Overview

We solve the logistic differential equation:

$$
\frac{df}{dt} = f(t)(1 - f(t)), \quad \text{with the known solution} \quad f(t) = \frac{1}{1 + e^{-t}}
$$

This equation models logistic growth, and the goal is to recover the solution with only two samples giving the start end end point of the interval we are paying attention to.

## Outcome

Through symbolic regression, we can eventually express the function in closed form, successfully recovering the original equation from the neural network's approximation
