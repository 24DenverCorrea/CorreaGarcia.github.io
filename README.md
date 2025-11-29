# CorreaGarcia.github.io

<h1>WELCOME</h1>
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Your Name — Portfolio</title>
  <meta name="description" content="Simple, modern portfolio template." />
  <link rel="preconnect" href="https://fonts.gstatic.com">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#94a3b8; --accent:#7c3aed;
      --glass: rgba(255,255,255,0.04);
      font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{margin:0;background:linear-gradient(180deg,#071124 0%, var(--bg) 100%);color:#e6eef8;line-height:1.5}
    .container{max-width:1100px;margin:48px auto;padding:0 20px}

    /* Header */
    header{display:flex;align-items:center;justify-content:space-between;margin-bottom:28px}
    .brand{display:flex;gap:14px;align-items:center}
    .logo{width:56px;height:56px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#06b6d4);display:flex;align-items:center;justify-content:center;font-weight:700;color:#fff}
    nav a{margin-left:18px;color:var(--muted);text-decoration:none;font-weight:600}
    nav a:hover{color:#fff}

    /* Hero */
    .hero{display:grid;grid-template-columns:1fr 360px;gap:28px;align-items:center;margin-bottom:36px}
    .intro h1{margin:0;font-size:clamp(28px,4vw,44px)}
    .intro p{color:var(--muted);margin-top:10px}
    .cta{margin-top:18px}
    .btn{background:var(--accent);border:none;padding:10px 16px;border-radius:10px;color:#fff;font-weight:600;cursor:pointer}
    .profile{background:var(--glass);padding:18px;border-radius:14px;display:flex;flex-direction:column;gap:14px;align-items:center}
    .avatar{width:160px;height:160px;border-radius:12px;background:linear-gradient(135deg,#111827,#334155);display:flex;align-items:center;justify-content:center;font-size:40px;color:#fff}
    .small{color:var(--muted);font-size:14px}

    /* Sections */
    section{margin-bottom:34px}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);padding:20px;border-radius:12px}

    /* Projects grid */
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:14px}
    .project{padding:14px;border-radius:10px;background:linear-gradient(180deg,#071428 0%, #071525 60%)}
    .project h3{margin:0 0 8px 0;font-size:16px}
    .project p{margin:0;color:var(--muted);font-size:14px}
    .tags{margin-top:10px;display:flex;gap:8px;flex-wrap:wrap}
    .tag{font-size:12px;padding:6px 8px;background:rgba(255,255,255,0.03);border-radius:999px;color:var(--muted)}

    /* Skills */
    .skills{display:flex;gap:12px;flex-wrap:wrap}
    .skill{min-width:150px}
    .bar{height:10px;background:rgba(255,255,255,0.06);border-radius:999px;overflow:hidden}
    .bar > i{display:block;height:100%;background:linear-gradient(90deg,var(--accent),#06b6d4)}

    /* Contact */
    .contact-form{display:grid;grid-template-columns:1fr 1fr;gap:12px}
    input,textarea{width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.06);background:transparent;color:inherit}
    textarea{min-height:110px}

    footer{padding:24px 0;text-align:center;color:var(--muted)}

    /* Responsive */
    @media (max-width:900px){
      .hero{grid-template-columns:1fr}
      .grid{grid-template-columns:repeat(2,1fr)}
    }
    @media (max-width:600px){
      nav a{display:none}
      .grid{grid-template-columns:1fr}
      .contact-form{grid-template-columns:1fr}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">YN</div>
        <div>
          <div style="font-weight:700">Your Name</div>
          <div class="small">Frontend Developer • Designer</div>
        </div>
      </div>
      <nav>
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <main>
      <section class="hero">
        <div class="intro card">
          <h1>Hi, I’m <span style="color:var(--accent)">Your Name</span>. I build beautiful web experiences.</h1>
          <p>I’m a frontend developer who focuses on accessible, performant interfaces and delightful UX. I also design and ship complete projects from idea to production.</p>
          <div class="cta">
            <a class="btn" href="#contact">Work with me</a>
          </div>
          <div style="margin-top:18px;color:var(--muted);font-size:14px">Single-sentence purpose: showcase my work & skills to potential clients/employers.</div>
        </div>

        <aside class="profile">
          <div class="avatar">YN</div>
          <div style="text-align:center">
            <div style="font-weight:700">Your Name</div>
            <div class="small">Based in Manila • Open to remote</div>
          </div>
          <div style="width:100%">
            <div style="display:flex;justify-content:space-between;font-size:13px;color:var(--muted)"><span>Experience</span><strong>3 yrs</strong></div>
            <div style="height:8px;background:rgba(255,255,255,0.06);border-radius:8px;margin-top:8px;overflow:hidden"><i style="width:65%;display:block;height:100%;background:linear-gradient(90deg,var(--accent),#06b6d4)"></i></div>
          </div>
        </aside>
      </section>

      <section id="about">
        <div class="card">
          <h2 style="margin-top:0">About</h2>
          <p class="small">I turn ideas into polished websites and apps. I love writing clean code, crafting pixel-perfect UI, and optimizing performance. Outside of work I enjoy pixel art and indie games.</p>
        </div>
      </section>

      <section id="projects">
        <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:8px">
          <h2 style="margin:0">Projects</h2>
          <div class="small">Featured work — clickable demos recommended</div>
        </div>
        <div class="grid">
          <article class="project">
            <h3>Project One</h3>
            <p>Responsive marketing site with CMS integration and fast load times.</p>
            <div class="tags"><span class="tag">HTML</span><span class="tag">CSS</span><span class="tag">Netlify</span></div>
          </article>

          <article class="project">
            <h3>Project Two</h3>
            <p>SPA dashboard for analytics with charts and export features.</p>
            <div class="tags"><span class="tag">React</span><span class="tag">Chart.js</span><span class="tag">API</span></div>
          </article>

          <article class="project">
            <h3>Project Three</h3>
            <p>E-commerce frontend optimized for conversions and accessibility.</p>
            <div class="tags"><span class="tag">Vue</span><span class="tag">Stripe</span><span class="tag">A11y</span></div>
          </article>
        </div>
      </section>

      <section id="skills">
        <h2 style="margin-bottom:8px">Skills</h2>
        <div class="card">
          <div class="skills">
            <div class="skill">
              <strong>HTML & CSS</strong>
              <div class="bar" style="margin-top:8px"><i style="width:92%"></i></div>
            </div>
            <div class="skill">
              <strong>JavaScript</strong>
              <div class="bar" style="margin-top:8px"><i style="width:80%"></i></div>
            </div>
            <div class="skill">
              <strong>React / Vue</strong>
              <div class="bar" style="margin-top:8px"><i style="width:72%"></i></div>
            </div>
            <div class="skill">
              <strong>Design & Prototyping</strong>
              <div class="bar" style="margin-top:8px"><i style="width:68%"></i></div>
            </div>
          </div>
        </div>
      </section>

      <section id="contact">
        <h2>Contact</h2>
        <div class="card">
          <form class="contact-form" action="mailto:your.email@example.com" method="post" enctype="text/plain">
            <input type="text" name="name" placeholder="Your name" required>
            <input type="email" name="email" placeholder="Your email" required>
            <textarea name="message" placeholder="Message"></textarea>
            <div style="grid-column:1/-1;display:flex;gap:8px;justify-content:flex-end">
              <button type="reset" class="btn" style="background:transparent;border:1px solid rgba(255,255,255,0.06);">Reset</button>
              <button type="submit" class="btn">Send</button>
            </div>
          </form>
        </div>
      </section>
    </main>

    <footer>
      <div class="small">© <span id="year"></span> Your Name — Designed & built by you.</div>
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
    // Smooth scroll for anchors
    document.querySelectorAll('a[href^="#"]').forEach(a=>a.addEventListener('click',e=>{e.preventDefault();const t=document.querySelector(a.getAttribute('href')); if(t) t.scrollIntoView({behavior:'smooth',block:'start'});}));
  </script>
</body>
</html>
