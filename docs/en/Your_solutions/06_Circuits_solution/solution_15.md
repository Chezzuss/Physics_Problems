# Task 15 – Resistor Cube

## Problem Statement

A cube is constructed from 12 identical resistors on its edges. Each resistor has resistance $R$.

Find the equivalent resistance between two opposite corners of the cube.

## Theory

The cube has a high degree of symmetry. When current enters one corner and leaves through the opposite corner, several vertices of the cube must be at the same electric potential.

Vertices that are symmetric with respect to the input and output corners can be grouped together. If two vertices have the same potential, no current flows between them if they are directly connected by a resistor.

For a resistor network, Ohm's law is

$$
V = IR
$$

The equivalent resistance is defined as

$$
R_{\mathrm{eq}} = \frac{V}{I}
$$

where:

- $V$ is the potential difference between the two chosen corners,
- $I$ is the total current entering the network,
- $R_{\mathrm{eq}}$ is the equivalent resistance.

## Step-by-Step Solution

Let the current enter the cube at corner $A$ and leave at the opposite corner $B$.

Because of symmetry, the three vertices connected directly to $A$ are at the same potential. Call this group $C$.

Also, the three vertices connected directly to $B$ are at the same potential. Call this group $D$.

The network can therefore be reduced into three sections.

From $A$ to group $C$, there are three identical resistors $R$ in parallel.

The equivalent resistance of three equal resistors in parallel is

$$
\frac{1}{R_{AC}} = \frac{1}{R} + \frac{1}{R} + \frac{1}{R}
$$

Therefore,

$$
R_{AC} = \frac{R}{3}
$$

Between group $C$ and group $D$, there are six resistors connecting the two groups.

These six resistors are in parallel, so

$$
\frac{1}{R_{CD}} = 6 \cdot \frac{1}{R}
$$

Therefore,

$$
R_{CD} = \frac{R}{6}
$$

From group $D$ to corner $B$, there are again three identical resistors $R$ in parallel.

Thus,

$$
R_{DB} = \frac{R}{3}
$$

The reduced circuit is now a series connection:

$$
R_{\mathrm{eq}} = R_{AC} + R_{CD} + R_{DB}
$$

Substitute the three equivalent resistances:

$$
R_{\mathrm{eq}} = \frac{R}{3} + \frac{R}{6} + \frac{R}{3}
$$

Use a common denominator:

$$
R_{\mathrm{eq}} = \frac{2R}{6} + \frac{R}{6} + \frac{2R}{6}
$$

Therefore,

$$
R_{\mathrm{eq}} = \frac{5R}{6}
$$

## Final Result

The equivalent resistance between two opposite corners of the resistor cube is

$$
R_{\mathrm{eq}} = \frac{5R}{6}
$$

## Interpretation

The equivalent resistance is smaller than $R$ because the current has many possible paths through the cube.

The symmetry of the cube allows groups of vertices to be treated as single points with equal potential. This reduces the complicated three-dimensional resistor network to a simple series combination of three equivalent resistances.
