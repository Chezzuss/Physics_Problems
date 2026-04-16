# Task 06 – Electric Field from Two Charges

## Problem Statement

Charges:

- $+q$ at $(-a,0)$
- $+2q$ at $(a,0)$

Find $\vec E(x,y)$ and analyze special cases.

## Theory

Electric field from a charge:

$$
\vec E = k \frac{q}{r^3} \vec r
$$

## Step-by-Step Solution

General form:

$$
\vec E = kq \frac{\vec r_1}{r_1^3} + 2kq \frac{\vec r_2}{r_2^3}
$$

where

$$
\vec r_1 = (x+a, y), \quad \vec r_2 = (x-a, y)
$$

### Along y-axis

$$
E_x = kq \left(\frac{a}{r_1^3} - \frac{2a}{r_2^3}\right)
$$

$$
E_y = kq \left(\frac{y}{r_1^3} + \frac{2y}{r_2^3}\right)
$$

## Final Result

Field is vector sum of contributions from both charges.

## Interpretation

Asymmetry of charges produces non-zero field at origin.
