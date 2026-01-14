<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Sole — 夜の女神</title>

<style>
*{margin:0;padding:0;box-sizing:border-box}

body{
  min-height:100vh;
  background:
    radial-gradient(circle at 15% 20%, rgba(90,120,255,0.5), transparent 35%),
    radial-gradient(circle at 85% 80%, rgba(30,50,160,0.6), transparent 40%),
    linear-gradient(180deg,#00010a,#020317,#000);
  font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
  color:#eaf0ff;
  overflow:hidden;
}

/* ✦ STAR STORM */
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
  background:#b7c8ff;
  box-shadow:0 0 15px #9fb4ff,0 0 30px rgba(120,150,255,0.8);
  animation:fall linear infinite;
}

@keyframes fall{
  from{transform:translateY(120vh);opacity:0}
  15%{opacity:1}
  to{transform:translateY(-20vh);opacity:0}
}

/* ✦ MIST */
.mist{
  position:fixed;
  inset:0;
  background:
    radial-gradient(circle at 30% 60%, rgba(40,60,120,0.25), transparent 50%),
    radial-gradient(circle at 70% 30%, rgba(20,30,90,0.3), transparent 55%);
  filter:blur(40px);
  animation:mistMove 20s ease-in-out infinite alternate;
  z-index:1;
}

@keyframes mistMove{
  from{transform:translateX(-5%)}
  to{transform:translateX(5%)}
}

/* ✦ CONTENT */
.wrapper{
  position:relative;
  z-index:2;
  max-width:1200px;
  padding:120px;
}

.jp{
  font-size:1.2rem;
  letter-spacing:8px;
  color:#7f95ff;
  opacity:0.8;
  margin-bottom:30px;
}

h1{
  font-size:5.2rem;
  font-weight:800;
  letter-spacing:-2px;
  margin-bottom:30px;
  text-shadow:
    0 0 25px rgba(140,170,255,0.6),
    0 0 80px rgba(60,100,255,0.8);
}

h1 span{
  color:#9fb4ff;
}

h2{
  font-size:1.6rem;
  font-weight:400;
  letter-spacing:2px;
  color:#c6d4ff;
  margin-bottom:60px;
}

p{
  max-width:680px;
  font-size:1.25rem;
  line-height:2;
  color:#dbe4ff;
}

.buttons{
  margin-top:70px;
  display:flex;
  gap:30px;
}

.button{
  padding:18px 50px;
  border-radius:999px;
  border:1px solid rgba(150,170,255,0.6);
  background:rgba(10,15,60,0.7);
  color:#eef2ff;
  text-decoration:none;
  font-size:1rem;
  letter-spacing:2px;
  backdrop-filter:blur(16px);
  transition:all .45s ease;
}

.button:hover{
  background:#9fb4ff;
  color:#00010a;
  box-shadow:
    0 0 50px rgba(160,180,255,1),
    0 0 120px rgba(100,140,255,0.9);
  transform:translateY(-10px) scale(1.05);
}

footer{
  margin-top:130px;
  font-size:.8rem;
  letter-spacing:4px;
  color:#8fa2ff;
  opacity:.7;
}
</style>
</head>

<body>

<!-- STAR CHAOS -->
<div class="stars">
  <script>
    for(let i=0;i<120;i++){
      document.write(
        `<div class="star" style="
          left:${Math.random()*100}%;
          animation-duration:${5+Math.random()*6}s;
          animation-delay:${Math.random()*6}s
        "></div>`
      )
    }
  </script>
</div>

<div class="mist"></div>

<div class="wrapper">
  <div class="jp">夜 • 美 • 力</div>

  <h1>Hi, I’m <span>Sole</span></h1>
  <h2>Graphic Designer & Illustrator</h2>

  <p>
  Hi, I’m Ecem. Graphic designer and illustrator with eight years of experience
  in visual storytelling and image-making. My professional focus includes visual
  identity, illustration, and concept-driven design.
  <br><br>
  I have experience in developing strong narratives through composition,
  typography, and character-based visuals, aiming to create designs that are
  intentional and conceptually grounded rather than purely decorative.
  <br><br>
  Throughout my career, I have built a distinctive visual language influenced by
  illustration, digital culture, and editorial aesthetics. I value clarity,
  consistency, and meaning in design, and I strive to produce visuals that
  communicate ideas with confidence and precision.
  <br><br>
  This portfolio represents my long-term dedication to graphic design and
  illustration as both a professional practice and a way of thinking.
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
    © 2026 SOLE
  </footer>
</div>

</body>
</html>