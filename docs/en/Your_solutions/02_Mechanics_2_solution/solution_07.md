# Task 07 – Dynamics with Friction

## Problem Statement

A $5 \text{ kg}$ block is placed on a $10 \text{ kg}$ block. A horizontal force of $45 \text{ N}$ is applied to the $10 \text{ kg}$ block, and the $5 \text{ kg}$ block is tied to the wall. The coefficient of kinetic friction between all moving surfaces is $0.2$.

Find the acceleration of the $10 \text{ kg}$ block.

## Theory

Because the upper block is tied to the wall, the lower block moves relative to it. Therefore kinetic friction acts between the two blocks.

The lower block also slides over the ground, so kinetic friction acts between the lower block and the floor.

For kinetic friction,

$$
f_k = \mu_k N
$$

Newton's second law for the $10 \text{ kg}$ block is

$$
\sum F_x = ma
$$

## Step-by-Step Solution

### 1. Identify forces acting on the $10 \text{ kg}$ block

The horizontal forces on the lower block are:

- applied force $45 \text{ N}$ to the right,
- friction from the upper block to the left,
- friction from the floor to the left.

Thus the net force is

$$
F_{\text{net}} = 45 - f_{\text{top}} - f_{\text{floor}}
$$

---

### 2. Friction between the $5 \text{ kg}$ block and the $10 \text{ kg}$ block

The normal force between the blocks equals the weight of the upper block:

$$
N_{\text{top}} = 5g
$$

Thus the kinetic friction magnitude is

$$
f_{\text{top}} = \mu_k N_{\text{top}} = 0.2 \cdot 5g
$$

Using $g=9.81$:

$$
f_{\text{top}} = 0.2 \cdot 5 \cdot 9.81 = 9.81 \text{ N}
$$

---

### 3. Friction between the $10 \text{ kg}$ block and the floor

The floor supports both blocks, so the normal force from the floor is

$$
N_{\text{floor}} = (10+5)g = 15g
$$

Therefore,

$$
f_{\text{floor}} = \mu_k N_{\text{floor}} = 0.2 \cdot 15g
$$

$$
f_{\text{floor}} = 0.2 \cdot 15 \cdot 9.81 = 29.43 \text{ N}
$$

---

### 4. Compute the net force

$$
F_{\text{net}} = 45 - 9.81 - 29.43
$$

$$
F_{\text{net}} = 5.76 \text{ N}
$$

---

### 5. Compute the acceleration of the $10 \text{ kg}$ block

Use Newton's second law for the lower block:

$$
a = \frac{F_{\text{net}}}{m}
$$

$$
a = \frac{5.76}{10}
$$

$$
a = 0.576 \text{ m/s}^2
$$

## Final Result

The acceleration of the $10 \text{ kg}$ block is

$$
a \approx 0.58 \text{ m/s}^2
$$

## Interpretation

The applied force is opposed by two friction forces:

- friction with the upper block,
- friction with the floor.

Because the upper block is tied to the wall, sliding necessarily occurs between the blocks, so kinetic friction must be included there. The remaining net force is small, which leads to a relatively small acceleration.
