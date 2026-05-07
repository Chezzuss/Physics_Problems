# Task 09 – Vector Lorentz Force

## Problem Statement

A proton moves with velocity

$$
\vec{v} = (2\hat{i} - 4\hat{j} + \hat{k}) \ \mathrm{m/s}
$$

in a region where the magnetic field is

$$
\vec{B} = (\hat{i} + 2\hat{j} - \hat{k}) \ \mathrm{T}
$$

Find the magnitude of the magnetic force experienced by the proton.

## Theory

The magnetic force on a moving charged particle is the magnetic part of the Lorentz force:

$$
\vec{F} = q\vec{v} \times \vec{B}
$$

where:

- $\vec{F}$ is the magnetic force,
- $q$ is the electric charge of the particle,
- $\vec{v}$ is the velocity vector,
- $\vec{B}$ is the magnetic field vector,
- $\vec{v} \times \vec{B}$ is the cross product of velocity and magnetic field.

For a proton, the charge is positive:

$$
q = e = 1.602 \times 10^{-19} \ \mathrm{C}
$$

The magnitude of the magnetic force is

$$
F = q|\vec{v} \times \vec{B}|
$$

The cross product is used because the magnetic force depends only on the component of velocity perpendicular to the magnetic field.

## Step-by-Step Solution

The velocity vector is

$$
\vec{v} = 2\hat{i} - 4\hat{j} + \hat{k}
$$

The magnetic field vector is

$$
\vec{B} = \hat{i} + 2\hat{j} - \hat{k}
$$

This means the vector components are

$$
\vec{v} = (2, -4, 1)
$$

and

$$
\vec{B} = (1, 2, -1)
$$

The magnetic force is calculated using

$$
\vec{F} = q\vec{v} \times \vec{B}
$$

First calculate the cross product $\vec{v} \times \vec{B}$.

For two vectors

$$
\vec{a} = (a_x, a_y, a_z)
$$

and

$$
\vec{b} = (b_x, b_y, b_z)
$$

their cross product is

$$
\vec{a} \times \vec{b}
=
(a_y b_z - a_z b_y)\hat{i}
+
(a_z b_x - a_x b_z)\hat{j}
+
(a_x b_y - a_y b_x)\hat{k}
$$

In this problem,

$$
a_x = 2
$$

$$
a_y = -4
$$

$$
a_z = 1
$$

and

$$
b_x = 1
$$

$$
b_y = 2
$$

$$
b_z = -1
$$

The $x$-component of the cross product is

$$
(\vec{v} \times \vec{B})_x = v_y B_z - v_z B_y
$$

$$
(\vec{v} \times \vec{B})_x = (-4)(-1) - (1)(2)
$$

$$
(\vec{v} \times \vec{B})_x = 4 - 2
$$

$$
(\vec{v} \times \vec{B})_x = 2
$$

The $y$-component is

$$
(\vec{v} \times \vec{B})_y = v_z B_x - v_x B_z
$$

$$
(\vec{v} \times \vec{B})_y = (1)(1) - (2)(-1)
$$

$$
(\vec{v} \times \vec{B})_y = 1 + 2
$$

$$
(\vec{v} \times \vec{B})_y = 3
$$

The $z$-component is

$$
(\vec{v} \times \vec{B})_z = v_x B_y - v_y B_x
$$

$$
(\vec{v} \times \vec{B})_z = (2)(2) - (-4)(1)
$$

$$
(\vec{v} \times \vec{B})_z = 4 + 4
$$

$$
(\vec{v} \times \vec{B})_z = 8
$$

Therefore,

$$
\vec{v} \times \vec{B} = 2\hat{i} + 3\hat{j} + 8\hat{k}
$$

The magnitude of this vector is

$$
|\vec{v} \times \vec{B}| =
\sqrt{2^2 + 3^2 + 8^2}
$$

$$
|\vec{v} \times \vec{B}| =
\sqrt{4 + 9 + 64}
$$

$$
|\vec{v} \times \vec{B}| =
\sqrt{77}
$$

$$
|\vec{v} \times \vec{B}| \approx 8.775
$$

Now substitute into the force formula:

$$
F = q|\vec{v} \times \vec{B}|
$$

$$
F = (1.602 \times 10^{-19})(8.775)
$$

$$
F = 1.405 \times 10^{-18} \ \mathrm{N}
$$

Rounding to three significant figures,

$$
F \approx 1.41 \times 10^{-18} \ \mathrm{N}
$$

## Final Result

$$
F \approx 1.41 \times 10^{-18} \ \mathrm{N}
$$

## Interpretation

The force is very small because the proton charge is very small. Since the proton has positive charge, the direction of the force is the same as the direction of $\vec{v} \times \vec{B}$.

The vector $\vec{v} \times \vec{B}$ points in the direction

$$
2\hat{i} + 3\hat{j} + 8\hat{k}
$$

Therefore, the force vector itself would be

$$
\vec{F}
=
(1.602 \times 10^{-19})(2\hat{i} + 3\hat{j} + 8\hat{k})
$$

or

$$
\vec{F}
=
(3.204 \times 10^{-19})\hat{i}
+
(4.806 \times 10^{-19})\hat{j}
+
(1.282 \times 10^{-18})\hat{k}
\ \mathrm{N}
$$

The required answer is the magnitude, so the final scalar result is

$$
F \approx 1.41 \times 10^{-18} \ \mathrm{N}
$$
