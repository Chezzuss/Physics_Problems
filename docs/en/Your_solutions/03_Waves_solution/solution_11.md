<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Double Slit Interference</title>
<style>
  body { margin: 0; background: black; }
  canvas { display: block; }
</style>
</head>
<body>

<canvas id="c"></canvas>

<script>
const canvas = document.getElementById("c");
const ctx = canvas.getContext("2d");

canvas.width = window.innerWidth;
canvas.height = window.innerHeight;

let d = 50;      // расстояние между щелями
let lambda = 20; // длина волны
let t = 0;

function draw() {
  const w = canvas.width;
  const h = canvas.height;

  const img = ctx.createImageData(w, h);

  for (let x = 0; x < w; x++) {
    for (let y = 0; y < h; y++) {

      // позиции щелей
      let r1 = Math.hypot(x - w/2, y - (h/2 - d/2));
      let r2 = Math.hypot(x - w/2, y - (h/2 + d/2));

      let k = 2 * Math.PI / lambda;

      let u = Math.sin(k * r1 - t) + Math.sin(k * r2 - t);

      let intensity = (u*u) * 255;

      let i = (y * w + x) * 4;
      img.data[i] = intensity;
      img.data[i+1] = intensity;
      img.data[i+2] = intensity;
      img.data[i+3] = 255;
    }
  }

  ctx.putImageData(img, 0, 0);
  t += 0.1;

  requestAnimationFrame(draw);
}

draw();
</script>

</body>
</html>
