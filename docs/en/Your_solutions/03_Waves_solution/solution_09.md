# Task 09 – Damped Harmonic Oscillator Interactive Animation

## Problem Statement

Consider the damped harmonic oscillator described by

$$
m \frac{d^2 x}{dt^2} + b \frac{dx}{dt} + kx = 0
$$

Construct an interactive HTML animation with a slider for the damping parameter $b$ in order to visualize the underdamped, critically damped, and overdamped regimes. The animation must include:

1. The general solution
2. The classification of regimes
3. A numerical solution obtained with the RK4 method
4. An investigation of the effect of parameter $b$
5. A graph of $x(t)$
6. A phase portrait

## Theory

The equation of motion is

$$
m \ddot{x} + b \dot{x} + kx = 0
$$

Dividing by $m$ gives

$$
\ddot{x} + \frac{b}{m}\dot{x} + \frac{k}{m}x = 0
$$

Introduce the parameters

$$
\gamma = \frac{b}{2m}
$$

and

$$
\omega_0 = \sqrt{\frac{k}{m}}
$$

Then the equation takes the form

$$
\ddot{x} + 2\gamma \dot{x} + \omega_0^2 x = 0
$$

The characteristic equation is

$$
r^2 + 2\gamma r + \omega_0^2 = 0
$$

Its roots are

$$
r = -\gamma \pm \sqrt{\gamma^2 - \omega_0^2}
$$

## Step-by-Step Solution

### General solution

The type of solution depends on the sign of the discriminant.

#### Underdamped regime

If

$$
\gamma^2 < \omega_0^2
$$

equivalently,

$$
b^2 < 4mk
$$

the roots are complex:

$$
r = -\gamma \pm i\omega_d
$$

where

$$
\omega_d = \sqrt{\omega_0^2 - \gamma^2}
$$

The solution is

$$
x(t) = e^{-\gamma t}\left(C_1 \cos(\omega_d t) + C_2 \sin(\omega_d t)\right)
$$

#### Critically damped regime

If

$$
\gamma^2 = \omega_0^2
$$

equivalently,

$$
b^2 = 4mk
$$

the characteristic equation has a repeated root:

$$
r = -\gamma
$$

The solution is

$$
x(t) = (C_1 + C_2 t)e^{-\gamma t}
$$

#### Overdamped regime

If

$$
\gamma^2 > \omega_0^2
$$

equivalently,

$$
b^2 > 4mk
$$

the roots are real and distinct:

$$
r_{1,2} = -\gamma \pm \sqrt{\gamma^2 - \omega_0^2}
$$

The solution is

$$
x(t) = C_1 e^{r_1 t} + C_2 e^{r_2 t}
$$

### Classification of cases

The critical damping value is

$$
b_c = 2\sqrt{mk}
$$

Therefore:

- underdamped for $b < b_c$
- critically damped for $b = b_c$
- overdamped for $b > b_c$

### Numerical system for RK4

To solve the equation numerically, introduce the velocity

$$
v = \dot{x}
$$

Then the second-order equation becomes the first-order system

$$
\dot{x} = v
$$

$$
\dot{v} = -\frac{b}{m}v - \frac{k}{m}x
$$

This system is suitable for numerical integration with the fourth-order Runge–Kutta method.

### Effect of the damping parameter

The parameter $b$ determines how fast the system loses energy:

- for small $b$, oscillations persist but decay exponentially
- at the critical value, the system returns to equilibrium as fast as possible without oscillation
- for large $b$, the return to equilibrium is slower and non-oscillatory

### Graphical interpretation

The graph of $x(t)$ shows the time evolution of the displacement.

The phase portrait represents the trajectory in the $(x,v)$ plane and shows how the system approaches equilibrium at the origin.

## Final Result

The interactive simulation is implemented in the separate HTML file

`task_09_animation.html`

## Interpretation

The damped harmonic oscillator provides a standard example of how dissipation modifies oscillatory motion. The slider for $b$ makes the transition between underdamped, critically damped, and overdamped motion directly observable.
