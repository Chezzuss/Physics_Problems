# Task 05 – Relative Velocity

## Problem Statement

A river flows east at $2 \text{ m/s}$. A boat that can travel at $5 \text{ m/s}$ in still water wants to go directly north across the river.

Determine:

- the direction in which the boat must head,
- the time required to cross the river if the river is $200 \text{ m}$ wide.

## Theory

Relative velocity describes motion with respect to a moving medium.

Let:

- $\vec{v}_{bw}$ be the velocity of the boat relative to the water,
- $\vec{v}_{wg}$ be the velocity of the water relative to the ground,
- $\vec{v}_{bg}$ be the velocity of the boat relative to the ground.

Then

$$
\vec{v}_{bg} = \vec{v}_{bw} + \vec{v}_{wg}
$$

To move directly north relative to the ground, the boat's east-west component relative to the ground must be zero.

## Step-by-Step Solution

### 1. Choose coordinate axes

Let:

- positive $x$ be east,
- positive $y$ be north.

The river velocity is

$$
\vec{v}_{wg} = (2, 0)
$$

The boat's speed relative to water has magnitude $5 \text{ m/s}$.

The boat must aim somewhat west of north so that its westward component cancels the river's eastward flow.

---

### 2. Determine the required horizontal component

For the boat to move directly north relative to the ground,

$$
v_{bg,x} = 0
$$

Thus,

$$
v_{bw,x} + v_{wg,x} = 0
$$

$$
v_{bw,x} + 2 = 0
$$

$$
v_{bw,x} = -2
$$

So the boat must have a westward component of $2 \text{ m/s}$ relative to the water.

---

### 3. Determine the northward component

Since the magnitude of the boat's velocity relative to the water is $5$,

$$
v_{bw,x}^2 + v_{bw,y}^2 = 5^2
$$

$$
(-2)^2 + v_{bw,y}^2 = 25
$$

$$
4 + v_{bw,y}^2 = 25
$$

$$
v_{bw,y}^2 = 21
$$

$$
v_{bw,y} = \sqrt{21}
$$

Therefore the actual northward speed across the river is

$$
v_{bg,y} = \sqrt{21} \text{ m/s}
$$

since the water has no northward component.

---

### 4. Determine the heading angle

Let $\theta$ be the angle west of north.

Then

$$
\sin\theta = \frac{2}{5}
$$

Hence,

$$
\theta = \sin^{-1}\left(\frac{2}{5}\right)
$$

$$
\theta \approx 23.6^\circ
$$

So the boat must head

$$
23.6^\circ \text{ west of north}
$$

---

### 5. Determine the crossing time

Distance across the river:

$$
d = 200 \text{ m}
$$

Northward speed:

$$
v = \sqrt{21} \text{ m/s}
$$

Time:

$$
t = \frac{d}{v}
$$

$$
t = \frac{200}{\sqrt{21}}
$$

$$
t \approx 43.6 \text{ s}
$$

## Final Result

The boat must head

$$
23.6^\circ \text{ west of north}
$$

The time required to cross the river is

$$
t = \frac{200}{\sqrt{21}} \approx 43.6 \text{ s}
$$

## Interpretation

If the boat pointed exactly north, the river would carry it eastward.

To arrive directly opposite the starting point, the boat must aim upstream. The required westward component exactly cancels the river flow, while the remaining northward component determines the crossing time.
