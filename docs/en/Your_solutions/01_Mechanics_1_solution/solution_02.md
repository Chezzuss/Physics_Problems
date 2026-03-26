# Task 02 – Range Optimization

## Problem Statement

For projectile motion, show analytically that the maximum range

$$
R(\theta)=\frac{v_0^2 \sin(2\theta)}{g}
$$

for a given initial velocity is achieved at a launch angle of $45^\circ$.

## Theory

The horizontal range of a projectile (neglecting air resistance) is given by

$$
R(\theta)=\frac{v_0^2 \sin(2\theta)}{g}
$$

The maximum value of the range depends on maximizing the function $\sin(2\theta)$.

Key trigonometric property:

$$
-1 \leq \sin(x) \leq 1
$$

Maximum value:

$$
\sin(x) = 1 \quad \text{when} \quad x = \frac{\pi}{2}
$$

## Step-by-Step Solution

### 1. Expression for range

$$
R(\theta)=\frac{v_0^2}{g}\sin(2\theta)
$$

The factor $\frac{v_0^2}{g}$ is constant.

Maximizing $R(\theta)$ reduces to maximizing $\sin(2\theta)$.

---

### 2. Maximization condition

Maximum occurs when:

$$
\sin(2\theta) = 1
$$

Thus:

$$
2\theta = \frac{\pi}{2}
$$

---

### 3. Solve for angle

$$
\theta = \frac{\pi}{4}
$$

Convert to degrees:

$$
\theta = 45^\circ
$$

---

### 4. Alternative method (derivative)

Differentiate $R(\theta)$:

$$
\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta)
$$

Set derivative equal to zero:

$$
\cos(2\theta) = 0
$$

$$
2\theta = \frac{\pi}{2}
$$

$$
\theta = \frac{\pi}{4}
$$

Second derivative:

$$
\frac{d^2R}{d\theta^2} = -\frac{v_0^2}{g} \cdot 4\sin(2\theta)
$$

At $\theta=\frac{\pi}{4}$:

$$
\sin(2\theta)=1 \Rightarrow \frac{d^2R}{d\theta^2} < 0
$$

This confirms a maximum.

## Final Result

$$
\theta = 45^\circ
$$

## Interpretation

The optimal launch angle is independent of the initial velocity.

This result follows from the symmetry of projectile motion:

- Increasing angle increases flight time
- Decreasing angle increases horizontal velocity

The balance occurs at $45^\circ$, where these effects combine to maximize the range.
