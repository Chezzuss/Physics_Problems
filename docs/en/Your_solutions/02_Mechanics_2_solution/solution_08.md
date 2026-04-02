# Task 08 – Work of a Variable Force

## Problem Statement

Given the one-dimensional force

$$
F(x) = -kx
$$

determine:

- the equation of motion and its solution,
- the work done during displacement from $0$ to $x_0$,
- the interpretation of the result as potential energy,
- the verification of the relation $F = -\frac{dU}{dx}$,
- the qualitative graphs of $F(x)$ and $U(x)$.

## Theory

A force of the form

$$
F(x) = -kx
$$

is Hooke's law for an ideal spring. The negative sign indicates that the force is restoring: it always points toward the equilibrium position $x=0$.

Newton's second law gives

$$
m\frac{d^2x}{dt^2} = -kx
$$

which is the differential equation of simple harmonic motion.

The work done by a variable force from $x=a$ to $x=b$ is

$$
W = \int_a^b F(x)\,dx
$$

For conservative forces, a potential energy function $U(x)$ exists such that

$$
F(x) = -\frac{dU}{dx}
$$

## Step-by-Step Solution

### 1. Equation of motion

Using Newton's second law,

$$
m\frac{d^2x}{dt^2} = -kx
$$

Rearrange:

$$
\frac{d^2x}{dt^2} + \frac{k}{m}x = 0
$$

Define

$$
\omega = \sqrt{\frac{k}{m}}
$$

Then the equation becomes

$$
\frac{d^2x}{dt^2} + \omega^2 x = 0
$$

This is the standard equation of simple harmonic motion.

---

### 2. General solution of the equation of motion

The general solution is

$$
x(t) = A \cos(\omega t) + B \sin(\omega t)
$$

Equivalently, it can be written as

$$
x(t) = C \cos(\omega t + \phi)
$$

where $A$, $B$, or equivalently $C$, $\phi$ are constants determined by initial conditions.

---

### 3. Work done from $0$ to $x_0$

The work is

$$
W = \int_0^{x_0} (-kx)\,dx
$$

Take out the constant $-k$:

$$
W = -k \int_0^{x_0} x\,dx
$$

$$
W = -k \left[\frac{x^2}{2}\right]_0^{x_0}
$$

$$
W = -k \left(\frac{x_0^2}{2} - 0\right)
$$

$$
W = -\frac{1}{2}k x_0^2
$$

---

### 4. Interpret the result as potential energy

For a conservative force,

$$
W_{0 \to x_0} = -(U(x_0)-U(0))
$$

Choose the reference value

$$
U(0)=0
$$

Then

$$
-\frac{1}{2}k x_0^2 = -U(x_0)
$$

Hence

$$
U(x_0) = \frac{1}{2}k x_0^2
$$

Therefore the potential energy function is

$$
U(x) = \frac{1}{2}k x^2
$$

---

### 5. Verify the relation $F = -\frac{dU}{dx}$

Differentiate the potential energy:

$$
\frac{dU}{dx} = \frac{d}{dx}\left(\frac{1}{2}k x^2\right)
$$

$$
\frac{dU}{dx} = kx
$$

Therefore,

$$
-\frac{dU}{dx} = -kx
$$

which is exactly the given force:

$$
F(x) = -kx
$$

Thus the relation is verified.

---

### 6. Graphs of $F(x)$ and $U(x)$

The force function is

$$
F(x) = -kx
$$

This is a straight line through the origin with negative slope $-k$.

The potential energy is

$$
U(x) = \frac{1}{2}k x^2
$$

This is an upward-opening parabola with minimum at $x=0$.

## Final Result

The equation of motion is

$$
m\frac{d^2x}{dt^2} = -kx
$$

or equivalently

$$
\frac{d^2x}{dt^2} + \frac{k}{m}x = 0
$$

Its general solution is

$$
x(t) = A \cos\left(\sqrt{\frac{k}{m}}\,t\right) + B \sin\left(\sqrt{\frac{k}{m}}\,t\right)
$$

The work done from $0$ to $x_0$ is

$$
W = -\frac{1}{2}k x_0^2
$$

The corresponding potential energy is

$$
U(x) = \frac{1}{2}k x^2
$$

and it satisfies

$$
F(x) = -\frac{dU}{dx}
$$

## Interpretation

The force always acts toward equilibrium, so the motion is oscillatory.

The work done by the spring during a displacement away from equilibrium is negative because the force opposes the motion. The stored potential energy increases quadratically with displacement, which is characteristic of an ideal spring.
