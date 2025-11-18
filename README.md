 <!DOCTYPE html><html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Princess Day</title>
<style>
  body {
    margin: 0;
    background: #ffe6f2;
    overflow: hidden;
    font-family: "Poppins", sans-serif;
  }/* Center popup */ .popup { position: fixed; top: 50%; left: 50%; transform: translate(-50%, -50%); background: white; padding: 25px 35px; border-radius: 20px; box-shadow: 0 0 25px rgba(255, 105, 180, 0.4); text-align: center; z-index: 10; } .popup h2 { margin: 0; color: #ff4da6; font-size: 22px; }

/* Floating hearts */ .heart { position: absolute; color: #ff4da6; font-size: 22px; animation: floatUp linear infinite; opacity: 0.8; }

@keyframes floatUp { 0% { transform: translateY(0) scale(1); opacity: 1; } 100% { transform: translateY(-120vh) scale(1.5); opacity: 0; } } </style>

</head>
<body><div class="popup">
  <h2>💗 Happy Princess Day My Princess Appu 💗</h2>
</div><script>
  function createHeart() {
    const heart = document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML = "❤️";

    heart.style.left = Math.random() * 100 + "vw";
    heart.style.animationDuration = (2 + Math.random() * 3) + "s";
    heart.style.fontSize = (18 + Math.random() * 20) + "px";

    document.body.appendChild(heart);

    setTimeout(() => heart.remove(), 4000);
  }

  setInterval(createHeart, 200);
</script></body>
</html>