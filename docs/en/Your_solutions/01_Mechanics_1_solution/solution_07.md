# Task 07 – Elimination of Time and Interpretation of Acceleration

## Problem Statement

The path equation is given in parametric form:

$$
x(t)=2t^2, \qquad y(t)=3t^3
$$

Determine:

- the Cartesian equation obtained by eliminating the parameter $t$,
- the trajectory,
- $\vec v(t)$, $|\vec v(t)|$, $\vec a(t)$, and $|\vec a(t)|$,
- whether the acceleration is constant.

## Theory

For parametric motion in the plane,

$$
\vec{r}(t) = x(t)\hat{i} + y(t)\hat{j}
$$

The velocity and acceleration vectors are

$$
\vec{v}(t) = \frac{d\vec{r}}{dt}
$$

$$
\vec{a}(t) = \frac{d\vec{v}}{dt}
$$

Their magnitudes are

$$
|\vec{v}(t)| = \sqrt{v_x^2 + v_y^2}
$$

$$
|\vec{a}(t)| = \sqrt{a_x^2 + a_y^2}
$$

To eliminate the parameter, one variable is expressed in terms of the other using the parametric equations.

## Step-by-Step Solution

### 1. Eliminate the parameter $t$

From

$$
x = 2t^2
$$

it follows that

$$
t^2 = \frac{x}{2}
$$

From

$$
y = 3t^3
$$

square both sides to avoid the sign ambiguity in $t$:

$$
y^2 = 9t^6
$$

Since

$$
t^6 = (t^2)^3
$$

we obtain

$$
t^6 = \left(\frac{x}{2}\right)^3
$$

Therefore,

$$
y^2 = 9 \left(\frac{x}{2}\right)^3
$$

$$
y^2 = \frac{9}{8}x^3
$$

This is the Cartesian equation of the trajectory.

---

### 2. Describe the trajectory

Since

$$
x = 2t^2 \geq 0
$$

the motion is restricted to the half-plane $x \geq 0$.

The Cartesian equation

$$
y^2 = \frac{9}{8}x^3
$$

describes a semicubical parabola.

Because $y = 3t^3$:

- for $t>0$, the point lies above the $x$-axis,
- for $t<0$, the point lies below the $x$-axis,
- at $t=0$, the point passes through the origin.

Thus the trajectory has two symmetric branches with respect to the $x$-axis.

---

### 3. Compute the velocity vector

The position vector is

$$
\vec{r}(t) = 2t^2\,\hat{i} + 3t^3\,\hat{j}
$$

Differentiate componentwise:

$$
\vec{v}(t) = \frac{d}{dt}(2t^2)\,\hat{i} + \frac{d}{dt}(3t^3)\,\hat{j}
$$

$$
\vec{v}(t) = 4t\,\hat{i} + 9t^2\,\hat{j}
$$

---

### 4. Compute the speed

The speed is the magnitude of velocity:

$$
|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2}
$$

$$
|\vec{v}(t)| = \sqrt{16t^2 + 81t^4}
$$

Factor $t^2$:

$$
|\vec{v}(t)| = \sqrt{t^2(16 + 81t^2)}
$$

$$
|\vec{v}(t)| = |t|\sqrt{16 + 81t^2}
$$

---

### 5. Compute the acceleration vector

Differentiate the velocity vector:

$$
\vec{a}(t) = \frac{d}{dt}(4t)\,\hat{i} + \frac{d}{dt}(9t^2)\,\hat{j}
$$

$$
\vec{a}(t) = 4\,\hat{i} + 18t\,\hat{j}
$$

---

### 6. Compute the magnitude of acceleration

$$
|\vec{a}(t)| = \sqrt{4^2 + (18t)^2}
$$

$$
|\vec{a}(t)| = \sqrt{16 + 324t^2}
$$

---

### 7. Determine whether the acceleration is constant

A constant acceleration vector must have constant components.

Here,

$$
\vec{a}(t) = 4\,\hat{i} + 18t\,\hat{j}
$$

The $x$-component is constant, but the $y$-component depends on time.

Therefore the acceleration vector is not constant.

Also, its magnitude

$$
|\vec{a}(t)| = \sqrt{16 + 324t^2}
$$

depends on time, so the size of the acceleration also changes.

## Final Result

The Cartesian equation of the trajectory is

$$
y^2 = \frac{9}{8}x^3
$$

The velocity vector is

$$
\vec{v}(t) = 4t\,\hat{i} + 9t^2\,\hat{j}
$$

The speed is

$$
|\vec{v}(t)| = |t|\sqrt{16 + 81t^2}
$$

The acceleration vector is

$$
\vec{a}(t) = 4\,\hat{i} + 18t\,\hat{j}
$$

The magnitude of acceleration is

$$
|\vec{a}(t)| = \sqrt{16 + 324t^2}
$$

The acceleration is not constant.

## Interpretation

The motion follows a curved path that starts at the origin and opens to the right.

The velocity changes in both direction and magnitude. The acceleration also changes with time because the vertical component increases linearly with $t$.

This is a clear example of non-uniform two-dimensional motion with non-constant acceleration.
