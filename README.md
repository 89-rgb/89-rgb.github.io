<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Senin İçin</title>
  <style>
    body {
      background: linear-gradient(#fbc2eb, #a6c1ee);
      font-family: 'Segoe UI', sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      color: #333;
      text-align: center;
      padding: 20px;
    }
    h1 {
      font-size: 2.5em;
      margin-bottom: 0.5em;
    }
    #messageBox {
      font-size: 1.5em;
      background: #fff;
      padding: 20px;
      border-radius: 20px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.2);
      max-width: 600px;
      transition: all 0.3s ease;
    }
    button {
      margin-top: 2em;
      padding: 12px 24px;
      font-size: 1em;
      border: none;
      border-radius: 10px;
      background-color: #ff5e78;
      color: white;
      cursor: pointer;
      transition: background-color 0.3s;
    }
    button:hover {
      background-color: #e04e68;
    }
  </style>
</head>
<body>
  <h1>Senin İçin Küçük Bir Sürpriz</h1>
  <div id="messageBox">Hazır mısın? Bir şey söylemek istiyorum...</div>
  <button onclick="showMessage()">Bana tıkla</button>

  <script>
    const messages = [
      "Gülüşünü görmesem bile hayal etmek yetiyor.",
      "Bugün aklımdan geçen en güzel şey sendin.",
      "Seninle konuşmak bile ayrı bir huzur.",
      "Bir tebessümün, en yorgun anımı bile unutturur.",
      "Sen farkında değilsin ama, kalbimde güzel bir yerdesin.",
      "Seninle aynı zaman diliminde olmak bile güzel."
    ];

    function showMessage() {
      const box = document.getElementById("messageBox");
      const random = Math.floor(Math.random() * messages.length);
      box.textContent = messages[random];
    }
  </script>
</body>
</html>
