<!DOCTYPE html>
<html lang="ml">
<head>
  <meta charset="UTF-8">
  <title>ഹാപ്പി വിഷു അമ്മുക്കുട്ടി</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: #ffe066;
      overflow: hidden;
      font-family: 'Noto Sans Malayalam', sans-serif;
    }

    .greeting {
      position: absolute;
      top: 30%;
      width: 100%;
      text-align: center;
      font-size: 2.5em;
      color: #ff5e00;
      text-shadow: 0 0 10px #fff200, 0 0 20px #ffae00;
      animation: glow 2s infinite alternate;
      padding: 0 20px;
    }

    @keyframes glow {
      from {
        text-shadow: 0 0 10px #fff200;
      }
      to {
        text-shadow: 0 0 20px #ffae00, 0 0 30px #ffd700;
      }
    }

    .flower {
      position: absolute;
      width: 40px;
      height: 40px;
      background: url('https://i.imgur.com/Ym4xN1F.png') no-repeat center/cover;
      animation: float 10s linear infinite;
      opacity: 0.8;
    }

    @keyframes float {
      0% {
        transform: translateY(100vh) rotate(0deg);
        opacity: 0;
      }
      50% {
        opacity: 1;
      }
      100% {
        transform: translateY(-20vh) rotate(360deg);
        opacity: 0;
      }
    }

    .subtext {
      margin-top: 20px;
      font-size: 1.2em;
      color: #8b4f00;
      text-shadow: 0 0 5px #fff;
    }
  </style>
  <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Malayalam&display=swap" rel="stylesheet">
</head>
<body>
  <div class="greeting">
    🌸 ഹാപ്പി വിഷു അമ്മുക്കുട്ടി! 🌼<br>
    <div class="subtext">വിഷുക്കണിയുടെ പ്രകാശം പോലെ നിന്റെ പുഞ്ചിരിയും പ്രകാശിക്കട്ടെ ✨</div>
  </div>

  <script>
    // Generate multiple floating flowers
    for (let i = 0; i < 20; i++) {
      const flower = document.createElement('div');
      flower.classList.add('flower');
      flower.style.left = Math.random() * 100 + 'vw';
      flower.style.animationDuration = 8 + Math.random() * 5 + 's';
      flower.style.animationDelay = Math.random() * 5 + 's';
      document.body.appendChild(flower);
    }
  </script>
</body>
</html>
