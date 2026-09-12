<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Noslid32 — Portafolio</title>
<style>
  :root{
    --bg: #0a0e12;
    --bg-panel: #10151b;
    --border: #22303c;
    --text: #d7dde3;
    --muted: #6f7f8c;
    --accent: #5eead4;
    --accent-dim: #2c7a70;
    --amber: #f5b942;
  }
  *{ box-sizing: border-box; }
  html,body{ margin:0; padding:0; }
  body{
    background: var(--bg);
    color: var(--text);
    font-family: 'JetBrains Mono','Fira Code',ui-monospace,SFMono-Regular,Consolas,monospace;
    font-size: 15px;
    line-height: 1.6;
  }
  a{ color: var(--accent); text-decoration: none; }
  a:hover{ text-decoration: underline; }
  a:focus-visible, button:focus-visible{ outline: 2px solid var(--accent); outline-offset: 3px; }

  .wrap{ max-width: 760px; margin: 0 auto; padding: 0 24px; }

  /* nav */
  header.nav{
    border-bottom: 1px solid var(--border);
    padding: 18px 0;
    position: sticky; top:0;
    background: rgba(10,14,18,0.9);
    backdrop-filter: blur(6px);
    z-index: 10;
  }
  .nav .wrap{ display:flex; justify-content: space-between; align-items:center; flex-wrap: wrap; gap:10px; }
  .brand{ color: var(--text); font-weight:700; }
  .brand .dot{ color: var(--accent); }
  .nav-links{ display:flex; gap:22px; font-size:14px; }
  .nav-links a{ color: var(--muted); }
  .nav-links a:hover{ color: var(--accent); }

  /* hero */
  .hero{ padding: 64px 0 40px; }
  .prompt-line{ color: var(--muted); font-size: 14px; margin-bottom: 6px; }
  .prompt-line .sym{ color: var(--accent); }
  h1{
    font-size: 30px;
    margin: 4px 0 4px;
    color: var(--text);
    font-weight: 700;
    letter-spacing: -0.3px;
  }
  .cursor{
    display:inline-block; width:9px; height:22px;
    background: var(--accent);
    margin-left:4px; vertical-align: -3px;
    animation: blink 1s steps(1) infinite;
  }
  @keyframes blink{ 50%{ opacity: 0; } }
  .tagline{ color: var(--amber); font-size: 15px; margin-bottom: 22px; }

  .terminal{
    background: var(--bg-panel);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 20px 22px;
    margin-top: 8px;
  }
  .terminal .line{ margin: 0 0 6px; }
  .terminal .out{ color: var(--text); }
  .terminal .cmd{ color: var(--accent); }
  .terminal .cmt{ color: var(--muted); }

  /* sections */
  section{ padding: 46px 0; border-top: 1px solid var(--border); }
  .sec-head{ display:flex; align-items:baseline; gap:10px; margin-bottom: 22px; }
  .sec-head .sym{ color: var(--accent); font-size: 15px; }
  .sec-head h2{ font-size: 18px; margin:0; color: var(--text); font-weight:700; }

  /* tech */
  .chip-row{ display:flex; flex-wrap: wrap; gap:10px; }
  .chip{
    border:1px solid var(--border);
    background: var(--bg-panel);
    color: var(--text);
    padding: 7px 13px;
    border-radius: 6px;
    font-size: 13px;
  }
  .chip .lvl{ color: var(--accent); }

  /* projects */
  .project{
    border: 1px solid var(--border);
    background: var(--bg-panel);
    border-radius: 8px;
    padding: 22px 24px;
    margin-bottom: 20px;
  }
  .project h3{ margin:0 0 6px; font-size: 16px; color: var(--text); }
  .project .lab{ color: var(--muted); font-size: 12.5px; margin-bottom: 12px; }
  .project p{ margin: 0 0 14px; color: var(--text); }
  .project ul{ margin: 0 0 14px; padding-left: 18px; color: var(--text); }
  .project li{ margin-bottom: 4px; }
  .tag-row{ display:flex; flex-wrap:wrap; gap:8px; margin-bottom: 14px; }
  .tag{
    font-size: 11.5px;
    color: var(--accent-dim);
    border: 1px solid var(--accent-dim);
    padding: 3px 9px;
    border-radius: 4px;
    color: var(--accent);
  }
  .link-row{ display:flex; gap:18px; font-size: 13.5px; }
  .link-row a::before{ content: "→ "; }

  /* contact */
  .contact-list{ list-style:none; padding:0; margin:0; }
  .contact-list li{ margin-bottom: 10px; }
  .contact-list .k{ color: var(--muted); display:inline-block; width: 90px; }

  footer{ padding: 30px 0 50px; color: var(--muted); font-size: 12.5px; }

  @media (max-width: 560px){
    h1{ font-size: 24px; }
    .terminal{ padding: 16px; }
    .nav-links{ gap:14px; }
  }
