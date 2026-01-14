<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>ECEM 夜青</title>

<style>
*{margin:0;padding:0;box-sizing:border-box}

body{
  height:100vh;
  background:
    radial-gradient(circle at 30% 20%, #050a25 0%, transparent 40%),
    radial-gradient(circle at 70% 80%, #020617 0%, transparent 45%),
    linear-gradient(180deg,#00010a,#020318,#00010a);
  font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
  overflow:hidden;
  color:#cfd9ff;
}

/* STAR FIELD */
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
    0 0 14px #0a1a4f,
    0 0 30px rgba(20,40,120,.9);
  animation:fall linear infinite;
}
@keyframes fall{
  from{transform:translateY(110vh);opacity:0}
  10%{opacity:1}
  to{transform:translateY(-10vh);opacity:0}
}

/* DARK MIST */
.mist{
  position:fixed;
  inset:-20%;
  background:
    radial-gradient(circle at 20% 30%, rgba(10,20,80,.6), transparent 50%),
    radial-gradient(circle at 80% 70%, rgba(5,10,40,.8), transparent 55%);
  filter:blur(90px);
  animation:drift 30s alternate infinite ease-in-out;
  z-index:1;
}
@keyframes drift{
  from{transform:translateX(-10%)}
  to{transform:translateX(10%)}
}

/* SCANLINES */
.scanlines{
  position:fixed;
  inset:0;
  background:
    repeating-linear-gradient(
      to bottom,
      rgba(0,0,0,.35) 0px,
      rgba(0,0,0,.35) 1px,
      transparent 3px,
      transparent 5px
    );
  z-index:4;
  pointer-events:none;
}

/* CONTENT */
.wrapper{
  position:relative;
  z-index:3;
  max-width:1100px;
  padding:110px;
}

.kanji{
  color:#243a8a;
  letter-spacing:12px;
  margin-bottom:40px;
  font-size:1.2rem;
}

h1{
  font-size:5.2rem;
  letter-spacing:4px;
  color:#e4ebff;
  text-shadow:
    0 0 25px rgba(40,80,180,.8),
    0 0 80px rgba(20,40,120,.9);
}

h2{
  margin-top:20px;
  font-size:1.4rem;
  letter-spacing:6px;
  color:#9fb0ff;
}

p{
  margin-top:60px;
  max-width:760px;
  font-size:1.15rem;
  line-height:2.2;
  color:#c7d3ff;
}

/* BUTTONS */
.buttons{
  margin-top:90px;
  display:flex;
  gap:40px;
}

.button{
  padding:18px 52px;
  border-radius:999px;
  border:1px solid #1b2b6f;
  background:rgba(5,10,30,.85);
  color:#dfe6ff;
  letter-spacing:4px;
  text-decoration:none;
  backdrop-filter:blur(12px);
  transition:.4s;
}
.button:hover{
  background:#0a1440;
  box-shadow:
    0 0 40px rgba(40,80,180,.9),
    0 0 120px rgba(20,40,120,.9);
  transform:translateY(-8px) scale(1.05);
}
</style>
</head>

<body>

<div class="stars">
<script>
for(let i=0;i<420;i++){
  document.write(`
    <div class="star" style="
      left:${Math.random()*100}%;
      animation-duration:${3+Math.random()*6}s;
      animation-delay:${Math.random()*5}s;
    "></div>
  `)
}
</script>
</div>

<div class="mist"></div>
<div class="scanlines"></div>

<div class="wrapper">
  <div class="kanji">夜・青・影</div>

  <h1>ECEM</h1>
  <h2>GRAPHIC DESIGNER & ILLUSTRATOR</h2>

  <p>
    Graphic designer and illustrator with eight years of experience in visual
    storytelling and image-making. My professional focus includes visual identity,
    illustration, and concept-driven design.
    <br><br>
    I build strong narratives through composition, typography, and
    character-based visuals, aiming to create work that is intentional,
    conceptually grounded, and precise.
    <br><br>
    Influenced by Japanese visual culture, darkness, and editorial aesthetics.
    Design as atmosphere. Image as language.
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