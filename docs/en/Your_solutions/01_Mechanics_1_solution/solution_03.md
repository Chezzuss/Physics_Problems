# Task 03 – Path Intersection

## Problem Statement

Alice moves along:

$$
A(t) = (2+t, 8-3t)
$$

Bob moves along:

$$
B(t) = (2t-1, 2t+2)
$$

Determine whether their paths intersect. If yes, find when and where. If not, determine the minimum distance and when it occurs.

## Theory

Two objects collide if their position vectors are equal at the same time:

$$
A(t) = B(t)
$$

This leads to a system of equations.

If no solution exists, the distance between them is minimized by minimizing:

$$
D(t)^2 = (x_A - x_B)^2 + (y_A - y_B)^2
$$

## Step-by-Step Solution

### 1. Set coordinates equal

$$
2 + t = 2t - 1
$$

$$
8 - 3t = 2t + 2
$$

---

### 2. Solve first equation

$$
2 + t = 2t - 1
$$

$$
2 + 1 = 2t - t
$$

$$
t = 3
$$

---

### 3. Check second equation

Substitute $t=3$:

$$
8 - 3(3) = 8 - 9 = -1
$$

$$
2(3) + 2 = 8
$$

Since $-1 \neq 8$, no intersection occurs.

---

### 4. Distance between paths

Coordinates difference:

$$
x_A - x_B = (2+t) - (2t-1) = 3 - t
$$

$$
y_A - y_B = (8-3t) - (2t+2) = 6 - 5t
$$

Distance squared:

$$
D^2 = (3 - t)^2 + (6 - 5t)^2
$$

---

### 5. Minimize distance

Expand:

$$
D^2 = (3 - t)^2 + (6 - 5t)^2
$$

$$
= (9 - 6t + t^2) + (36 - 60t + 25t^2)
$$

$$
= 45 - 66t + 26t^2
$$

Differentiate:

$$
\frac{d}{dt}D^2 = -66 + 52t
$$

Set to zero:

$$
52t = 66
$$

$$
t = \frac{33}{26}
$$

---

### 6. Minimum distance

Substitute $t = \frac{33}{26}$:

$$
D_{min}^2 = 45 - 66\cdot\frac{33}{26} + 26\cdot\left(\frac{33}{26}\right)^2
$$

Simplifies to:

$$
D_{min}^2 = \frac{351}{26}
$$

$$
D_{min} = \sqrt{\frac{351}{26}} \approx 3.67
$$

## Final Result

- No intersection occurs
- Minimum distance:

$$
D_{min} \approx 3.67
$$

- Occurs at:

$$
t = \frac{33}{26}
$$

## Interpretation

The paths do not intersect because both coordinate equations cannot be satisfied simultaneously.

The motion is linear, so the distance function is quadratic in time, ensuring a unique minimum.
