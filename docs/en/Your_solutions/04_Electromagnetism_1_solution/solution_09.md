# Task 09 – Vector Lorentz Force

## Problem Statement

A proton moves with velocity

$$
\vec{v} = (2\hat{i} - 4\hat{j} + \hat{k}) \ \mathrm{m/s}
$$

in a magnetic field

$$
\vec{B} = (\hat{i} + 2\hat{j} - \hat{k}) \ \mathrm{T}
$$

Find the magnitude of the magnetic force on the proton.

## Theory

The magnetic force acting on a moving charged particle is given by the Lorentz force equation:

$$
\vec{F} = q\vec{v} \times \vec{B}
$$

where:

- $\vec{F}$ is the magnetic force,
- $q$ is the electric charge,
- $\vec{v}$ is the velocity vector,
- $\vec{B}$ is the magnetic field vector.

For a proton,

$$
q = 1.602 \times 10^{-19} \ \mathrm{C}
$$

The magnitude of the force is

$$
F = q|\vec{v} \times \vec{B}|
$$

## Step-by-Step Solution

The vectors are

$$
\vec{v} = (2, -4, 1)
$$

and

$$
\vec{B} = (1, 2, -1)
$$

Compute the cross product using the determinant form:

$$
\vec{v} \times \vec{B}
=
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & -4 & 1 \\
1 & 2 & -1
\end{vmatrix}
$$

Expand the determinant:

$$
\vec{v} \times \vec{B}
=
\hat{i}[(-4)(-1) - (1)(2)]
-
\hat{j}[(2)(-1) - (1)(1)]
+
\hat{k}[(2)(2) - (-4)(1)]
$$

Simplify each component:

$$
\vec{v} \times \vec{B}
=
\hat{i}(4 - 2)
-
\hat{j}(-2 - 1)
+
\hat{k}(4 + 4)
$$

$$
\vec{v} \times \vec{B}
=
2\hat{i} + 3\hat{j} + 8\hat{k}
$$

Find the magnitude of this vector:

$$
|\vec{v} \times \vec{B}|
=
\sqrt{2^2 + 3^2 + 8^2}
$$

$$
|\vec{v} \times \vec{B}|
=
\sqrt{4 + 9 + 64}
$$

$$
|\vec{v} \times \vec{B}|
=
\sqrt{77}
$$

$$
|\vec{v} \times \vec{B}|
\approx 8.775
$$

Now calculate the magnetic force magnitude:

$$
F = q|\vec{v} \times \vec{B}|
$$

Substitute the values:

$$
F = (1.602 \times 10^{-19})(8.775)
$$

$$
F \approx 1.41 \times 10^{-18} \ \mathrm{N}
$$

## Final Result

$$
F \approx 1.41 \times 10^{-18} \ \mathrm{N}
$$

## Interpretation

The proton experiences a very small magnetic force because the proton charge is extremely small. Since the proton has positive charge, the force direction is the same as the direction of the vector product

$$
\vec{v} \times \vec{B}
$$
