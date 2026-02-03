# free-Valentine-Questionnaire-
is a real hassle-free yes or no question for your special someone 
[valentine2.html](https://github.com/user-attachments/files/25031100/valentine2.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Valentine’s Request 💘</title>
  <style>
    body {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      font-family: Arial, sans-serif;
      background: #ffd6e8;
      text-align: center;
    }

    h1 {
      font-size: 2.5em;
      margin-bottom: 10px;
    }

    .dog {
      width: 150px;
      margin-bottom: 15px;
      border-radius: 10px;
    }

    .buttons {
      position: relative;
      margin-top: 20px;
    }

    button {
      font-size: 1.2em;
      padding: 12px 24px;
      margin: 10px;
      cursor: pointer;
      transition: transform 0.3s ease;
    }

    #yes {
      z-index: 2;
    }

    #no {
      z-index: 1;
    }
  </style>
</head>
<body>

<img class="dog" src="https://media.giphy.com/media/26ufdipQqU2lhNA4g/giphy.gif" alt="Cute Scooby-Doo">
<h1>Will you be my Valentine?</h1>
<p>(Ruh-roh… choose wisely 😏)</p>

<div class="buttons">
  <button id="yes" onclick="alert('YAY!! I love you forever ❤️🐶')">
    YES 💕
  </button>
  <button id="no">NO 💔</button>
</div>

<script>
  const yesBtn = document.getElementById('yes');
  const noBtn = document.getElementById('no');

  let scale = 1;
  let texts = [
    "pleases!!! 💕",
    "come on bro pleasessssss!!!!! 😭",
    "it's not like I'm begging 😅",
    "I'm begging now 😭💘",
    "please please please!! 🐶❤️",
    "ok last try… I love you!! 💖"
  ];
  let clickCount = 0;

  noBtn.addEventListener('click', () => {
    // Grow YES
    scale += 0.3;
    yesBtn.style.transform = `scale(${scale})`;

    // Change YES text
    if (clickCount < texts.length) {
      yesBtn.innerText = texts[clickCount];
      clickCount++;
    }
  });
</script>

</body>
</html>
