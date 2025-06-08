<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Will You Be Mine?</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Comic Sans MS', cursive;
      background: url('your_uploaded_image.jpg') no-repeat center center fixed;
      background-size: cover;
      text-align: center;
      color: white;
      backdrop-filter: blur(5px);
    }
    .container {
      margin-top: 20vh;
    }
    h1 {
      font-size: 3em;
    }
    .btn {
      padding: 15px 30px;
      font-size: 1.2em;
      margin: 20px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: 0.3s;
    }
    .yes {
      background-color: #4CAF50;
      color: white;
    }
    .no {
      background-color: #f44336;
      color: white;
      position: absolute;
    }
    .message {
      display: none;
      font-size: 2em;
      margin-top: 50px;
    }
  </style>
</head>
<body>
  <audio autoplay loop volume="0.2">
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mp3">
  </audio>
  <div class="container">
    <h1>💖 Sanjida Ashrafi, Will you be mine? 💖</h1>
    <button class="btn yes" onclick="showMessage()">Yes</button>
    <button class="btn no" id="noBtn">No</button>
    <div class="message" id="message">🥰 Yay! Easin Arafat loves you so much! 🥰</div>
  </div>
  <script>
    const noBtn = document.getElementById('noBtn');
    const message = document.getElementById('message');noBtn.addEventListener('mouseover', () => {
  const i = Math.floor(Math.random() * window.innerWidth);
  const j = Math.floor(Math.random() * window.innerHeight);
  noBtn.style.left = i + 'px';
  noBtn.style.top = j + 'px';
});

function showMessage() {
  message.style.display = 'block';
}

  </script>
</body>
</html>
