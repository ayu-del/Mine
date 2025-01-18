# Mine
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Do You Love Me?</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #ffe4ec;
      color: #333;
      text-align: center;
      padding: 20px;
    }
    .container {
      margin-top: 10%;
    }
    .question {
      font-size: 28px;
      font-weight: bold;
      margin-bottom: 20px;
    }
    .subtext {
      font-size: 16px;
      margin-bottom: 20px;
      color: #555;
    }
    button {
      font-size: 18px;
      padding: 10px 20px;
      margin: 10px;
      cursor: pointer;
      border: none;
      border-radius: 5px;
    }
    .yes {
      background-color: #6dd17a;
      color: white;
    }
    .no {
      background-color: #f14c4c;
      color: white;
    }
    .emoji {
      font-size: 50px;
      margin-bottom: 20px;
    }
    img {
      max-width: 150px;
      margin-bottom: 20px;
    }
  </style>
</head>
<body>
  <div class="container">
    <img src="https://i.imgur.com/Q5XhMbJ.png" alt="Cute Cat"> <!-- Replace with your preferred image -->
    <div class="emoji">🥰</div>
    <div class="question">Do you love me?</div>
    <div class="subtext">~vaidehi is all yours</div>
    <button class="yes" onclick="handleYes()">Yes</button>
    <button class="no" onclick="handleNo()">No</button>
  </div>

  <script>
    const messages = [
      "PARAT V4 KRR! 😢",
      "PAKKA SOCH LEE 🥺",
      "FINAL SOCH LE ❤️",
      "MUJHSE NARAAZ HO KYA? 😔",
      "PLEASE BOLO YES 😭"
    ];
    let messageIndex = 0;

    function handleYes() {
      alert("I love you too! 🥰");
    }

    function handleNo() {
      if (messageIndex < messages.length) {
        document.querySelector('.question').innerText = messages[messageIndex];
        messageIndex++;
      } else {
        document.querySelector('.question').innerText = "AB TO HAAN BOL DO! 🙏";
      }
    }
  </script>
</body>
</html>
