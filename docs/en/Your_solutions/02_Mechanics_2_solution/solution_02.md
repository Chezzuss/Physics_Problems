# Task 02 – Harmonic Motion of a Mass-Spring System

## Problem Statement

A $10 \text{ kg}$ mass is attached to a spring and oscillates according to

$$
x(t) = 0.2 \cos(10\pi t)
$$

where $x$ is measured in meters.

Determine:

- the spring constant $k$,
- the total mechanical energy of the system.

## Theory

For simple harmonic motion of a mass-spring system,

$$
x(t) = A \cos(\omega t + \phi)
$$

where:

- $A$ is the amplitude,
- $\omega$ is the angular frequency.

For an ideal spring-mass oscillator, the angular frequency satisfies

$$
\omega = \sqrt{\frac{k}{m}}
$$

Therefore,

$$
k = m\omega^2
$$

The total mechanical energy of the oscillator is constant and equals

$$
E = \frac{1}{2}kA^2
$$

## Step-by-Step Solution

### 1. Identify amplitude and angular frequency

Compare the given equation

$$
x(t) = 0.2 \cos(10\pi t)
$$

with the standard form

$$
x(t) = A \cos(\omega t)
$$

Thus,

$$
A = 0.2 \text{ m}
$$

$$
\omega = 10\pi \text{ rad/s}
$$

---

### 2. Calculate the spring constant

Use

$$
k = m\omega^2
$$

Substitute $m = 10 \text{ kg}$ and $\omega = 10\pi$:

$$
k = 10(10\pi)^2
$$

$$
k = 10 \cdot 100\pi^2
$$

$$
k = 1000\pi^2 \text{ N/m}
$$

Numerically,

$$
k \approx 1000 \cdot 9.8696 \approx 9869.6 \text{ N/m}
$$

---

### 3. Calculate the total mechanical energy

Use

$$
E = \frac{1}{2}kA^2
$$

Substitute $k = 1000\pi^2$ and $A=0.2$:

$$
E = \frac{1}{2}(1000\pi^2)(0.2)^2
$$

$$
E = \frac{1}{2}(1000\pi^2)(0.04)
$$

$$
E = 20\pi^2 \text{ J}
$$

Numerically,

$$
E \approx 20 \cdot 9.8696 \approx 197.4 \text{ J}
$$

## Final Result

The spring constant is

$$
k = 1000\pi^2 \text{ N/m} \approx 9869.6 \text{ N/m}
$$

The total mechanical energy is

$$
E = 20\pi^2 \text{ J} \approx 197.4 \text{ J}
$$

## Interpretation

The system performs ideal harmonic motion with fixed amplitude and constant total energy.

A large angular frequency implies a stiff spring, which is consistent with the large value of $k$. The mechanical energy remains constant because no damping or friction is present.
