<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>ECEM 夜黒</title>

<style>
*{margin:0;padding:0;box-sizing:border-box}

body{
  height:100vh;
  background:
    repeating-linear-gradient(
      180deg,
      rgba(0,0,0,.9) 0px,
      rgba(0,0,0,.9) 2px,
      rgba(5,10,30,.95) 4px
    ),
    linear-gradient(120deg,#000,#02030a,#010214);
  font-family: 'Arial', sans-serif;
  color:#0a0f2a;
  overflow:hidden;
}

/* JAPANESE NOISE */
.noise{
  position:fixed;
  inset:0;
  background-image:url("https://grainy-gradients.vercel.app/noise.svg");
  opacity:.15;
  z-index:10;
  pointer-events:none;
}

/* FLOATING KANJI */
.kanji{
  position:absolute;
  color:#05081a;
  font-size:5rem;
  font-weight:900;
  writing-mode:vertical-rl;
  opacity:.7;
  animation:float 20s linear infinite;
}
@keyframes float{
  from{transform:translateY(120vh)}
  to{transform:translateY(-140vh)}
}

/* SHARDS */
.shard{
  position:absolute;
  width:200px;
  height:200px;
  border:1px solid rgba(10,20,60,.8);
  transform:rotate(45deg);
  opacity:.4;
  animation:spin 60s linear infinite;
}
@keyframes spin{
  from{transform:rotate(0deg)}
  to{transform:rotate(360deg)}
}

/* CENTER CORE */
.core{
  position:absolute;
  top:50%;
  left:50%;
  transform:translate(-50%,-50%);
  text-align:center;
  z-index:5;
}

h1{
  font-size:6rem;
  letter-spacing:6px;
  color:#02061a;
  text-shadow:
    0 0 40px rgba(0,0,40,.9),
    0 0 120px rgba(0,0,80,.9);
}

h2{
  margin-top:20px;
  font-size:1.2rem;
  letter-spacing:8px;
  color:#030720;
}

p{
  margin-top:60px;
  max-width:720px;
  line-height:2.2;
  font-size:1.05rem;
  color:#02061f;
}

/* BUTTONS */
.links{
  margin-top:90px;
  display:flex;
  justify-content:center;
  gap:50px;
}

a{
  text-decoration:none;
  color:#030720;
  padding:22px 60px;
  border:1px solid rgba(10,20,80,.8);
  letter-spacing:5px;
  transition:.6s;
}
a:hover{
  background:#02061a;
  box-shadow:
    0 0 40px rgba(0,0,80,1),
    0 0 140px rgba(0,0,120,1);
  transform:scale(1.15) rotate(-2deg);
}

/* DARK PULSE */
.pulse{
  position:fixed;
  inset:0;
  background:radial-gradient(circle, rgba(0,0,60,.15), transparent 70%);
  animation:pulse 8s infinite alternate;
  z-index:2;
}
@keyframes pulse{
  from{opacity:.2}
  to{opacity:.6}
}
</style>
</head>

<body>

<div class="pulse"></div>
<div class="noise"></div>

<!-- KANJI CHAOS -->
<div class="kanji" style="left:10%;animation-duration:28s;">夜</div>
<div class="kanji" style="left:30%;animation-duration:24s;">影</div>
<div class="kanji" style="left:55%;animation-duration:32s;">黒</div>
<div class="kanji" style="left:75%;animation-duration:26s;">夢</div>

<!-- SHARDS -->
<div class="shard" style="top:10%;left:15%"></div>
<div class="shard" style="bottom:20%;right:20%"></div>

<div class="core">
  <h1>ECEM</h1>
  <h2>GRAPHIC DESIGNER · ILLUSTRATOR</h2>

  <p>
    Graphic designer and illustrator with eight years of experience in visual
    storytelling and image-making. Focused on visual identity, illustration,
    and concept-driven design rooted in narrative, restraint, and intention.
    <br><br>
    Influenced by Japanese visual culture, darkness, silence, editorial systems,
    and controlled chaos. Design as ritual. Image as language.
  </p>

  <div class="links">
    <a href="https://www.behance.net/ecemnurkahrman" target="_blank">PORTFOLIO</a>
    <a href="mailto:gwem1720@gmail.com">CONTACT</a>
  </div>
</div>

</body>
</html>