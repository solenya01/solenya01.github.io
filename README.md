# solenya01.github.io
<!DOCTYPE html>
<html>
<head>
  <title>Awesome Portfolio</title>
  <style>
    /* GENEL AYARLAR */
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4); /* gradient arkaplan */
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      color: #333;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      text-align: center;
      animation: fadeIn 2s ease-in;
    }

    /* BAŞLIK */
    h1 {
      font-size: 3rem;
      color: #fff;
      text-shadow: 2px 2px 10px rgba(0,0,0,0.3);
      margin-bottom: 20px;
    }

    /* ALT YAZI */
    p {
      font-size: 1.2rem;
      color: #fff;
      max-width: 600px;
      line-height: 1.5;
    }

    /* BUTON */
    .btn {
      margin-top: 30px;
      padding: 10px 30px;
      font-size: 1rem;
      color: #ff9a9e;
      background-color: #fff;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .btn:hover {
      transform: scale(1.1);
      background-color: rgba(255,255,255,0.8);
    }

    /* BASİT ANİMASYON */
    @keyframes fadeIn {
      from {opacity: 0;}
      to {opacity: 1;}
    }

  </style>
</head>
<body>
  <h1>Hi, I'm Sole</h1>
  <p>I'm a passionate graphic designer & illustrator creating vibrant visuals and telling stories through colors and shapes. Welcome to my colorful world!</p>
  <button class="btn">Check my work</button>
</body>
</html>