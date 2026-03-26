# Task 01 – Projectile Motion

## Problem Statement

A projectile is fired from the ground with an initial velocity of $100 \text{ m/s}$ at an angle of $37^\circ$ above the horizontal. Assume no air resistance.

- Derive the differential equations of motion in the horizontal and vertical directions.
- Determine the time of flight.
- Determine the maximum height.
- Determine the range.

## Theory

Projectile motion without air resistance is governed by constant acceleration:

- Horizontal direction: no acceleration
- Vertical direction: constant acceleration due to gravity

The acceleration vector is

$$
\vec{a} = (0, -g)
$$

Velocity is obtained by integrating acceleration:

$$
\vec{v}(t) = \frac{d\vec{r}}{dt}
$$

Position is obtained by integrating velocity:

$$
\vec{r}(t) = \int \vec{v}(t)\,dt
$$

Initial velocity components:

$$
v_{0x} = v_0 \cos\theta
$$

$$
v_{0y} = v_0 \sin\theta
$$

## Step-by-Step Solution

### 1. Differential equations of motion

Horizontal motion:

$$
\frac{d^2 x}{dt^2} = 0
$$

Vertical motion:

$$
\frac{d^2 y}{dt^2} = -g
$$

---

### 2. Velocity as a function of time

Integrating:

$$
v_x(t) = v_0 \cos\theta
$$

$$
v_y(t) = v_0 \sin\theta - g t
$$

---

### 3. Position as a function of time

Integrating again:

$$
x(t) = v_0 \cos\theta \cdot t
$$

$$
y(t) = v_0 \sin\theta \cdot t - \frac{1}{2} g t^2
$$

---

### 4. Time of flight

The projectile lands when $y(t)=0$:

$$
v_0 \sin\theta \cdot t - \frac{1}{2} g t^2 = 0
$$

Factoring:

$$
t \left( v_0 \sin\theta - \frac{1}{2} g t \right) = 0
$$

Non-zero solution:

$$
t = \frac{2 v_0 \sin\theta}{g}
$$

Substitute values:

$$
t = \frac{2 \cdot 100 \cdot \sin(37^\circ)}{9.81}
$$

Approximation:

$$
\sin(37^\circ) \approx 0.6
$$

$$
t \approx \frac{200 \cdot 0.6}{9.81} \approx 12.2 \text{ s}
$$

---

### 5. Maximum height

At maximum height, vertical velocity is zero:

$$
v_y = 0
$$

$$
v_0 \sin\theta - g t = 0
$$

$$
t_{max} = \frac{v_0 \sin\theta}{g}
$$

Height:

$$
H = v_0 \sin\theta \cdot t_{max} - \frac{1}{2} g t_{max}^2
$$

Simplified formula:

$$
H = \frac{v_0^2 \sin^2\theta}{2g}
$$

Substitute:

$$
H = \frac{100^2 \cdot (0.6)^2}{2 \cdot 9.81}
$$

$$
H \approx \frac{10000 \cdot 0.36}{19.62} \approx 183.5 \text{ m}
$$

---

### 6. Range

Range is horizontal displacement at landing:

$$
R = v_0 \cos\theta \cdot t_{flight}
$$

Using formula:

$$
R = \frac{v_0^2 \sin(2\theta)}{g}
$$

$$
\sin(74^\circ) \approx 0.96
$$

$$
R \approx \frac{10000 \cdot 0.96}{9.81} \approx 978 \text{ m}
$$

## Final Result

- Time of flight: $t \approx 12.2 \text{ s}$
- Maximum height: $H \approx 183.5 \text{ m}$
- Range: $R \approx 978 \text{ m}$

## Interpretation

The motion separates into independent horizontal and vertical components.

- Horizontal motion is uniform.
- Vertical motion is uniformly accelerated.

The symmetry of motion implies:

- Time to reach maximum height is half of total flight time.
- Maximum range depends on $\sin(2\theta)$, not $\sin\theta$.

This forms the foundation for all projectile motion problems.
