
 
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Fern — Portfolio</title>
  <meta name="description" content="Fern — Computer Science student portfolio" />
  <meta name="theme-color" content="#ffe6f2" />
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;600&family=Nunito:wght@300;400;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0b0f14; /* deep dark */
      --card:#0f1720; /* slightly lighter */
      --accent1:#f7c7ec; /* soft pink */
      --accent2:#bfe8ff; /* soft blue */
      --muted:#a9b4bf;
      --glass: rgba(255,255,255,0.04);
      --radius:14px;
    }

    *{box-sizing:border-box}
    html,body{height:100%;}
    body{
      margin:0;
      font-family:Nunito, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background: radial-gradient(1200px 600px at 10% 10%, rgba(191,232,255,0.06), transparent),
                  radial-gradient(900px 400px at 90% 90%, rgba(247,199,236,0.06), transparent),
                  var(--bg);
      color:#eef2f6;
      display:flex;
      align-items:center;
      justify-content:center;
      padding:48px 20px;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    .container{
      width:100%;
      max-width:920px;
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border:1px solid rgba(255,255,255,0.03);
      border-radius:20px;
      padding:36px;
      box-shadow: 0 10px 30px rgba(3,6,10,0.7);
      backdrop-filter: blur(6px);
    }

    header{
      display:flex;
      gap:20px;
      align-items:center;
      justify-content:space-between;
      margin-bottom:28px;
    }

    .intro{
      display:flex;
      gap:18px;
      align-items:center;
    }

    .avatar{
      width:88px;
      height:88px;
      border-radius:18px;
      background: linear-gradient(135deg,var(--accent2),var(--accent1));
      display:flex;
      align-items:center;
      justify-content:center;
      font-weight:700;
      font-family:Montserrat, Nunito, sans-serif;
      color:#102027;
      box-shadow: 0 6px 18px rgba(183,173,222,0.08), inset 0 -6px 18px rgba(255,255,255,0.03);
      flex-shrink:0;
    }

    .title{
      line-height:1.05;
    }

    .title h1{
      margin:0;
      font-size:20px;
      font-weight:700;
      letter-spacing: -0.2px;
      color: #fff;
    }

    .title p{
      margin:4px 0 0 0;
      color:var(--muted);
      font-size:14px;
    }

    .heart{color:var(--accent1); margin-left:6px}

    /* floating pastel blobs for idol vibe */
    .blobs{
      position:relative;
      width:140px;height:64px;
    }

    .blob{
      position:absolute;
      border-radius:999px;
      filter: blur(18px);
      opacity:0.9;
      transform-origin:center;
      animation: float 6s ease-in-out infinite;
    }
    .blob.b1{width:72px;height:72px; left:12px; top:-6px; background:var(--accent2); animation-delay:0s}
    .blob.b2{width:56px;height:56px; right:6px; top:6px; background:var(--accent1); animation-delay:1.6s}

    @keyframes float{
      0%{ transform: translateY(0) scale(1)}
      50%{ transform: translateY(-10px) scale(1.03)}
      100%{ transform: translateY(0) scale(1)}
    }

    main{
      display:grid;
      grid-template-columns: 1fr 320px;
      gap:28px;
      align-items:start;
    }

    .card{
      background:var(--card);
      border-radius:var(--radius);
      padding:22px;
      border:1px solid rgba(255,255,255,0.02);
    }

    .section-title{
      display:flex;align-items:center;gap:12px;margin-bottom:12px;
    }
    .section-title h2{margin:0;font-size:16px;font-weight:600;color:#fff}
    .section-title .dot{width:10px;height:10px;border-radius:50%;background:linear-gradient(135deg,var(--accent1),var(--accent2));box-shadow:0 6px 20px rgba(191,232,255,0.06)}

    /* About */
    .about p{color:var(--muted);margin:0;font-size:15px;line-height:1.6}

    /* Tech tags */
    .tags{display:flex;flex-wrap:wrap;gap:10px}
    .tag{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); padding:8px 14px;border-radius:14px;font-weight:600;border:1px solid rgba(255,255,255,0.03);color:#fff;font-size:13px}

    /* Connect */
    .connect a{
      display:inline-block;padding:10px 14px;border-radius:12px;background:linear-gradient(90deg,var(--accent2),var(--accent1));color:#08212a;text-decoration:none;font-weight:700;border: none;box-shadow: 0 8px 20px rgba(183,173,222,0.06);
    }

    /* footer */
    .foot{margin-top:20px;text-align:center;color:var(--muted);font-size:13px}

    /* Responsive */
    @media (max-width:880px){
      main{grid-template-columns:1fr;}
      header{flex-direction:column;align-items:flex-start}
    }

  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="intro">
        <div class="avatar">F</div>
        <div class="title">
          <h1>Hello my name is <strong>Chayanid</strong>
            <span class="heart">❤️</span>
          </h1>
          <p>Call me <strong>Fern</strong> — I study Computer Science at the University of Phayao</p>
        </div>
      </div>

      <div class="blobs" aria-hidden="true">
        <div class="blob b1"></div>
        <div class="blob b2"></div>
      </div>
    </header>

    <main>
      <section class="card about">
        <div class="section-title"><div class="dot"></div><h2>About Me</h2></div>
        <p>
          Hello my name is Fern ❤️<br>
          I study Computer Science at the University of Phayao.
        </p>

        <div class="foot">Minimal, pastel-kawaii aesthetic — inspired by K‑pop idol color palettes.</div>
      </section>

      <aside>
        <div class="card">
          <div class="section-title"><div class="dot"></div><h2>Tech Stack</h2></div>
          <div class="tags">
            <div class="tag">Python</div>
            <div class="tag">Figma</div>
          </div>
        </div>

        <div style="height:18px"></div>

        <div class="card">
          <div class="section-title"><div class="dot"></div><h2>Connect</h2></div>
          <a href="e-mail:67092318@up.ac.th">Email</a>
        </div>
      </aside>
    </main>
  </div>
</body>
</html>

   
