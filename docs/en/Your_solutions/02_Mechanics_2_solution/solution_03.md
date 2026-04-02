# Task 03 – Conservation of Energy in a Pendulum

## Problem Statement

A pendulum of length $1.0 \text{ m}$ is released from an initial angle of $15^\circ$.

Determine the speed of the pendulum bob at the bottom of its swing.

## Theory

If air resistance and friction are neglected, the mechanical energy is conserved.

At the release point, the pendulum has gravitational potential energy relative to the lowest point. At the bottom, this potential energy is converted into kinetic energy.

Thus,

$$
mgh = \frac{1}{2}mv^2
$$

The vertical height difference between the initial position and the bottom is

$$
h = L - L\cos\theta = L(1-\cos\theta)
$$

## Step-by-Step Solution

### 1. Determine the vertical drop

Given:

$$
L = 1.0 \text{ m}
$$

$$
\theta = 15^\circ
$$

Use

$$
h = L(1-\cos\theta)
$$

Substitute:

$$
h = 1.0(1-\cos 15^\circ)
$$

Using

$$
\cos 15^\circ \approx 0.9659
$$

we obtain

$$
h \approx 1 - 0.9659 = 0.0341 \text{ m}
$$

---

### 2. Apply conservation of energy

At the top:

$$
E = mgh
$$

At the bottom:

$$
E = \frac{1}{2}mv^2
$$

Equate the two:

$$
mgh = \frac{1}{2}mv^2
$$

Cancel the mass:

$$
gh = \frac{1}{2}v^2
$$

Solve for $v$:

$$
v = \sqrt{2gh}
$$

Substitute values:

$$
v = \sqrt{2 \cdot 9.81 \cdot 0.0341}
$$

$$
v \approx \sqrt{0.669} \approx 0.818 \text{ m/s}
$$

## Final Result

The speed of the pendulum bob at the bottom is approximately

$$
v \approx 0.82 \text{ m/s}
$$

## Interpretation

The bob starts from rest and accelerates downward due to gravity. The larger the release angle, the greater the vertical drop and therefore the greater the speed at the bottom.

For a relatively small angle of $15^\circ$, the speed remains modest because the loss of height is small.
