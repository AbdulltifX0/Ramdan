
<html>
<head>
  <title>Ramadan Greeting - HALA</title>

  <style>
    body {
      text-align: center;
      font-family: Arial;
      background: #f5f5f5;
    }

    #card {
      position: relative;
      display: inline-block;
      margin-top: 20px;
    }

    #card img {
      max-width: 900px;
      width: 100%;
      height: auto;
    }

    #nameText {
      position: absolute;
      bottom: 120px;   /* Adjust if needed */
      width: 100%;
      font-size: 32px;
      font-weight: bold;
      color: #333;
      text-transform: capitalize;
    }
  </style>
</head>

<body>

<h2>Ramadan Greeting Generator</h2>

<input type="text" id="username" placeholder="Enter your name">
<button onclick="generateCard()">Generate</button>

<div id="card">

  <!-- ✅ Your new direct image link -->
  <img src="https://i.postimg.cc/523dpf2h/IMG-9980-(1).jpg">

  <div id="nameText"></div>
</div>

<script>
function generateCard() {
  var name = document.getElementById("username").value;
  document.getElementById("nameText").innerText = name;
}
</script>

</body>
</html>
