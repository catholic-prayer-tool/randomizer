# randomizer
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Catholic Prayer Randomizer</title>
  <style>
    body {
      font-family: Georgia, serif;
      background-color: #fdfdfd;
      color: #333;
      padding: 2em;
      text-align: center;
    }
    h1 {
      font-size: 1.8em;
      margin-bottom: 1em;
    }
    button {
      font-size: 1.2em;
      padding: 0.6em 1.2em;
      margin-top: 1em;
      border-radius: 0.5em;
      border: none;
      background-color: #4a5c6a;
      color: white;
      cursor: pointer;
    }
    button:hover {
      background-color: #394a56;
    }
    #quote {
      margin-top: 2em;
      font-size: 1.2em;
      white-space: pre-wrap;
    }
  </style>
</head>
<body>
  <h1>✡️ Catholic Prayer Randomizer</h1>
  <button onclick="showRandom()">Show Me One</button>
  <div id="quote">Click the button for a prayer, quote, or verse.</div>

  <script>
    const items = [
      // Inserted full list begins below
      "COME HOLY SPIRIT",
      "THY WILL BE DONE.",
      "MY GOD AND MY ALL.",
      "Lord, I am not worthy",
      "O HEART OF JESUS, ALL FOR THEE.",
      "O GOD, HAVE MERCY ON ME, A SINNER.",
      // The rest of your full list goes here...
      "‘Do not be afraid. Do not be satisfied with mediocrity. Put out into the deep and let down your nets for a catch.’ – St. John Paul II",
      "‘Let nothing trouble you, let nothing make you afraid. All things pass away. God never changes. Patience obtains everything. God alone is enough.’ – St. Teresa of Avila",
      "‘I will spend my heaven doing good on earth.’ – St. Thérèse of Lisieux",
      "‘Prayer is the foundation of the spiritual edifice. Prayer is all powerful.’ – St. Josemaria Escriva"
    ];

    function showRandom() {
      const choice = items[Math.floor(Math.random() * items.length)];
      document.getElementById("quote").innerText = choice;
    }
  </script>
</body>
</html>
