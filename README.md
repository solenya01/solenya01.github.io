<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sole | Designer & Illustrator</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      min-height: 100vh;
      background:
        radial-gradient(circle at 30% 20%, rgba(40,60,120,0.35), transparent 45%),
        radial-gradient(circle at 70% 80%, rgba(20,30,80,0.4), transparent 50%),
        linear-gradient(160deg, #05070f, #0a1430, #02040a);
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      color: #eef1ff;
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
    }

    /* ✨ YILDIZLAR */
    .stars {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      z-index: 0;
    }

    .star {
      position: absolute;
      width: 2px;
      height: 2px;
      background: rgba(160,180,255,0.8);
      border-radius: 50%;
      animation: floatStar 6s linear infinite;
    }

    @keyframes floatStar {
      from {
        transform: translateY(110vh);
        opacity: 0;
      }
      30% {
        opacity: 1;
      }
      to {
        transform: translateY(-10vh);
        opacity: 0;
      }
    }

    /* 📦 İÇERİK */
    .wrapper {
      position: relative;
      z-index: 2;
      max-width: 1000px;
      padding: 90px;
    }

    h1 {
      font-size: 4.2rem;
      font-weight: 700;
      margin-bottom: 20px;
      letter-spacing: -1px;
      text-shadow:
        0 0 12px rgba(90,120,255,0.35),
        0 0 40px rgba(30,50,120,0.4);
    }

    h1 span {
      color: #7aa2ff;
    }

    h2 {
      font-size: 1.4rem;
      font-weight: 400;
      color: #a9b8ff;
      margin-bottom: 40px;
    }

    p {
      max-width: 600px;
      font-size: 1.15rem;
      line-height: 1.8;
      color: #d6e0ff;
    }

    .buttons {
      margin-top: 50px;
      display: flex;
      gap: 20px;
    }

    .button {
      padding: 14px 38px;
      border-radius: 999px;
      border: 1px solid rgba(120,140,255,0.4);
      background: rgba(10,20,60,0.6);
      color: #e6ebff;
      font-size: 1rem;
      cursor: pointer;
      transition: all 0.4s ease;
      backdrop-filter: blur(10px);
      text-decoration: none;
    }

    .button:hover {
      background: rgba(120,140,255,0.85);
      color: #05070f;
      box-shadow: 0 0 35px rgba(120,140,255,0.8);
      transform: translateY(-6px);
    }

    footer {
      margin-top: 90px;
      font-size: 0.85rem;
      color: #7f91b3;
      letter-spacing: 0.5px;
    }
  </style>
</head>

<body>

  <!-- ✨ STARS -->
  <div class="stars">
    <div class="star" style="left:10%; animation-delay:0s;"></div>
    <div class="star" style="left:25%; animation-delay:2s;"></div>
    <div class="star" style="left:40%; animation-delay:4s;"></div>
    <div class="star" style="left:60%; animation-delay:1s;"></div>
    <div class="star" style="left:75%; animation-delay:3s;"></div>
    <div class="star" style="left:90%; animation-delay:5s;"></div>
  </div>

  <!-- 💙 CONTENT -->
  <div class="wrapper">
    <h1>Hi, I’m <span>Sole</span></h1>
    <h2>Graphic Designer & Illustrator</h2>

    <p>
      I create visual stories through illustration and graphic design.
      Focused on dark aesthetics, strong contrasts and feminine energy.
    </p>

    <div class="buttons">
      <a href="https://www.behance.net/ecemnurkahrman" target="_blank" class="button">
        View Portfolio
      </a>
      <a href="mailto:gwem1720@gmail.com" class="button">
        Contact
      </a>
    </div>

    <footer>
      © 2026 Sole
    </footer>
  </div>

</body>
</html>