</style>
</head>
<body>

<header class="nav">
  <div class="wrap">
    <div class="brand">noslid32<span class="dot">.</span>dev</div>
    <nav class="nav-links">
      <a href="#tech">_tech</a>
      <a href="#projects">_projects</a>
      <a href="#contact">_contact</a>
    </nav>
  </div>
</header>

<main class="wrap">

  <section class="hero" style="border-top:none; padding-top:64px;">
    <div class="prompt-line"><span class="sym">$</span> whoami</div>
    <h1>Dilson Morales <span class="cursor"></span></h1>
    <div class="tagline">Estudiante de Ingeniería en Sistemas · Guatemala</div>

    <div class="terminal">
      <p class="line out"><span class="cmd">&gt;</span> cat me.txt</p>
      <p class="line out">Estudiante de 3er año de Ingeniería en Sistemas en la Universidad Galileo.</p>
      <p class="line out">Aprendiendo Java y Python, construyendo proyectos con React y bases de datos.</p>
      <p class="line cmt">// Maya K'iche' · cuando no estoy programando, ando subiendo de nivel en algún juego</p>
    </div>
  </section>

  <section id="tech">
    <div class="sec-head">
      <span class="sym">&gt;</span>
      <h2>_Tech</h2>
    </div>
    <div class="chip-row">
      <span class="chip">Java <span class="lvl">●●●</span></span>
      <span class="chip">Python <span class="lvl">●●●</span></span>
      <span class="chip">JavaScript <span class="lvl">●●●</span></span>
      <span class="chip">React <span class="lvl">●●</span></span>
      <span class="chip">Bootstrap <span class="lvl">●●</span></span>
      <span class="chip">Material-UI <span class="lvl">●●</span></span>
      <span class="chip">MySQL <span class="lvl">●●</span></span>
      <span class="chip">Git &amp; GitHub <span class="lvl">●●●</span></span>
    </div>
  </section>

  <section id="projects">
    <div class="sec-head">
      <span class="sym">&gt;</span>
      <h2>_Projects</h2>
    </div>

    <div class="project">
      <h3>Tic-Tac-Toe Plus</h3>
      <div class="lab">Lab 3 — Universidad Galileo</div>
      <p>Versión mejorada del clásico tres en raya construida en React, enfocada en la experiencia de usuario más que en reinventar la lógica del juego.</p>
      <ul>
        <li>Resalta el último movimiento realizado en el tablero</li>
        <li>Interfaz responsiva construida con Bootstrap</li>
        <li>Gestión de estado y arquitectura basada en componentes</li>
      </ul>
      <div class="tag-row">
        <span class="tag">React</span>
        <span class="tag">Bootstrap</span>
        <span class="tag">JavaScript</span>
      </div>
      <div class="link-row">
        <a href="https://github.com/Noslid32/Tic-Tac-Toe-Plus" target="_blank" rel="noopener">Código</a>
        <a href="https://5djtrf.csb.app/" target="_blank" rel="noopener">Demo en vivo</a>
      </div>
    </div>

    <div class="project">
      <h3>Survey — Encuesta con validación en tiempo real</h3>
      <div class="lab">Lab 5 — Universidad Galileo</div>
      <p>Formulario de encuesta estructurado que valida cada respuesta en tiempo real y no permite el envío hasta completar todos los campos requeridos.</p>
      <ul>
        <li>Al menos tres tipos de entrada: texto, correo y opción múltiple</li>
        <li>Barra de progreso dinámica según el avance del usuario</li>
        <li>Mensaje de éxito al finalizar el envío</li>
        <li>Componentes organizados en <code>src/components/</code></li>
      </ul>
      <div class="tag-row">
        <span class="tag">React</span>
        <span class="tag">Material-UI</span>
        <span class="tag">JavaScript</span>
      </div>
      <div class="link-row">
        <a href="https://github.com/Noslid32/Survey" target="_blank" rel="noopener">Código</a>
        <a href="https://xh34tx.csb.app/" target="_blank" rel="noopener">Demo en vivo</a>
      </div>
    </div>
  </section>

  <section id="contact">
    <div class="sec-head">
      <span class="sym">&gt;</span>
      <h2>_Contact</h2>
    </div>
    <ul class="contact-list">
      <li><span class="k">email</span> <a href="mailto:moralestajis23@gmail.com">moralestajis23@gmail.com</a></li>
      <li><span class="k">github</span> <a href="https://github.com/Noslid32" target="_blank" rel="noopener">github.com/Noslid32</a></li>
      <li><span class="k">phone</span> 4536-7948</li>
    </ul>
  </section>

</main>

<footer>
  <div class="wrap">
    Diseñado y construido por Dilson Morales · desplegado en Vercel
  </div>
</footer>

</body>
</html>
