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

The magnetic part of the Lorentz force is

$$
\vec{F} = q\vec{v} \times \vec{B}
$$

where:

- $\vec{F}$ is the magnetic force,
- $q$ is the charge,
- $\vec{v}$ is the velocity,
- $\vec{B}$ is the magnetic field.

For a proton,

$$
q = e = 1.602 \times 10^{-19} \ \mathrm{C}
$$

The magnitude of the force is

$$
F = q|\vec{v} \times \vec{B}|
$$

## Step-by-Step Solution

The cross product is

$$
\vec{v} \times \vec{B}
=
\begin{pmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & -4 & 1 \\
1 & 2 & -1
\end{pmatrix}
$$

Calculate each component:

$$
\vec{v} \times \vec{B}
=
\hat{i}[(-4)(-1) - (1)(2)]
-
\hat{j}[(2)(-1) - (1)(1)]
+
\hat{k}[(2)(2) - (-4)(1)]
$$

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

The magnitude is

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

Now calculate the force magnitude:

$$
F = q|\vec{v} \times \vec{B}|
$$

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

The proton experiences a very small magnetic force because the charge of a proton is very small. The force direction is along $\vec{v} \times \vec{B}$ because the proton has positive charge.
