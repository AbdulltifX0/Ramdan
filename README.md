<html>
<head>
  <title>Ramadan Greeting - HALA</title>

  <style>
    body {
      text-align: center;
      font-family: Arial;
      background: #f5f5f5;
    }

    canvas {
      margin-top: 20px;
      max-width: 90%;
    }

    input {
      padding: 10px;
      font-size: 16px;
      text-align: center;
    }

    button {
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
      margin: 5px;
    }
  </style>
</head>

<body>

<h2>Ramadan Greeting Generator</h2>

<input type="text" id="username" placeholder="Enter your name">
<br><br>

<button onclick="generateCard()">Generate</button>
<button onclick="downloadImage()">Download</button>

<br>

<canvas id="cardCanvas"></canvas>

<script>
const canvas = document.getElementById("cardCanvas");
const ctx = canvas.getContext("2d");

const img = new Image();
img.crossOrigin = "anonymous"; // important for download

img.src = "https://i.postimg.cc/523dpf2h/IMG-9980-(1).jpg";

img.onload = function() {
  canvas.width = img.width;
  canvas.height = img.height;
  ctx.drawImage(img, 0, 0);
};

function generateCard() {

  const name = document.getElementById("username").value;

  // redraw image first
  ctx.drawImage(img, 0, 0);

  // text style
  ctx.font = "bold 35px Arial";
  ctx.fillStyle = "#333";
  ctx.textAlign = "center";

  // position (adjust if needed)
  ctx.fillText(name, canvas.width / 2, canvas.height - 100);
}

function downloadImage() {
  const link = document.createElement("a");
  link.download = "Ramadan-Greeting.png";
  link.href = canvas.toDataURL("image/png");
  link.click();
}
</script>

</body>
</html>
