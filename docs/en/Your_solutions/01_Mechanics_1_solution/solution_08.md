# Task 08 – Circular Motion

## Problem Statement

Calculate the centripetal acceleration of a person standing on the Earth's equator. The Earth's radius is approximately $6378 \text{ km}$.

## Theory

An object moving in a circle with angular speed $\omega$ experiences centripetal acceleration

$$
a_c = \omega^2 r
$$

An equivalent formula is

$$
a_c = \frac{v^2}{r}
$$

For Earth, one full rotation is completed in approximately

$$
T = 24 \cdot 3600 = 86400 \text{ s}
$$

The angular speed is therefore

$$
\omega = \frac{2\pi}{T}
$$

## Step-by-Step Solution

### 1. Convert the radius to SI units

Given

$$
r = 6378 \text{ km}
$$

Convert to meters:

$$
r = 6.378 \times 10^6 \text{ m}
$$

---

### 2. Compute the angular speed of Earth's rotation

$$
\omega = \frac{2\pi}{86400}
$$

$$
\omega \approx 7.27 \times 10^{-5} \text{ rad/s}
$$

---

### 3. Compute the centripetal acceleration

Use

$$
a_c = \omega^2 r
$$

Substitute values:

$$
a_c = \left(7.27 \times 10^{-5}\right)^2 \cdot 6.378 \times 10^6
$$

$$
a_c \approx 0.0337 \text{ m/s}^2
$$

## Final Result

The centripetal acceleration at the Earth's equator is approximately

$$
a_c \approx 3.37 \times 10^{-2} \text{ m/s}^2
$$

## Interpretation

This acceleration is much smaller than the gravitational acceleration

$$
g \approx 9.81 \text{ m/s}^2
$$

The ratio is approximately

$$
\frac{a_c}{g} \approx 0.0034
$$

Thus the rotational effect of Earth slightly reduces the apparent weight of a person at the equator, but the effect is small compared to gravity.
