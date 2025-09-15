<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Love Note for Hope 💜</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background: #f5e6ff;
    }
    .screen {
      display: none;
      padding: 20px;
      border-radius: 12px;
      background: white;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
      margin: 20px auto;
      width: 80%;
    }
    .active {
      display: block;
    }
    button {
      margin: 10px;
      padding: 10px 20px;
      border: none;
      border-radius: 8px;
      background: purple;
      color: white;
      font-size: 16px;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <div id="screen1" class="screen active">
    <h2>Hi Hope 💜</h2>
    <p>I made this just for you!</p>
    <button onclick="showScreen(2)">Next ➡️</button>
  </div>

  <div id="screen2" class="screen">
    <h2>Your Cute Chubby Cheeks 🥰</h2>
    <p>I love them so much!</p>
    <button onclick="showScreen(3)">Next ➡️</button>
  </div>

  <div id="screen3" class="screen">
    <h2>Your Dangerous Laughter 😂💖</h2>
    <p>It’s literally my favorite sound.</p>
    <button onclick="showScreen(4)">Final Surprise 🎁</button>
  </div>

  <div id="screen4" class="screen">
    <h2>The Best Girlfriend Ever 💗</h2>
    <p>That’s YOU, my Hope. Always and forever.</p>
  </div>

  <script>
    function showScreen(num) {
      document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
      document.getElementById('screen' + num).classList.add('active');
    }
  </script>

</body>
</html>
