<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Important Question</title>
  <style>
    body {
      height: 100vh;
      background: #ffe6eb;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      font-family: Arial, sans-serif;
      text-align: center;
    }
    h1 { font-size: 28px; padding: 0 15px; }
    .container {
      position: relative;
      width: 260px;
      height: 200px;
      margin-top: 30px;
    }
    button {
      padding: 14px 26px;
      font-size: 18px;
      border: none;
      border-radius: 30px;
      position: absolute;
      cursor: pointer;
    }
    #yes {
      background: #ff4d6d;
      color: white;
      left: 20px;
      top: 80px;
    }
    #no {
      background: #777;
      color: white;
      left: 140px;
      top: 80px;
    }
  </style>
</head>

<body>
  <h1>Atrima, will you be my Valentine? 😌❤️</h1>

  <div class="container">
    <button id="yes">Yes 💕</button>
    <button id="no">No 🙄</button>
  </div>

  <script>
    const noBtn = document.getElementById("no");
    const yesBtn = document.getElementById("yes");

    noBtn.addEventListener("mouseover", () => {
      noBtn.style.left = Math.random() * 160 + "px";
      noBtn.style.top = Math.random() * 120 + "px";
      yesBtn.style.transform = "scale(1.3)";
    });

    yesBtn.onclick = () => {
      document.body.innerHTML =
        "<h1>Good choice 😈❤️</h1><p>You really thought no was an option?</p>";
    };
  </script>
</body>
</html>
