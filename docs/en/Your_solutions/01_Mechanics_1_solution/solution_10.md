# Task 10 – Kinematics of a Point in Three Dimensions

## Problem Statement

Point $M$ moves according to

$$
\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), bt)
$$

where $a$, $b$, and $\omega$ are positive constants.

Determine:

a) the equation of the trajectory,

b) the path length from $t=0$ to $t=t_0$,

c) a Python script for plotting the trajectory and discuss special cases.

## Theory

The position vector in three-dimensional space is

$$
\vec{r}(t) = (x(t), y(t), z(t))
$$

The trajectory is found by eliminating the parameter $t$ from the coordinate equations.

The path length from $t=0$ to $t=t_0$ is

$$
s = \int_0^{t_0} |\vec{v}(t)|\,dt
$$

where

$$
\vec{v}(t) = \frac{d\vec{r}}{dt}
$$

and

$$
|\vec{v}(t)| = \sqrt{\left(\frac{dx}{dt}\right)^2 + \left(\frac{dy}{dt}\right)^2 + \left(\frac{dz}{dt}\right)^2}
$$

## Step-by-Step Solution

### 1. Write the coordinate functions

From

$$
\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), bt)
$$

the coordinates are

$$
x(t) = a \cos(\omega t)
$$

$$
y(t) = b \sin(\omega t)
$$

$$
z(t) = bt
$$

---

### 2. Determine the trajectory equation in the $xy$-plane

Using the trigonometric identity

$$
\cos^2(\omega t) + \sin^2(\omega t) = 1
$$

we obtain

$$
\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = 1
$$

Thus, the projection onto the $xy$-plane is an ellipse.

Since

$$
z = bt
$$

the point rises linearly with time while moving around the ellipse. Therefore the full spatial trajectory is an elliptical helix.

It can also be written parametrically in terms of $z$ by substituting

$$
t = \frac{z}{b}
$$

which gives

$$
x = a \cos\left(\frac{\omega z}{b}\right)
$$

$$
y = b \sin\left(\frac{\omega z}{b}\right)
$$

$$
\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = 1
$$

with $z$ increasing linearly.

---

### 3. Compute the velocity vector

Differentiate each coordinate:

$$
\frac{dx}{dt} = -a\omega \sin(\omega t)
$$

$$
\frac{dy}{dt} = b\omega \cos(\omega t)
$$

$$
\frac{dz}{dt} = b
$$

Hence,

$$
\vec{v}(t) = \left(-a\omega \sin(\omega t),\; b\omega \cos(\omega t),\; b\right)
$$

---

### 4. Compute the speed

The speed is

$$
|\vec{v}(t)| = \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2}
$$

This is the general expression.

Therefore the path length from $0$ to $t_0$ is

$$
s = \int_0^{t_0} \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2}\,dt
$$

This integral is the exact arc-length formula for the trajectory.

---

### 5. Simplify in the special case $a=b$

If $a=b$, then the projection in the $xy$-plane is a circle of radius $a$, and the trajectory becomes a circular helix.

The speed becomes

$$
|\vec{v}(t)| = \sqrt{a^2\omega^2 \sin^2(\omega t) + a^2\omega^2 \cos^2(\omega t) + a^2}
$$

Using

$$
\sin^2(\omega t) + \cos^2(\omega t) = 1
$$

we obtain

$$
|\vec{v}(t)| = \sqrt{a^2\omega^2 + a^2}
$$

$$
|\vec{v}(t)| = a\sqrt{\omega^2 + 1}
$$

which is constant.

Thus, in this special case the path length is

$$
s = a\sqrt{\omega^2 + 1}\, t_0
$$

---

### 6. Python script for plotting the trajectory

The following script plots the curve in three dimensions.

## Final Result

The trajectory is an elliptical helix with projection

$$
\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = 1
$$

and vertical coordinate

$$
z = bt
$$

The velocity vector is

$$
\vec{v}(t) = \left(-a\omega \sin(\omega t),\; b\omega \cos(\omega t),\; b\right)
$$

The path length from $0$ to $t_0$ is

$$
s = \int_0^{t_0} \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2}\,dt
$$

In the special case $a=b$,

$$
s = a\sqrt{\omega^2 + 1}\, t_0
$$

## Interpretation

The point combines two types of motion:

- periodic motion in the horizontal plane,
- uniform upward motion in the vertical direction.

This produces a helical curve.

Special cases:

- If $a=b$, the helix is circular.
- If $a \neq b$, the helix is elliptical.
- If $\omega$ increases, the point winds around the axis more rapidly.
- If $b$ increases, the vertical rise becomes steeper.

## Python Plot Script

python
import numpy as np
import matplotlib.pyplot as plt

a = 3.0
b = 2.0
omega = 1.5
t0 = 10.0

t = np.linspace(0, t0, 1000)

x = a * np.cos(omega * t)
y = b * np.sin(omega * t)
z = b * t

fig = plt.figure(figsize=(8, 6))
ax = fig.add_subplot(111, projection='3d')

ax.plot(x, y, z, linewidth=2)

ax.set_xlabel('x')
ax.set_ylabel('y')
ax.set_zlabel('z')
ax.set_title('Elliptical Helix')

plt.show()
