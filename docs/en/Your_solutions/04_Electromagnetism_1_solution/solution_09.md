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

The magnetic force on a moving charge is

$$
\vec{F} = q\vec{v} \times \vec{B}
$$

For a proton,

$$
q = 1.602 \times 10^{-19} \ \mathrm{C}
$$

The magnitude of the force is

$$
F = q|\vec{v} \times \vec{B}|
$$

## Step-by-Step Solution

First calculate the cross product:

$$
\vec{v} \times \vec{B}
=
\begin{pmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & -4 & 1 \\
1 & 2 & -1
\end{pmatrix}
$$

Using the component formula,

$$
\vec{v} \times \vec{B}
=
(v_yB_z - v_zB_y)\hat{i}
+
(v_zB_x - v_xB_z)\hat{j}
+
(v_xB_y - v_yB_x)\hat{k}
$$

Substitute the components:

$$
\vec{v} \times \vec{B}
=
[(-4)(-1) - (1)(2)]\hat{i}
+
[(1)(1) - (2)(-1)]\hat{j}
+
[(2)(2) - (-4)(1)]\hat{k}
$$

$$
\vec{v} \times \vec{B}
=
2\hat{i} + 3\hat{j} + 8\hat{k}
$$

Find its magnitude:

$$
|\vec{v} \times \vec{B}|
=
\sqrt{2^2 + 3^2 + 8^2}
$$

$$
|\vec{v} \times \vec{B}|
=
\sqrt{77}
\approx 8.775
$$

Now calculate the force:

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

The proton experiences a very small magnetic force because its charge is very small. Since the proton is positively charged, the force direction is the same as the direction of $\vec{v} \times \vec{B}$.
