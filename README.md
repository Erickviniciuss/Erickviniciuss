## Erickviniciuss
<!DOCTYPE html><html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Pac-Man GitHub Banner</title>
  <style>
    body {
      margin: 0;
      background: #000;
      overflow: hidden;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      image-rendering: pixelated;
      font-family: monospace;
    }.banner {
  position: relative;
  width: 900px;
  height: 145px;
  background: #000;
  overflow: hidden;
  border: 4px solid #111;
}

.track {
  position: absolute;
  top: 50%;
  left: 0;
  width: 100%;
  height: 8px;
  transform: translateY(-50%);
  background: repeating-linear-gradient(
    to right,
    transparent 0,
    transparent 18px,
    #222 18px,
    #222 20px
  );
}

.dot {
  position: absolute;
  width: 8px;
  height: 8px;
  background: #fff5a5;
  border-radius: 50%;
  top: 50%;
  transform: translateY(-50%);
  box-shadow: 0 0 6px #fff5a5;
  animation: blink 0.8s infinite alternate;
}

@keyframes blink {
  from {
    opacity: 1;
  }
  to {
    opacity: 0.4;
  }
}

.pacman {
  position: absolute;
  width: 48px;
  height: 48px;
  background: #ffd800;
  border-radius: 50%;
  top: 50%;
  left: -60px;
  transform: translateY(-50%);
  animation: movePacman 12s linear infinite;
  image-rendering: pixelated;
}

.pacman::before {
  content: "";
  position: absolute;
  width: 0;
  height: 0;
  border-top: 12px solid transparent;
  border-bottom: 12px solid transparent;
  border-left: 24px solid #000;
  top: 0;
  right: 0;
  transform-origin: left center;
  animation: mouthTop 0.18s infinite alternate;
}

.pacman::after {
  content: "";
  position: absolute;
  width: 0;
  height: 0;
  border-top: 12px solid transparent;
  border-bottom: 12px solid transparent;
  border-left: 24px solid #000;
  bottom: 0;
  right: 0;
  transform-origin: left center;
  animation: mouthBottom 0.18s infinite alternate;
}

@keyframes mouthTop {
  from {
    transform: rotate(-40deg);
  }
  to {
    transform: rotate(-5deg);
  }
}

@keyframes mouthBottom {
  from {
    transform: rotate(40deg);
  }
  to {
    transform: rotate(5deg);
  }
}

@keyframes movePacman {
  from {
    left: -60px;
  }
  to {
    left: 960px;
  }
}

.ghost {
  position: absolute;
  width: 42px;
  height: 42px;
  border-radius: 20px 20px 6px 6px;
  top: 50%;
  transform: translateY(-50%);
  animation: moveGhost 12s linear infinite;
}

.ghost::before,
.ghost::after {
  content: "";
  position: absolute;
  background: white;
  width: 8px;
  height: 10px;
  border-radius: 50%;
  top: 10px;
}

.ghost::before {
  left: 10px;
}

.ghost::after {
  right: 10px;
}

.ghost.red {
  background: #ff2b2b;
  left: -140px;
  animation-delay: 1s;
}

.ghost.cyan {
  background: #00eaff;
  left: -240px;
  animation-delay: 2s;
}

.ghost.pink {
  background: #ff79d1;
  left: -340px;
  animation-delay: 3s;
}

@keyframes moveGhost {
  from {
    left: -100px;
  }
  to {
    left: 930px;
  }
}

.title {
  position: absolute;
  right: 25px;
  top: 50%;
  transform: translateY(-50%);
  color: #00ffcc;
  font-size: 24px;
  letter-spacing: 3px;
  text-shadow:
    0 0 6px #00ffcc,
    0 0 12px #00ffcc;
  z-index: 5;
}

.scanlines {
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    to bottom,
    rgba(255,255,255,0.04),
    rgba(255,255,255,0.04) 1px,
    transparent 1px,
    transparent 3px
  );
  pointer-events: none;
}

  </style>
</head>
<body>
  <div class="banner">
    <div class="track"></div><div class="pacman"></div>

<div class="ghost red"></div>
<div class="ghost cyan"></div>
<div class="ghost pink"></div>

<div class="title">ERICK DEV</div>

<div class="scanlines"></div>

  </div>  <script>
    const banner = document.querySelector('.banner');

    for (let i = 0; i < 35; i++) {
      const dot = document.createElement('div');
      dot.classList.add('dot');
      dot.style.left = `${40 + i * 24}px`;
      banner.appendChild(dot);
    }
  </script></body>
</html>
### 🤖 Linguagens e Tecnologias

<img 
    align="left" 
    alt="HTML"
    title="HTML" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" 
/>
<img 
    align="left" 
    alt="CSS" 
    title="CSS"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" 
/>
<img 
    align="left" 
    alt="JavaScript" 
    title="JavaScript"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" 
/>
<img 
    align="left" 
    alt="TypeScript"
    title="TypeScript" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" 
/>
<img 
    align="left" 
    alt="React"
    title="React" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/react/react-original.svg" 
/>
<img 
    align="left" 
    alt="Next.js" 
    title="Next.js"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nextjs/nextjs-original.svg" 
/>
<img 
    align="left" 
    alt="Bootstrap"
    title="Bootstrap" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/bootstrap/bootstrap-original.svg" 
/>
<img 
    align="left" 
    alt="Tailwind" 
    title="Tailwind"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg" 
/>
<img 
    align="left" 
    alt="SASS" 
    title="SASS"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/sass/sass-original.svg" 
/>
<img 
    align="left" 
    alt="PHP" 
    title="PHP"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/php/php-original.svg" 
/>
<img 
    align="left" 
    alt="Laravel" 
    title="Laravel"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/laravel/laravel-original.svg" 
/>
<img 
    align="left" 
    alt="JQuery" 
    title="JQuery"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/jquery/jquery-original.svg" 
/>
<img 
    align="left" 
    alt="Git" 
    title="Git"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg" 
/>
<img 
    align="left" 
    alt="Python" 
    title="Python"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" 
/>

<br/>
<br/>

### 📊 Estatísticas

<p>
  <img 
    align="left" 
    alt="GitHub Stats" 
    height="200" 
    style="padding-right: 10px;" 
    src="https://github-readme-stats.vercel.app/api?username=Larissakich&show_icons=true&theme=tokyonight&include_all_commits=true&locale=pt-br" 
  />

<img 
      align="left" 
      alt="GitHub Stats" 
      height="200" 
      src="https://github-readme-stats.vercel.app/api/top-langs/?username=larissakich&theme=tokyonight&layout=compact&custom_title=Tecnologias&langs_count=9" 
  />

</p>
