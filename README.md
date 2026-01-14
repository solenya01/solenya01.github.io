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
        radial-gradient(circle at 20% 10%, rgba(40,60,140,0.45), transparent 40%),
        radial-gradient(circle at 80% 90%, rgba(10,20,80,0.6), transparent 45%),
        linear-gradient(180deg, #02030a, #050b1e, #00010a);
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      color: #eef1ff;
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
    }

    /* ✦ STARS SKY */
    .stars {
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 0;
    }

    .star {
      position: absolute;
      width: 2px;
      height: 2px;
      background: rgba(180,200,255,0.95);
      border-radius: 50%;
      box-shadow: 0 0 12px rgba(140,170,255,0.9);
      animation: starMove linear infinite;
    }

    @keyframes starMove {
      from {
        transform: translateY(110vh);
        opacity: 0;
      }
      20% { opacity: 1; }
      to {
        transform: translateY(-20vh);
        opacity: 0;
      }
    }

    /* ✦ CONTENT */
    .wrapper {
      position: relative;
      z-index: 2;
      max-width: 1100px;
      padding: 100px;
    }

    h1 {
      font-size: 4.6rem;
      font-weight: 700;
      letter-spacing: -1px;
      margin-bottom: 24px;
      color: #f1f3ff;
      text-shadow:
        0 0 20px rgba(120,150,255,0.45),
        0 0 60px rgba(40,70,180,0.5);
    }

    h1 span {
      color: #8fa8ff;
    }

    h2 {
      font-size: 1.5rem;
      font-weight: 400;
      letter-spacing: 0.5px;
      color: #b7c6ff;
      margin-bottom: 50px;
    }

    p {
      max-width: 620px;
      font-size: 1.2rem;
      line-height: 1.9;
      color: #d8e0ff;
    }

    .buttons {
      margin-top: 60px;
      display: flex;
      gap: 24px;
    }

    .button {
      padding: 16px 44px;
      border-radius: 999px;
      border: 1px solid rgba(140,160,255,0.45);
      background: rgba(15,25,80,0.7);
      color: #eef1ff;
      font-size: 1rem;
      cursor: pointer;
      text-decoration: none;
      transition: all 0.45s ease;
      backdrop-filter: blur(14px);
      letter-spacing: 0.5px;
    }

    .button:hover {
      background: rgba(150,170,255,0.95);
      color: #02030a;
      box-shadow:
        0 0 40px rgba(150,170,255,0.9),
        0 0 80px rgba(80,120,255,0.7);
      transform: translateY(-8px);
    }

    footer {
      margin-top: 110px;
      font-size: 0.85rem;
      color: #8b9bd1;
      letter-spacing: 1px;
    }
  </style>
</head>

<body>

  <!-- ✦ STAR FIELD -->
  <div class="stars">
    <div class="star" style="left:5%; animation-duration:7s;"></div>
    <div class="star" style="left:12%; animation-duration:9s;"></div>
    <div class="star" style="left:18%; animation-duration:6s;"></div>
    <div class="star" style="left:26%; animation-duration:8s;"></div>
    <div class="star" style="left:34%; animation-duration:10s;"></div>
    <div class="star" style="left:42%; animation-duration:7s;"></div>
    <div class="star" style="left:50%; animation-duration:9s;"></div>
    <div class="star" style="left:58%; animation-duration:6s;"></div>
    <div class="star" style="left:66%; animation-duration:8s;"></div>
    <div class="star" style="left:74%; animation-duration:10s;"></div>
    <div class="star" style="left:82%; animation-duration:7s;"></div>
    <div class="star" style="left:90%; animation-duration:9s;"></div>
  </div>

  <!-- ✦ MAIN -->
  <div class="wrapper">
    <h1>Hi, I’m <span>Sole</span></h1>
    <h2>Graphic Designer & Illustrator</h2>

    <p>
      I create dark, expressive visuals inspired by night cities,
      feminine power and subtle chaos.
      Illustration and design are my way of telling quiet but dangerous stories.
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