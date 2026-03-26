# Task 06 – Variable Velocity

## Problem Statement

An object's velocity is given by

$$
v(t) = t^2 + 2t - 5
$$

If the object was at $x=4$ at $t=0$, determine its position and acceleration at time $t=3$.

## Theory

Velocity is the derivative of position:

$$
v(t) = \frac{dx}{dt}
$$

Therefore the position is obtained by integrating the velocity:

$$
x(t) = \int v(t)\,dt + C
$$

The constant $C$ is found from the initial condition.

Acceleration is the derivative of velocity:

$$
a(t) = \frac{dv}{dt}
$$

## Step-by-Step Solution

### 1. Integrate the velocity function

Given

$$
v(t) = t^2 + 2t - 5
$$

Integrate term by term:

$$
x(t) = \int (t^2 + 2t - 5)\,dt
$$

$$
x(t) = \frac{t^3}{3} + t^2 - 5t + C
$$

---

### 2. Use the initial condition

The object is at $x=4$ when $t=0$:

$$
x(0) = 4
$$

Substitute into the position function:

$$
4 = \frac{0^3}{3} + 0^2 - 5 \cdot 0 + C
$$

$$
C = 4
$$

Thus,

$$
x(t) = \frac{t^3}{3} + t^2 - 5t + 4
$$

---

### 3. Evaluate the position at $t=3$

Substitute $t=3$:

$$
x(3) = \frac{3^3}{3} + 3^2 - 5 \cdot 3 + 4
$$

$$
x(3) = \frac{27}{3} + 9 - 15 + 4
$$

$$
x(3) = 9 + 9 - 15 + 4
$$

$$
x(3) = 7
$$

---

### 4. Differentiate velocity to obtain acceleration

$$
a(t) = \frac{d}{dt}(t^2 + 2t - 5)
$$

$$
a(t) = 2t + 2
$$

Evaluate at $t=3$:

$$
a(3) = 2 \cdot 3 + 2 = 8
$$

## Final Result

The position function is

$$
x(t) = \frac{t^3}{3} + t^2 - 5t + 4
$$

At time $t=3$,

$$
x(3) = 7
$$

and

$$
a(3) = 8
$$

## Interpretation

The velocity is not constant, so the motion is accelerated.

At $t=3$:

- the object is located at position $x=7$,
- the acceleration is positive, meaning the velocity is increasing at that instant.
