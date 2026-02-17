<!DOCTYPE html>
<html>
<head>
  <title>Ramadan Greeting - HALA</title>
  <style>
    body { 
      text-align: center; 
      font-family: Arial; 
    }

    #card {
      position: relative;
      display: inline-block;
      margin-top: 20px;
    }

    #nameText {
      position: absolute;
      bottom: 120px;
      width: 100%;
      font-size: 28px;
      font-weight: bold;
      color: #333;
    }
  </style>
</head>
<body>

<h2>Ramadan Greeting Generator</h2>

<input type="text" id="username" placeholder="Enter your name">
<button onclick="generateCard()">Generate</button>

<div id="card">

  <!-- ✅ Your new image link -->
  <img src="https://i.ibb.co/93N0TKDR/IMG-9980-1.jpg" width="600">

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
