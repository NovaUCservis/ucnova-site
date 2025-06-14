<!DOCTYPE html><html lang="uz">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>NOVA UC Redeem Code</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f3f4f6;
      text-align: center;
      padding: 50px;
    }
    .box {
      background: white;
      padding: 30px;
      max-width: 400px;
      margin: auto;
      border-radius: 12px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    input[type="text"] {
      padding: 10px;
      width: 80%;
      margin-top: 20px;
      border-radius: 8px;
      border: 1px solid #ccc;
    }
    button {
      margin-top: 20px;
      padding: 10px 20px;
      border: none;
      border-radius: 8px;
      background: #4f46e5;
      color: white;
      font-weight: bold;
      cursor: pointer;
    }
    .result {
      margin-top: 20px;
      font-size: 18px;
      font-weight: bold;
    }
    .nav {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      background: #4f46e5;
      color: white;
      padding: 10px 0;
      font-size: 18px;
      font-weight: bold;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .nav a {
      color: white;
      text-decoration: none;
      margin: 0 15px;
    }
  </style>
</head>
<body>
  <div class="nav">
    <a href="/ucnova-site/">🏠 Bosh sahifa</a>
    <a href="/ucnova-site/redeem.html">🎁 Redeem Kod</a>
  </div>  <div class="box" style="margin-top: 80px">
    <h2>🎁 UC Kodni Aktivlashtirish</h2>
    <p>Promo kodni kiriting va sovg'angizni oling!</p>
    <input type="text" id="codeInput" placeholder="Promo kodni kiriting">
    <br>
    <button onclick="checkCode()">✅ Tekshirish</button>
    <div id="result" class="result"></div>
  </div>  <script>
    const validCodes = {
      "ERWIN2025": "60 UC",
      "NOVAUC10": "10 UC",
      "YUTIQ100": "100 UC",
      "FREEPASS": "Free Royal Pass"
    };

    function checkCode() {
      const input = document.getElementById('codeInput').value.trim().toUpperCase();
      const result = document.getElementById('result');

      if (validCodes[input]) {
        result.style.color = 'green';
        result.textContent = `🎉 Tabriklaymiz! Siz ${validCodes[input]} yutdingiz.`;
      } else {
        result.style.color = 'red';
        result.textContent = "❌ Kechirasiz, bu kod noto'g'ri yoki muddati tugagan.";
      }
    }
  </script></body>
</html>
