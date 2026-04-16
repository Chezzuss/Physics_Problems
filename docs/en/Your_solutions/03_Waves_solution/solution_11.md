
FILE: `task_11.md`
```markdown
# Task 11 – Animation of Two-Slit Interference

## Problem Statement

Construct an HTML animation of Young's double-slit experiment in which two slits act as coherent point sources. The displacement field is

$$
u(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r_1}|} \sin(k |\vec{r} - \vec{r_1}| - \omega t) + \frac{A}{|\vec{r}-\vec{r_2}|} \sin(k |\vec{r} - \vec{r_2}| - \omega t)
$$

The user must be able to adjust the slit separation

$$
d = |\vec{r_1} - \vec{r_2}|
$$

and the wavelength $\lambda$. The animation must visualize the interference pattern in real time.

## Theory

In Young's experiment, the two slits behave as coherent sources emitting waves of the same frequency and phase. The total disturbance is the sum of the disturbances from each slit:

$$
u(\vec{r},t) = u_1(\vec{r},t) + u_2(\vec{r},t)
$$

with

$$
u_1(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r_1}|} \sin(k |\vec{r} - \vec{r_1}| - \omega t)
$$

and

$$
u_2(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r_2}|} \sin(k |\vec{r} - \vec{r_2}| - \omega t)
$$

The wave number is

$$
k = \frac{2\pi}{\lambda}
$$

Constructive interference occurs where the path difference is an integer multiple of the wavelength, while destructive interference occurs where the path difference is a half-integer multiple.

## Step-by-Step Solution

### 1. Geometry of the slits

The slits are placed symmetrically with respect to the center:

$$
\vec{r_1} = (x_0, y_0 - d/2)
$$

$$
\vec{r_2} = (x_0, y_0 + d/2)
$$

### 2. Superposition

For every point in the observation region, compute the distances to both slits, evaluate the two wave contributions, and add them.

### 3. Adjustable parameters

The user must be able to change:

- slit distance $d$
- wavelength $\lambda$

This changes the fringe spacing and overall interference geometry.

### 4. Real-time rendering

The field is recomputed at each animation frame for the current values of the parameters.

## Final Result

The following HTML file implements the Young's double-slit interference simulation.

## Interpretation

When the slit separation increases, the interference fringes become more closely spaced. When the wavelength increases, the fringes spread farther apart.

## HTML Source

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Young Double-Slit Interference</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
      background: #f4f4f4;
    }
    .panel {
      background: white;
      padding: 16px;
      border-radius: 10px;
      margin-bottom: 16px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.08);
    }
    .row {
      margin: 10px 0;
    }
    label {
      display: inline-block;
      min-width: 160px;
    }
    canvas {
      border: 1px solid #ccc;
      background: black;
      image-rendering: pixelated;
    }
  </style>
</head>
<body>
  <h1>Young's Two-Slit Interference</h1>

  <div class="panel">
    <div class="row">
      <label for="dSlider">Slit separation d</label>
      <input id="dSlider" type="range" min="10" max="180" step="1" value="60">
      <span id="dValue">60</span>
    </div>

    <div class="row">
      <label for="lambdaSlider">Wavelength</label>
      <input id="lambdaSlider" type="range" min="10" max="120" step="1" value="35">
      <span id="lambdaValue">35</span>
    </div>

    <div class="row">
      <label for="omegaSlider">Angular frequency</label>
      <input id="omegaSlider" type="range" min="0.5" max="12" step="0.1" value="5">
      <span id="omegaValue">5.0</span>
    </div>

    <div class="row">
      <label for="ampSlider">Amplitude</label>
      <input id="ampSlider" type="range" min="0.2" max="4" step="0.1" value="1.2">
      <span id="ampValue">1.2</span>
    </div>
  </div>

  <div class="panel">
    <canvas id="canvas" width="760" height="460"></canvas>
  </div>

  <script>
    const canvas = document.getElementById("canvas");
    const ctx = canvas.getContext("2d");

    const dSlider = document.getElementById("dSlider");
    const dValue = document.getElementById("dValue");
    const lambdaSlider = document.getElementById("lambdaSlider");
    const lambdaValue = document.getElementById("lambdaValue");
    const omegaSlider = document.getElementById("omegaSlider");
    const omegaValue = document.getElementById("omegaValue");
    const ampSlider = document.getElementById("ampSlider");
    const ampValue = document.getElementById("ampValue");

    const width = canvas.width;
    const height = canvas.height;

    const lowRes = document.createElement("canvas");
    lowRes.width = 190;
    lowRes.height = 115;
    const lowCtx = lowRes.getContext("2d");

    let time = 0;

    function updateLabels() {
      dValue.textContent = dSlider.value;
      lambdaValue.textContent = lambdaSlider.value;
      omegaValue.textContent = parseFloat(omegaSlider.value).toFixed(1);
      ampValue.textContent = parseFloat(ampSlider.value).toFixed(1);
    }

    [dSlider, lambdaSlider, omegaSlider, ampSlider].forEach(el => {
      el.addEventListener("input", updateLabels);
    });

    function clamp(v, min, max) {
      return Math.max(min, Math.min(max, v));
    }

    function draw() {
      const d = parseFloat(dSlider.value);
      const lambda = parseFloat(lambdaSlider.value);
      const omega = parseFloat(omegaSlider.value);
      const A = parseFloat(ampSlider.value);

      const k = 2 * Math.PI / lambda;

      const x0 = 120;
      const y0 = height / 2;

      const r1 = { x: x0, y: y0 - d / 2 };
      const r2 = { x: x0, y: y0 + d / 2 };

      const w = lowRes.width;
      const h = lowRes.height;
      const img = lowCtx.createImageData(w, h);

      for (let j = 0; j < h; j++) {
        for (let i = 0; i < w; i++) {
          const x = i * width / w;
          const y = j * height / h;

          let d1 = Math.hypot(x - r1.x, y - r1.y);
          let d2 = Math.hypot(x - r2.x, y - r2.y);

          d1 = Math.max(d1, 1.0);
          d2 = Math.max(d2, 1.0);

          const u =
            (A / d1) * Math.sin(k * d1 - omega * time) +
            (A / d2) * Math.sin(k * d2 - omega * time);

          const scaled = clamp(Math.round(127 + 220 * u), 0, 255);
          const idx = 4 * (j * w + i);

          img.data[idx + 0] = scaled;
          img.data[idx + 1] = scaled;
          img.data[idx + 2] = 255 - scaled;
          img.data[idx + 3] = 255;
        }
      }

      lowCtx.putImageData(img, 0, 0);

      ctx.clearRect(0, 0, width, height);
      ctx.imageSmoothingEnabled = false;
      ctx.drawImage(lowRes, 0, 0, width, height);

      ctx.strokeStyle = "white";
      ctx.lineWidth = 2;
      ctx.beginPath();
      ctx.moveTo(x0, 0);
      ctx.lineTo(x0, height);
      ctx.stroke();

      ctx.fillStyle = "white";
      ctx.beginPath();
      ctx.arc(r1.x, r1.y, 5, 0, 2 * Math.PI);
      ctx.fill();

      ctx.beginPath();
      ctx.arc(r2.x, r2.y, 5, 0, 2 * Math.PI);
      ctx.fill();

      time += 0.05;
      requestAnimationFrame(draw);
    }

    updateLabels();
    draw();
  </script>
</body>
</html>
