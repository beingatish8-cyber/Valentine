<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Valentine for Golu 💖</title>
  <style>
    body {
      height: 100vh;
      margin: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff5f9e, #ffc371);
      font-family: 'Segoe UI', sans-serif;
      overflow: hidden;
    }

    .card {
      background: white;
      padding: 30px 40px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 15px 30px rgba(0,0,0,0.25);
      z-index: 10;
    }

    h1 {
      color: #ff2e63;
      margin-bottom: 20px;
    }

    button {
      padding: 12px 28px;
      font-size: 16px;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      margin: 10px;
    }

    #yes {
      background: #ff2e63;
      color: white;
    }

    #no {
      background: #ccc;
      position: absolute;
    }

    .heart, .glitter {
      position: fixed;
      top: -10px;
      pointer-events: none;
      animation: fall linear infinite;
    }

    .heart {
      color: #ff2e63;
      font-size: 24px;
    }

    .glitter {
      color: gold;
      font-size: 14px;
    }

    @keyframes fall {
      to {
        transform: translateY(110vh);
        opacity: 0;
      }
    }
  </style>
</head>
<body>

  <div class="card" id="card">
    <h1>Will you be my Valentine, Golu? 💕</h1>
    <button id="yes" onclick="yesClicked()">Yes 💖</button>
    <button id="no" onmouseover="moveNo()">No 🙈</button>
  </div>

  <script>
    function yesClicked() {
