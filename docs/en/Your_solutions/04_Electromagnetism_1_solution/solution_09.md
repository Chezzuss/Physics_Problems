# Task 09 – Vector Lorentz Force

## Problem Statement

A proton moves with a velocity vector $\vec{v} = (2\hat{i} - 4\hat{j} + \hat{k})$ m/s in a region containing a uniform magnetic field described by the vector $\vec{B} = (\hat{i} + 2\hat{j} - \hat{k})$ T. Determine the magnitude of the magnetic force experienced by the proton.

## Theory

The magnetic force exerted on a moving charge is determined by the magnetic component of the Lorentz force equation. The force vector is the cross product of the velocity vector and the magnetic field vector, scaled by the electric charge of the particle.

$$
\vec{F}_B = q (\vec{v} \times \vec{B})
$$

The cross product of two vectors in a three-dimensional Cartesian coordinate system can be computed using the determinant of a matrix containing the unit vectors and the components of the two vectors.

$$
\vec{v} \times \vec{B} = \det
\begin{pmatrix}
\hat{i} & \hat{j} & \hat{k} \\
v_x & v_y & v_z \\
B_x & B_y & B_z
\end{pmatrix}
$$

The magnitude of the resulting force vector is calculated using the Euclidean norm.

$$
|\vec{F}_B| = \sqrt{F_x^2 + F_y^2 + F_z^2}
$$

## Step-by-Step Solution

The elementary charge of a proton is a standard physical constant.

$$
q = 1.60 \times 10^{-19} \text{ C}
$$

First, construct the matrix to compute the cross product of the velocity vector and the magnetic field vector.

$$
\vec{v} \times \vec{B} = \det
\begin{pmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & -4 & 1 \\
1 & 2 & -1
\end{pmatrix}
$$

Expand the determinant along the first row to find the Cartesian components of the resulting vector.

$$
\begin{align}
\vec{v} \times \vec{B} &= \hat{i} [(-4)(-1) - (1)(2)] - \hat{j} [(2)(-1) - (1)(1)] + \hat{k} [(2)(2) - (-4)(1)] \\
                       &= \hat{i} (4 - 2) - \hat{j} (-2 - 1) + \hat{k} (4 + 4) \\
                       &= 2\hat{i} + 3\hat{j} + 8\hat{k}
\end{align}
$$

Compute the magnitude of the cross product vector.

$$
|\vec{v} \times \vec{B}| = \sqrt{2^2 + 3^2 + 8^2}
$$

$$
|\vec{v} \times \vec{B}| = \sqrt{4 + 9 + 64}
$$

$$
|\vec{v} \times \vec{B}| = \sqrt{77} \approx 8.775 \text{ m}\cdot\text{T/s}
$$

Multiply the magnitude of the cross product by the charge of the proton to obtain the magnitude of the magnetic force.

$$
|\vec{F}_B| = q |\vec{v} \times \vec{B}|
$$

$$
|\vec{F}_B| = (1.60 \times 10^{-19} \text{ C}) \times \sqrt{77}
$$

$$
|\vec{F}_B| \approx 1.40 \times 10^{-18} \text{ N}
$$

## Final Result

The magnitude of the magnetic force experienced by the proton is approximately $1.40 \times 10^{-18} \text{ N}$.

## Interpretation

The cross product dictates that the resulting magnetic force vector is completely orthogonal to both the proton's velocity vector and the external magnetic field. The calculation confirms that despite the three-dimensional complexity of the particle's trajectory relative to the field, the force strictly depends on the perpendicular components of the velocity and the field, yielding a relatively small absolute force typical for subatomic particles.
