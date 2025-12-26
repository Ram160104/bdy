<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Happy Birthday GIRIJA🎉</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    body {
      margin: 0;
      height: 100vh;
      background-image: url("https://images.unsplash.com/photo-1501973801540-537f08ccae7b");
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Segoe UI', sans-serif;
    }

    body::before {
      content: "";
      position: absolute;
      inset: 0;
      background: rgba(0, 0, 0, 0.35);
    }

    .card {
      position: relative;
      z-index: 1;
      background: rgba(255, 255, 255, 0.95);
      padding: 40px;
      border-radius: 20px;
      text-align: center;
      max-width: 350px;
      box-shadow: 0 20px 40px rgba(0,0,0,0.2);
      animation: fadeIn 2s ease;
    }

    h1 {
      color: #ff4d6d;
      font-size: 28px;
      margin-bottom: 10px;
    }

    h2 {
      color: #333;
      font-weight: normal;
    }

    p {
      color: #555;
      font-size: 16px;
      line-height: 1.6;
      margin-top: 20px;
    }

    button {
      margin-top: 25px;
      padding: 12px 25px;
      border: none;
      border-radius: 30px;
      background: #ff4d6d;
      color: white;
      font-size: 16px;
      cursor: pointer;
      transition: 0.3s;
    }

    button:hover {
      background: #e63e5c;
      transform: scale(1.05);
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translateY(30px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .heart {
      position: absolute;
      color: #ff4d6d;
      font-size: 20px;
      animation: floatUp 6s linear infinite;
    }

    @keyframes floatUp {
      from {
        transform: translateY(100vh);
        opacity: 1;
      }
      to {
        transform: translateY(-10vh);
        opacity: 0;
      }
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>🎂 Happy Birthday!</h1>
    <h2>To GIRIJA 💖</h2>

    
    <p>On this beautiful day,</p>
    <p>I just want you to know how special you are.</p>  
    <p>Your smile makes everything brighter</p>
    <p>and your presence makes life sweeter.</p>
    <p>Even the small talks to you feels so much better.</p>
    <p>Thanks for coming into my life.</p>

    <p>
      May your birthday be filled with happiness,  
      love, and everything your heart wishes for 🌸
    </p>

    <button onclick="showSurprise()">ONE LAST THING</button>
  </div>

  <script>
    function showSurprise() {
      alert("I am just feeling the days without talking to you are hard \nI am really sorry for what I did back then.\nPlease Matladachu ga \nYou make every day feel special 💕 \nHappy Birthday to the most beautiful soul 🎉");
    }

    function createHeart() {
      const heart = document.createElement("div");
      heart.classList.add("heart");
      heart.innerHTML = "❤";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.fontSize = Math.random() * 20 + 15 + "px";
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 6000);
    }

    setInterval(createHeart, 500);
  </script>

</body>
</html>
