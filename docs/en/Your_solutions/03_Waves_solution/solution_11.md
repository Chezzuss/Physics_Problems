# Task 11 – Animation of Two-Slit Interference

## Problem Statement

Construct an HTML animation of Young's double-slit experiment in which two slits act as coherent point sources. The displacement field is

$$
u(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r_1}|} \sin(k |\vec{r} - \vec{r_1}| - \omega t) + \frac{A}{|\vec{r}-\vec{r_2}|} \sin(k |\vec{r} - \vec{r_2}| - \omega t)
$$

The user must be able to adjust the slit separation

$$
d = |\vec{r_1} - \vec{r_2}|
$$

and the wavelength $\lambda$. The animation must visualize the interference pattern in real time.

## Theory

In Young's double-slit experiment, the two slits behave as coherent point sources with the same frequency and phase. The resulting displacement is the sum of the contributions from both slits.

For the two sources located at $\vec{r_1}$ and $\vec{r_2}$, the total field is

$$
u(\vec{r},t) = u_1(\vec{r},t) + u_2(\vec{r},t)
$$

where

$$
u_1(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r_1}|} \sin(k |\vec{r} - \vec{r_1}| - \omega t)
$$

and

$$
u_2(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r_2}|} \sin(k |\vec{r} - \vec{r_2}| - \omega t)
$$

The wave number is related to the wavelength by

$$
k = \frac{2\pi}{\lambda}
$$

Constructive interference occurs when the path difference is an integer multiple of the wavelength, while destructive interference occurs when the path difference is a half-integer multiple of the wavelength.

## Step-by-Step Solution

### Geometric configuration

The two slits are placed symmetrically with respect to the horizontal axis. If the slit separation is $d$, their positions may be written as

$$
\vec{r_1} = (x_0, y_0 - d/2)
$$

$$
\vec{r_2} = (x_0, y_0 + d/2)
$$

### Superposition of waves

At each point of the observation region, the distances to the two slits are computed. The displacement is obtained by summing the two partial waves.

### Adjustable parameters

The animation allows real-time control of:

- slit separation $d$
- wavelength $\lambda$
- angular frequency $\omega$
- amplitude $A$

### Numerical visualization

The interference pattern is rendered on a two-dimensional canvas. For each pixel, the displacement is evaluated and mapped to a color scale.

## Final Result

The simulation is implemented in a separate HTML file:

`task_11_animation.html`

## Interpretation

If the slit separation increases, the interference fringes become more closely spaced. If the wavelength increases, the fringes spread farther apart. The simulation makes these dependencies visible in real time.
