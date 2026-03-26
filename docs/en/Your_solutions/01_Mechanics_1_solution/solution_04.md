# Task 04 – Velocity and Acceleration Vectors

## Problem Statement

The position of an object is given by

$$
\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}
$$

Find the object's velocity and acceleration vectors as a function of time.

## Theory

In planar motion, the position vector can be written as

$$
\vec{r}(t) = x(t)\hat{i} + y(t)\hat{j}
$$

The velocity vector is the first derivative of position with respect to time:

$$
\vec{v}(t) = \frac{d\vec{r}}{dt}
$$

The acceleration vector is the derivative of velocity, or equivalently the second derivative of position:

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = \frac{d^2\vec{r}}{dt^2}
$$

The derivatives are taken componentwise.

## Step-by-Step Solution

### 1. Identify coordinate functions

From the given position vector,

$$
x(t) = 3t^2
$$

$$
y(t) = 5t - 8t^2
$$

---

### 2. Differentiate to obtain the velocity vector

Differentiate each component with respect to time:

$$
v_x(t) = \frac{dx}{dt} = \frac{d}{dt}(3t^2) = 6t
$$

$$
v_y(t) = \frac{dy}{dt} = \frac{d}{dt}(5t - 8t^2) = 5 - 16t
$$

Therefore,

$$
\vec{v}(t) = 6t\,\hat{i} + (5 - 16t)\,\hat{j}
$$

---

### 3. Differentiate again to obtain the acceleration vector

Differentiate the velocity components:

$$
a_x(t) = \frac{dv_x}{dt} = \frac{d}{dt}(6t) = 6
$$

$$
a_y(t) = \frac{dv_y}{dt} = \frac{d}{dt}(5 - 16t) = -16
$$

Therefore,

$$
\vec{a}(t) = 6\,\hat{i} - 16\,\hat{j}
$$

## Final Result

The velocity vector is

$$
\vec{v}(t) = 6t\,\hat{i} + (5 - 16t)\,\hat{j}
$$

The acceleration vector is

$$
\vec{a}(t) = 6\,\hat{i} - 16\,\hat{j}
$$

## Interpretation

The motion is non-uniform because the velocity depends on time.

The acceleration is constant, which means that:

- the object accelerates steadily in the positive $x$-direction,
- the object accelerates steadily in the negative $y$-direction.

Thus, the motion is a two-dimensional analogue of constant-acceleration kinematics.
