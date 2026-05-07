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

The magnetic force acting on a moving charged particle is given by

$$
\vec{F} = q\vec{v} \times \vec{B}
$$

where:

- $q$ is the electric charge,
- $\vec{v}$ is the velocity vector,
- $\vec{B}$ is the magnetic field vector.

For a proton,

$$
q = 1.602 \times 10^{-19} \ \mathrm{C}
$$

The magnitude of the magnetic force is

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

Compute the cross product using the component formula:

$$
\vec{v} \times \vec{B}
=
\bigl(
v_yB_z - v_zB_y,\ 
v_zB_x - v_xB_z,\ 
v_xB_y - v_yB_x
\bigr)
$$

Substitute the vector components:

$$
\vec{v} \times \vec{B}
=
\bigl(
(-4)(-1) - (1)(2),\
(1)(1) - (2)(-1),\
(2)(2) - (-4)(1)
\bigr)
$$

Simplify:

$$
\vec{v} \times \vec{B}
=
(2,\ 3,\ 8)
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

The proton experiences a very small magnetic force because the proton charge is extremely small. Since the proton has positive charge, the force direction is the same as the direction of

$$
\vec{v} \times \vec{B}
$$
