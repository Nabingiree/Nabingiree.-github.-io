<!DOCTYPE html>
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
    }
    .container {
      background: #fff;
      border-radius: 20px;
      max-width: 420px;
      width: 100%;
      padding: 25px;
      text-align: center;
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
      animation: fadeIn 2s ease;
    }
    @keyframes fadeIn {
      from {opacity: 0; transform: translateY(30px);}
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
    p {
      font-size: 15px;
      color: #444;
      line-height: 1.6;
    }
    .friend {
      margin-top: 20px;
      padding-top: 15px;
      border-top: 1px solid #ddd;
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
    audio {
      margin-top: 20px;
      width: 100%;
      outline: none;
    }
  </style>
</head>
<body>
  <div class="container" id="profile">
    <img src="https://i.ibb.co/CKdTD7xz/1752939425088-1.jpg" alt="Nabin Photo" />
    <h1 id="name">Nabin Giree</h1>
    <p>Hello! I'm <strong>Nabin</strong> from Nepal. Welcome to my animated and responsive portfolio site made with HTML, CSS & JavaScript.</p>

    <div class="friend">
      <h2>My Friend</h2>
      <p><strong>Saroj Kunwar</strong> — A progressive, speedy and supportive friend like a big brother.</p>
    </div>

    <div class="social-links">
      <a href="https://www.facebook.com/share/19eDPtmxKe/" target="_blank" class="facebook">Facebook</a>
      <a href="https://vm.tiktok.com/ZSHpfs8tgHUFF-5iHUv/" target="_blank" class="tiktok">TikTok</a>
      <a href="https://www.instagram.com/" target="_blank" class="instagram">Instagram</a>
    </div>

    <!-- Background music -->
    <audio autoplay loop controls>
      <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg" />
      Your browser does not support the audio element.
    </audio>
  </div>

  <script>
    // Simple JS animation: name fade-in
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
  </script>
</body>
</html>
