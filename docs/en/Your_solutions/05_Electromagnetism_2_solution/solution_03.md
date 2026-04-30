# Task 03 – Biot-Savart Law

## Problem Statement

A small segment of a line wire of length $0.1 \ \mathrm{m}$ carries a current of $3 \ \mathrm{A}$. The segment is located at a distance of $0.2 \ \mathrm{m}$ from a point $P$. Calculate the magnetic field at point $P$ due to this current segment. Assume the segment is perpendicular to the line connecting it to point $P$.

## Theory

For a short current element, the Biot-Savart law gives the approximate magnetic field:

$$
B = \frac{\mu_0}{4 \pi} \frac{I \Delta l \sin \theta}{r^2}
$$

where:

- $B$ is the magnetic field,
- $\mu_0 = 4 \pi \times 10^{-7} \ \mathrm{T \cdot m/A}$,
- $I$ is the current,
- $\Delta l$ is the wire segment length,
- $r$ is the distance from the segment to the point,
- $\theta$ is the angle between the current element and the line joining the segment to the point.

Since the segment is perpendicular to the line connecting it to point $P$,

$$
\theta = 90^\circ
$$

and therefore

$$
\sin \theta = 1
$$

## Step-by-Step Solution

The given values are

$$
I = 3 \ \mathrm{A}
$$

$$
\Delta l = 0.1 \ \mathrm{m}
$$

$$
r = 0.2 \ \mathrm{m}
$$

Using the Biot-Savart law,

$$
B = \frac{\mu_0}{4 \pi} \frac{I \Delta l \sin \theta}{r^2}
$$

Since

$$
\frac{\mu_0}{4 \pi} = 10^{-7} \ \mathrm{T \cdot m/A}
$$

the field becomes

$$
B = 10^{-7} \frac{(3)(0.1)(1)}{(0.2)^2}
$$

Calculate the denominator:

$$
(0.2)^2 = 0.04
$$

Then

$$
B = 10^{-7} \frac{0.3}{0.04}
$$

$$
B = 10^{-7}(7.5)
$$

$$
B = 7.5 \times 10^{-7} \ \mathrm{T}
$$

## Final Result

$$
B = 7.5 \times 10^{-7} \ \mathrm{T}
$$

## Interpretation

The magnetic field is small because it is produced by only a short segment of wire. Its direction is perpendicular to both the current element and the line from the segment to point $P$, according to the right-hand rule.
