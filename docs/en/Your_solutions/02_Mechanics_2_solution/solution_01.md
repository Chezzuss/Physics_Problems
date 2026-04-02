# Task 01 – Gravitational Dependence of a Simple Pendulum

## Problem Statement

A simple pendulum has a period of $4 \text{ s}$ on Earth.

Determine:

- its period on the Moon, where the gravitational acceleration is approximately $\frac{1}{6}$ of Earth's,
- the required pendulum length for a period of exactly $1 \text{ s}$ on Earth.

## Theory

For small oscillations, the period of a simple pendulum is

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

where:

- $T$ is the period,
- $L$ is the pendulum length,
- $g$ is the gravitational acceleration.

For a fixed length, the period is proportional to $\frac{1}{\sqrt{g}}$:

$$
T \propto \frac{1}{\sqrt{g}}
$$

Therefore, when gravity decreases, the period increases.

## Step-by-Step Solution

### 1. Period on the Moon

Let:

- $T_E = 4 \text{ s}$ be the period on Earth,
- $g_M = \frac{g_E}{6}$ be the Moon's gravitational acceleration.

Using the proportionality relation,

$$
\frac{T_M}{T_E} = \sqrt{\frac{g_E}{g_M}}
$$

Substitute $g_M = \frac{g_E}{6}$:

$$
\frac{T_M}{4} = \sqrt{\frac{g_E}{g_E/6}}
$$

$$
\frac{T_M}{4} = \sqrt{6}
$$

$$
T_M = 4\sqrt{6}
$$

Numerically,

$$
T_M \approx 4 \cdot 2.449 \approx 9.80 \text{ s}
$$

---

### 2. Required length for a period of $1 \text{ s}$ on Earth

Use the formula

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

Set $T = 1 \text{ s}$:

$$
1 = 2\pi \sqrt{\frac{L}{g}}
$$

Solve for $L$:

$$
\sqrt{\frac{L}{g}} = \frac{1}{2\pi}
$$

$$
\frac{L}{g} = \frac{1}{4\pi^2}
$$

$$
L = \frac{g}{4\pi^2}
$$

Using $g = 9.81 \text{ m/s}^2$:

$$
L = \frac{9.81}{4\pi^2}
$$

$$
L \approx \frac{9.81}{39.478} \approx 0.248 \text{ m}
$$

## Final Result

The pendulum period on the Moon is

$$
T_M = 4\sqrt{6} \approx 9.80 \text{ s}
$$

The required pendulum length for a period of $1 \text{ s}$ on Earth is

$$
L \approx 0.248 \text{ m}
$$

## Interpretation

The pendulum swings more slowly on the Moon because the restoring effect of gravity is weaker.

A pendulum with a period of $1 \text{ s}$ on Earth must be relatively short, about $25 \text{ cm}$. This result is valid under the small-angle approximation.
