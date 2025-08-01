<!DICOTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Nabin Giree | Portfolio</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom right, #e0f7fa, #ffffff);
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      margin: 0;
      padding: 20px;
      transition: background 0.5s;
    }
    .dark-mode {
      background: linear-gradient(to bottom right, #263238, #000000);
      color: #fff;
    }
    .container {
      background: #fff;
      border-radius: 20px;
      max-width: 440px;
      width: 100%;
      padding: 30px;
      text-align: center;
      box-shadow: 0 12px 30px rgba(0, 0, 0, 0.2);
      animation: fadeIn 1.8s ease;
      transition: background 0.5s, color 0.5s;
    }
    .dark-mode .container {
      background: #37474f;
      color: #fff;
    }
    @keyframes fadeIn {
      from {opacity: 0; transform: translateY(40px);}
      to {opacity: 1; transform: translateY(0);}
    }
    img {
      width: 140px;
      border-radius: 50%;
      border: 4px solid #00acc1;
      transition: transform 0.3s ease;
    }
    img:hover {
      transform: scale(1.05);
    }
    h1 {
      color: #00796b;
      margin: 15px 0 10px;
    }
    .dark-mode h1 {
      color: #80deea;
    }
    p {
      font-size: 15px;
      color: #444;
      line-height: 1.6;
    }
    .dark-mode p {
      color: #ddd;
    }
    .friend {
      margin-top: 20px;
      padding-top: 15px;
      border-top: 1px solid #ccc;
    }
    .social-links {
      margin-top: 20px;
    }
    .social-links a {
      display: inline-block;
      margin: 8px;
      padding: 10px 18px;
      border-radius: 30px;
      text-decoration: none;
      font-size: 14px;
      transition: 0.3s ease;
      color: #fff;
    }
    .facebook { background: #1877f2; }
    .tiktok { background: #000000; }
    .instagram { background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fd5949 45%, #d6249f 60%, #285aeb 90%); }

    .social-links a:hover {
      opacity: 0.85;
    }
    button {
      margin-top: 20px;
      padding: 10px 20px;
      border-radius: 25px;
      border: none;
      background-color: #00796b;
      color: white;
      font-size: 14px;
      cursor: pointer;
      transition: background 0.3s;
    }
    button:hover {
      background-color: #004d40;
    }
    audio {
      margin-top: 25px;
      width: 100%;
      outline: none;
      border-radius: 10px;
    }
  </style>
</head>
<body>
  <div class="container" id="profile">
    <img src="https://i.ibb.co/CKdTD7xz/1752939425088-1.jpg" alt="Nabin Photo" />
    <h1 id="name">Nabin Giree</h1>
    <p id="intro">Hi! I’m <strong>Nabin</strong> from Nepal, currently studying in <strong>Class 9</strong>. I love learning web design and development. This is my personal animated website!</p>

    <div class="friend">
      <h2>My Friend</h2>
      <p><strong>Saroj Kunwar</strong> — A progressive, speedy and supportive friend like a big brother.</p>
    </div>

    <div class="social-links">
      <a href="https://www.facebook.com/share/19eDPtmxKe/" target="_blank" class="facebook">Facebook</a>
      <a href="https://vm.tiktok.com/ZSHpfs8tgHUFF-5iHUv/" target="_blank" class="tiktok">TikTok</a>
      <a href="https://www.instagram.com/" target="_blank" class="instagram">Instagram</a>
    </div>

    <!-- Theme Switcher -->
    <button onclick="toggleTheme()">Switch Theme</button>

    <!-- Nepali Song (Audio) -->
    <audio controls autoplay loop>
      <source src="https://www.dropbox.com/scl/fi/36a1tm3gsgdfj1hv6xd5b/Samjhi-Basauna.mp3?rlkey=cn5vwqsm0yqb86acqz9ftbk36&raw=1" type="audio/mpeg" />
      Your browser does not support the audio element.
    </audio>
  </div>

  <script>
    // Fade-in animation for name
    window.addEventListener("DOMContentLoaded", () => {
      const name = document.getElementById("name");
      name.style.opacity = 0;
      let opacity = 0;
      const fadeIn = setInterval(() => {
        opacity += 0.02;
        name.style.opacity = opacity;
        if (opacity >= 1) clearInterval(fadeIn);
      }, 30);
    });

    // Theme toggle (light/dark)
    function toggleTheme() {
      document.body.classList.toggle("dark-mode");
    }
  </script>
</body>
</html>
