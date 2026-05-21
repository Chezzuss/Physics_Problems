# Task 02 – Resistors

## Problem Statement

A supply of exactly three resistors is given. Each resistor has resistance

$$
R = 1 \Omega
$$

Determine all possible unique equivalent resistances that can be obtained by combining the three resistors.

## Theory

For resistors in series, resistances add:

$$
R_{\mathrm{eq}} = R_1 + R_2 + R_3
$$

For resistors in parallel, reciprocal resistance values add:

$$
\frac{1}{R_{\mathrm{eq}}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}
$$

Mixed series-parallel combinations are also possible.

## Step-by-Step Solution

### 1. All Resistors in Series

$$
R_{\mathrm{eq}} = 1 + 1 + 1
$$

$$
R_{\mathrm{eq}} = 3 \Omega
$$

### 2. All Resistors in Parallel

$$
\frac{1}{R_{\mathrm{eq}}} = 1 + 1 + 1
$$

$$
\frac{1}{R_{\mathrm{eq}}} = 3
$$

$$
R_{\mathrm{eq}} = \frac{1}{3} \Omega
$$

### 3. Two Resistors in Series, Then in Parallel with the Third

First combine two resistors in series:

$$
R_s = 1 + 1 = 2 \Omega
$$

Then connect this result in parallel with the remaining resistor:

$$
\frac{1}{R_{\mathrm{eq}}} = \frac{1}{2} + \frac{1}{1}
$$

$$
\frac{1}{R_{\mathrm{eq}}} = \frac{3}{2}
$$

$$
R_{\mathrm{eq}} = \frac{2}{3} \Omega
$$

### 4. Two Resistors in Parallel, Then in Series with the Third

First combine two resistors in parallel:

$$
\frac{1}{R_p} = 1 + 1
$$

$$
R_p = \frac{1}{2} \Omega
$$

Then connect this result in series with the remaining resistor:

$$
R_{\mathrm{eq}} = \frac{1}{2} + 1
$$

$$
R_{\mathrm{eq}} = \frac{3}{2} \Omega
$$

## Final Result

The unique equivalent resistances are:

$$
\frac{1}{3} \Omega
$$

$$
\frac{2}{3} \Omega
$$

$$
\frac{3}{2} \Omega
$$

$$
3 \Omega
$$

## Interpretation

The smallest resistance is produced by connecting all three resistors in parallel.

The largest resistance is produced by connecting all three resistors in series.

Mixed combinations give intermediate resistance values.
