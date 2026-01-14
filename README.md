<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>ECEM — 夜の視覚</title>

<style>
*{margin:0;padding:0;box-sizing:border-box}

body{
  min-height:100vh;
  background:
    repeating-linear-gradient(
      90deg,
      rgba(40,60,140,0.08) 0px,
      rgba(40,60,140,0.08) 1px,
      transparent 1px,
      transparent 6px
    ),
    radial-gradient(circle at 10% 15%, rgba(90,120,255,0.55), transparent 35%),
    radial-gradient(circle at 90% 85%, rgba(20,30,120,0.7), transparent 40%),
    linear-gradient(180deg,#00010a,#020317,#000);
  font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
  color:#eaf0ff;
  overflow:hidden;
}

/* GLITCH LINES */
.scanlines{
  position:fixed;
  inset:0;
  background:
    repeating-linear-gradient(
      to bottom,
      rgba(255,255,255,0.03) 0px,
      rgba(255,255,255,0.03) 1px,
      transparent 2px,
      transparent 4px
    );
  mix-blend-mode:overlay;
  pointer-events:none;
  z-index:3;
}

/* STAR RAIN */
.stars{position:fixed;inset:0;z-index:0;pointer-events:none}
.star{
  position:absolute;
  width:2px;height:2px;
  background:#b9c7ff;
  box-shadow:0 0 18px #9fb4ff,0 0 40px rgba(120,160,255,.9);
  animation:rain linear infinite;
}
@keyframes rain{
  from{transform:translateY(120vh);opacity:0}
  20%{opacity:1}
  to{transform:translateY(-20vh);opacity:0}
}

/* NEON MIST */
.mist{
  position:fixed;
  inset:-20%;
  background:
    radial-gradient(circle at 30% 40%, rgba(60,90,255,.35), transparent 50%),
    radial-gradient(circle at 70% 60%, rgba(20,40,140,.4), transparent 55%);
  filter:blur(80px);
  animation:mistDrift 25s ease-in-out infinite alternate;
  z-index:1;
}
@keyframes mistDrift{
  from{transform:translateX(-10%)}
  to{transform:translateX(10%)}
}

/* CONTENT */
.wrapper{
  position:relative;
  z-index:2;
  max-width:1200px;
  padding:120px;
}

.kanji{
  font-size:1.3rem;
  letter-spacing:10px;
  color:#6f88ff;
  margin-bottom:35px;
  opacity:.85;
}

h1{
  font-size:5.4rem;
  font-weight:900;
  letter-spacing:-2px;
  margin-bottom:35px;
  text-shadow:
    0 0 30px rgba(140,170,255,.7),
    0 0 90px rgba(60,100,255,.9);
}

h1 span{color:#9fb4ff}

h2{
  font-size:1.7rem;
  font-weight:400;
  letter-spacing:3px;
  color:#c6d4ff;
  margin-bottom:65px;
}

p{
  max-width:720px;
  font-size:1.25rem;
  line-height:2.1;
  color:#dde6ff;
}

.buttons{
  margin-top:80px;
  display:flex;
  gap:32px;
}

.button{
  padding:20px 56px;
  border-radius:999px;
  border:1px solid rgba(160,180,255,.6);
  background:rgba(5,10,40,.75);
  color:#eef2ff;
  letter-spacing:3px;
  text-decoration:none;
  backdrop-filter:blur(18px);
  transition:.5s;
}
.button:hover{
  background:#a9baff;
  color:#00010a;
  box-shadow:
    0 0 60px rgba(170,190,255,1),
    0 0 160px rgba(120,150,255,.9);
  transform:translateY(-12px) scale(1.07);
}

footer{
  margin-top:150px;
  font-size:.8rem;
  letter-spacing:5px;
  color:#7f93ff;
  opacity:.7;
}
</style>
</head>

<body>

<div class="stars">
<script>
for(let i=0;i<220;i++){
  document.write(`<div class="star" style="
    left:${Math.random()*100}%;
    animation-duration:${4+Math.random()*7}s;
    animation-delay:${Math.random()*6}s
  "></div>`)
}
</script>
</div>

<div class="mist"></div>
<div class="scanlines"></div>

<div class="wrapper">
  <div class="kanji">夜・視・力</div>

  <h1>Hi, I’m <span>Ecem</span></h1>
  <h2>GRAPHIC DESIGNER & ILLUSTRATOR</h2>

  <p>
    Graphic designer and illustrator with eight years of experience in visual
    storytelling and image-making. My professional focus includes visual identity,
    illustration, and concept-driven design.
    <br><br>
    I develop strong narratives through composition, typography, and
    character-based visuals, aiming to create work that is intentional,
    conceptually grounded, and emotionally precise.
    <br><br>
    Influenced by illustration, digital culture, Japanese visual language, and
    editorial aesthetics, I value clarity, consistency, and meaning.
    This portfolio represents design as both a professional practice and
    a way of thinking.
  </p>

  <div class="buttons">
    <a href="https://www.behance.net/ecemnurkahrman" target="_blank" class="button">
      VIEW PORTFOLIO
    </a>
    <a href="mailto:gwem1720@gmail.com" class="button">
      CONTACT
    </a>
  </div>

  <footer>
    © 2026 ECEM
  </footer>
</div>

</body>
</html>