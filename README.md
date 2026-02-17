<html>
<head>
  <title>Ramadan Greeting - HALA</title>

  <style>
    body {
      text-align: center;
      font-family: Arial;
      background-color: #f5f5f5;
    }

    h2 {
      margin-top: 20px;
    }

    input {
      padding: 10px;
      font-size: 16px;
      width: 200px;
      text-align: center;
    }

    button {
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
    }

    #card {
      position: relative;
      display: inline-block;
      margin-top: 25px;
    }

    #card img {
      width: 600px;   /* keep high quality */
      height: auto;
    }

    /* 🔽 Name position (lowered) */
    #nameText {
      position: absolute;
      bottom: 300px;     /* move down here */
      width: 100%;
      font-size: 32px;
      font-weight: bold;
      color: #333;
      text-align: center;
      letter-spacing: 1px;
    }
  </style>
</head>

<body>

<h2>Ramadan Greeting Generator</h2>

<input type="text" id="username" placeholder="Enter your name">
<button onclick="generateCard()">Generate</button>

<div id="card">

  <!-- ✅ Your direct image link -->
  <img src="https://i.postimg.cc/523dpf2h/IMG-9980-(1).jpg" alt="Ramadan Card">

  <div id="nameText"></div>
</div>

<script>
function generateCard() {
  var name = document.getElementById("username").value;

  if(name.trim() === ""){
    alert("Please enter your name");
    return;
  }

  document.getElementById("nameText").innerText = name;
}
</script>

</body>
</html>
