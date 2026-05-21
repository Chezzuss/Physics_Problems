# Task 02 – Resistors

## Problem Statement

A supply of exactly three resistors is given. Each resistor has resistance

$$
R = 1 \ \Omega
$$

Determine all possible unique equivalent resistances that can be obtained by combining the three resistors.

## Theory

Resistors can be connected in two fundamental ways:

- series connection,
- parallel connection.

For resistors in series, the equivalent resistance is the sum:

$$
R_{\mathrm{eq}} = R_1 + R_2 + R_3
$$

For resistors in parallel, the reciprocal formula is used:

$$
\frac{1}{R_{\mathrm{eq}}}
=
\frac{1}{R_1}
+
\frac{1}{R_2}
+
\frac{1}{R_3}
$$

Mixed series-parallel combinations are also possible.

Since all resistors are identical,

$$
R = 1 \ \Omega
$$

the calculations become simpler.

## Step-by-Step Solution

All unique configurations using exactly three resistors are considered.

### 1. All Resistors in Series

The equivalent resistance is

$$
R_{\mathrm{eq}} = 1 + 1 + 1
$$

Therefore,

$$
R_{\mathrm{eq}} = 3 \ \Omega
$$

### 2. All Resistors in Parallel

Use the parallel formula:

$$
\frac{1}{R_{\mathrm{eq}}}
=
1 + 1 + 1
$$

Thus,

$$
\frac{1}{R_{\mathrm{eq}}} = 3
$$

Therefore,

$$
R_{\mathrm{eq}} = \frac{1}{3} \ \Omega
$$

### 3. Two Resistors in Series, Then in Parallel with the Third

First combine two resistors in series:

$$
R_s = 1 + 1 = 2 \ \Omega
$$

Now place this combination in parallel with the remaining resistor:

$$
\frac{1}{R_{\mathrm{eq}}}
=
\frac{1}{2}
+
\frac{1}{1}
$$

Simplify:

$$
\frac{1}{R_{\mathrm{eq}}}
=
\frac{1}{2}
+
\frac{2}{2}
=
\frac{3}{2}
$$

Therefore,

$$
R_{\mathrm{eq}} = \frac{2}{3} \ \Omega
$$

### 4. Two Resistors in Parallel, Then in Series with the Third

First combine two resistors in parallel:

$$
\frac{1}{R_p}
=
1 + 1
$$

Thus,

$$
\frac{1}{R_p} = 2
$$

Therefore,

$$
R_p = \frac{1}{2} \ \Omega
$$

Now connect this result in series with the remaining resistor:

$$
R_{\mathrm{eq}}
=
\frac{1}{2} + 1
$$

Therefore,

$$
R_{\mathrm{eq}} = \frac{3}{2} \ \Omega
$$

## Final Result

The unique equivalent resistances obtainable using exactly three identical $1 \ \Omega$ resistors are:

$$
\frac{1}{3} \ \Omega
$$

$$
\frac{2}{3} \ \Omega
$$

$$
\frac{3}{2} \ \Omega
$$

$$
3 \ \Omega
$$

## Interpretation

The smallest equivalent resistance occurs when all resistors are connected in parallel because multiple current paths reduce resistance.

The largest equivalent resistance occurs when all resistors are connected in series because resistances add directly.

Mixed configurations produce intermediate values between these two extremes.
