# Task 06 – EM Wave Analysis

## Problem Statement

An electromagnetic wave has its electric field component described by

$$
E_y(x,t) = 100 \sin(10^7 x - \omega t) \ \mathrm{V/m}
$$

Determine:

1. The direction of propagation.
2. The wavelength $\lambda$.
3. The angular frequency $\omega$.
4. The equation for the magnetic field component.

## Theory

A sinusoidal wave traveling in the positive $x$-direction has the form

$$
E_y(x,t) = E_0 \sin(kx - \omega t)
$$

where:

- $E_0$ is the electric field amplitude,
- $k$ is the wave number,
- $\omega$ is the angular frequency.

The wave number is related to wavelength by

$$
k = \frac{2\pi}{\lambda}
$$

For an electromagnetic wave in vacuum,

$$
c = \frac{\omega}{k}
$$

so

$$
\omega = ck
$$

The electric and magnetic field amplitudes are related by

$$
B_0 = \frac{E_0}{c}
$$

For a wave moving in the $+x$ direction with electric field in the $+y$ direction, the magnetic field points in the $+z$ direction.

## Step-by-Step Solution

The given electric field is

$$
E_y(x,t) = 100 \sin(10^7 x - \omega t)
$$

Comparing with the standard form,

$$
E_y(x,t) = E_0 \sin(kx - \omega t)
$$

gives

$$
E_0 = 100 \ \mathrm{V/m}
$$

and

$$
k = 10^7 \ \mathrm{rad/m}
$$

### Direction of Propagation

The phase has the form

$$
kx - \omega t
$$

This corresponds to propagation in the positive $x$-direction.

### Wavelength

Using

$$
k = \frac{2\pi}{\lambda}
$$

solve for $\lambda$:

$$
\lambda = \frac{2\pi}{k}
$$

Substitute the value of $k$:

$$
\lambda = \frac{2\pi}{10^7}
$$

$$
\lambda = 6.28 \times 10^{-7} \ \mathrm{m}
$$

### Angular Frequency

Using

$$
\omega = ck
$$

with

$$
c = 3.00 \times 10^8 \ \mathrm{m/s}
$$

substitute:

$$
\omega = (3.00 \times 10^8)(10^7)
$$

$$
\omega = 3.00 \times 10^{15} \ \mathrm{rad/s}
$$

### Magnetic Field Component

The magnetic field amplitude is

$$
B_0 = \frac{E_0}{c}
$$

Substitute:

$$
B_0 = \frac{100}{3.00 \times 10^8}
$$

$$
B_0 = 3.33 \times 10^{-7} \ \mathrm{T}
$$

The magnetic field is in the $z$-direction, so

$$
B_z(x,t) = 3.33 \times 10^{-7} \sin(10^7 x - 3.00 \times 10^{15}t) \ \mathrm{T}
$$

## Final Result

The wave propagates in the positive $x$-direction.

$$
\lambda = 6.28 \times 10^{-7} \ \mathrm{m}
$$

$$
\omega = 3.00 \times 10^{15} \ \mathrm{rad/s}
$$

$$
B_z(x,t) = 3.33 \times 10^{-7} \sin(10^7 x - 3.00 \times 10^{15}t) \ \mathrm{T}
$$

## Interpretation

The electric field oscillates in the $y$-direction, the magnetic field oscillates in the $z$-direction, and the wave travels in the $+x$ direction. These three directions are mutually perpendicular, as required for an electromagnetic wave.
