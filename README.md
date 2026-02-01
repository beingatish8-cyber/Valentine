<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Valentine Invitation 💖</title>
  <style>
    body {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff758c, #ff7eb3);
      font-family: 'Segoe UI', sans-serif;
      overflow: hidden;
    }

    .card {
      background: white;
      padding: 30px 40px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 15px 30px rgba(0,0,0,0.2);
    }

    h1 {
      color: #ff4d6d;
      margin-bottom: 20px;
    }

    button {
      padding: 12px 25px;
      font-size: 16px;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      margin: 10px;
    }

    #yes {
      background: #ff4d6d;
      color: white;
    }

    #no {
      background: #ccc;
      position: absolute;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Will you be my Valentine? 💕</h1>
    <button id="yes" onclick="yesClicked()">Yes 💖</button>
    <button id="no" onmouseover="moveNo()">No 😅</button>
  </div>

  <script>
    function yesClicked() {
      document.body.innerHTML = `
        <div style="text-align:center; color:white;">
          <h1>Yayyy! 💘🥰</h1>
          <h2>Best Valentine ever 💖</h2>
        </div>
      `;
    }

    function moveNo() {
      const noBtn = document.getElementById("no");
      const x = Math.random() * (window.innerWidth - 100);
      const y = Math.random() * (window.innerHeight - 50);
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    }
  </script>

</body>
</html># Valentine
