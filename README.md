<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>ECEM 夜の設計</title>

<style>
*{margin:0;padding:0;box-sizing:border-box}

body{
  height:100vh;
  background:
    radial-gradient(circle at 20% 30%, #02082a 0%, transparent 35%),
    radial-gradient(circle at 80% 70%, #010414 0%, transparent 40%),
    linear-gradient(180deg,#000,#020318,#000);
  font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
  overflow:hidden;
  color:#dfe6ff;
}

/* NOISE */
.noise{
  position:fixed;
  inset:0;
  background-image:url("https://grainy-gradients.vercel.app/noise.svg");
  opacity:.25;
  z-index:10;
  pointer-events:none;
}

/* STAR CHAOS */
.stars{
  position:fixed;
  inset:0;
  z-index:0;
  pointer-events:none;
}
.star{
  position:absolute;
  width:2px;
  height:2px;
  background:#1b2b6f;
  box-shadow:
    0 0 6px #1b2b6f,
    0 0 18px rgba(40,80,180,.9),
    0 0 40px rgba(20,40,120,.9);
  animation:fall linear infinite;
}
@keyframes fall{
  from{transform:translateY(120vh)}
  to{transform:translateY(-20vh)}
}

/* FLOAT TEXT */
.float-text{
  position:absolute;
  color:#16245c;
  font-size:1.1rem;
  letter-spacing:4px;
  opacity:.7;
  animation:float 30s linear infinite;
}
@keyframes float{
  from{transform:translateY(120vh)}
  to{transform:translateY(-120vh)}
}

/* BIG KANJI */
.big-kanji{
  position:absolute;
  font-size:9rem;
  font-weight:900;
  color:#050a2a;
  opacity:.6;
  writing-mode:vertical-rl;
}

/* MAIN */
.wrapper{
  position:relative;
  z-index:5;
  padding:120px;
  max-width:1200px;
}

h1{
  font-size:5.5rem;
  letter-spacing:4px;
  text-shadow:
    0 0 30px rgba(40,80,180,.9),
    0 0 100px rgba(20,40,120,.9);
}

h2{
  margin-top:18px;
  letter-spacing:6px;
  color:#9fb0ff;
}

p{
  margin-top:60px;
  max-width:760px;
  line-height:2.2;
  font-size:1.15rem;
}

/* BUTTONS */
.buttons{
  margin-top:90px;
  display:flex;
  gap:36px;
}

.button{
  padding:20px 56px;
  border-radius:999px;
  border:1px solid #1b2b6f;
  background:rgba(5,10,40,.85);
  color:#eaf0ff;
  letter-spacing:4px;
  text-decoration:none;
  backdrop-filter:blur(12px);
  transition:.4s;
}
.button:hover{
  background:#0a1440;
  box-shadow:
    0 0 50px rgba(40,80,180,1),
    0 0 140px rgba(20,40,120,1);
  transform:translateY(-10px) scale(1.06);
}
</style>
</head>

<body>

<!-- STARS -->
<div class="stars">
<script>
for(let i=0;i<650;i++){
  document.write(`
    <div class="star" style="
      left:${Math.random()*100}%;
      animation-duration:${2+Math.random()*5}s;
      animation-delay:${Math.random()*6}s;
    "></div>
  `)
}
</script>
</div>

<!-- FLOATING TEXT -->
<script>
const words=["TOKYO","VISUAL","DARK","夜","設計","IMAGE","NOISE","EDITORIAL","ILLUSTRATION"];
for(let i=0;i<25;i++){
  document.write(`
    <div class="float-text" style="
      left:${Math.random()*100}%;
      animation-duration:${20+Math.random()*30}s;
      animation-delay:${Math.random()*10}s;
    ">
      ${words[Math.floor(Math.random()*words.length)]}
    </div>
  `)
}
</script>

<!-- BIG KANJI -->
<div class="big-kanji" style="top:10%;left:5%;">夜</div>
<div class="big-kanji" style="bottom:5%;right:8%;">黒</div>

<div class="noise"></div>

<div class="wrapper">
  <h1>ECEM</h1>
  <h2>GRAPHIC DESIGNER & ILLUSTRATOR</h2>

  <p>
  Graphic designer and illustrator with eight years of experience in visual storytelling and image-makeing. My professional focus includes visual identity, illustration, and concept-driven design.
I have experience in developing strong narratives through composition. Typography, and character-based visuals, aiming to create designs that are intentional and conceptually grounded rather than purely decorative.
Throughout my career, i have built a distinctive visual language influenced by illustration, digital culture, and editorial aesthetics.. I value clarity, consistency, and meaning in design, And i strive to produce visuals that communicate ideas with confidence and precision. This portfolio represents my long-term dedication to graphic design And illustration as both a professional pratice and a way of thinking.
  </p>

  <div class="buttons">
    <a class="button" href="https://www.behance.net/ecemnurkahrman" target="_blank">
      VIEW PORTFOLIO
    </a>
    <a class="button" href="mailto:gwem1720@gmail.com">
      CONTACT
    </a>
  </div>
</div>

</body>
</html>