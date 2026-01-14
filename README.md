<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sole — Designer & Illustrator</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      min-height: 100vh;
      background: linear-gradient(135deg, #0a192f, #112240);
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      color: #e6f1ff;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .container {
      max-width: 900px;
      padding: 60px;
    }

    h1 {
      font-size: 3.5rem;
      margin: 0 0 20px 0;
      letter-spacing: -1px;
    }

    h1 span {
      color: #64ffda;
    }

    p {
      font-size: 1.2rem;
      line-height: 1.6;
      color: #a8b2d1;
      max-width: 600px;
    }

    .buttons {
      margin-top: 40px;
      display: flex;
      gap: 20px;
    }

    .btn {
      padding: 14px 32px;
      border-radius: 30px;
      border: 1px solid #64ffda;
      background: transparent;
      color: #64ffda;
      font-size: 1rem;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .btn:hover {
      background: #64ffda;
      color: #0a192f;
      transform: translateY(-3px);
    }

    .footer {
      margin-top: 80px;
      font-size: 0.9rem;
      color: #8892b0;
    }
  </style>
</head>

<body>
  <div class="container">
    <h1>
      Hi, I’m <span>Sole</span>
    </h1>

    <p>
      I’m a graphic designer & illustrator focused on creating clean,
      expressive visuals and digital experiences.
      I love color, balance and bold ideas.
    </p>

    <div class="buttons">
      <button class="btn">View My Work</button>
      <button class="btn">Contact Me</button>
    </div>

    <div class="footer">
      © 2026 Sole — all rights reserved
    </div>
  </div>
</body>
</html>