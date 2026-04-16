<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Young Double-Slit Interference</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
      background: #f4f4f4;
      color: #222;
    }

    h1 {
      margin-bottom: 12px;
    }

    .panel {
      background: white;
      padding: 16px;
      border-radius: 10px;
      margin-bottom: 16px;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
      max-width: 900px;
    }

    .row {
      margin: 10px 0;
    }

    label {
      display: inline-block;
      min-width: 180px;
    }

    canvas {
      border: 1px solid #ccc;
      background: black;
      image-rendering: pixelated;
      max-width: 100%;
      height: auto;
      display: block;
    }

    .note {
      font-size: 14px;
      color: #444;
      margin-top: 10px;
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
      <label for="lambdaSlider">Wavelength λ</label>
      <input id="lambdaSlider" type="range" min="10" max="120" step="1" value="35">
      <span id="lambdaValue">35</span>
    </div>

    <div class="row">
      <label for="omegaSlider">Angular frequency ω</label>
      <input id="omegaSlider" type="range" min="0.5" max="12" step="0.1" value="5">
      <span id="omegaValue">5.0</span>
    </div>

    <div class="row">
      <label for="ampSlider">Amplitude A</label>
      <input id="ampSlider" type="range" min="0.2" max="4" step="0.1" value="1.2">
      <span id="ampValue">1.2</span>
    </div>

    <p class="note">
      Open this file directly in a browser, or use a VS Code extension such as Live Server.
    </p>
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
      omegaValue.textContent = Number(omegaSlider.value).toFixed(1);
      ampValue.textContent = Number(ampSlider.value).toFixed(1);
    }

    [dSlider, lambdaSlider, omegaSlider, ampSlider].forEach(el => {
      el.addEventListener("input", updateLabels);
    });

    function clamp(value, min, max) {
      return Math.max(min, Math.min(max, value));
    }

    function draw() {
      const d = Number(dSlider.value);
      const lambda = Number(lambdaSlider.value);
      const omega = Number(omegaSlider.value);
      const A = Number(ampSlider.value);

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

          let dist1 = Math.hypot(x - r1.x, y - r1.y);
          let dist2 = Math.hypot(x - r2.x, y - r2.y);

          dist1 = Math.max(dist1, 1.0);
          dist2 = Math.max(dist2, 1.0);

          const u =
            (A / dist1) * Math.sin(k * dist1 - omega * time) +
            (A / dist2) * Math.sin(k * dist2 - omega * time);

          const scaled = clamp(Math.round(127 + 220 * u), 0, 255);
          const idx = 4 * (j * w + i);

          img.data[idx] = scaled;
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
