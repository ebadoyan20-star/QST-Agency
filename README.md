<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Pulse Studio — Digital Marketing & Experience</title>
  <meta name="description" content="Pulse Studio — digital marketing, experience design, paid media and analytics. Inspired creative agency template." />
  <style>
    :root{
      --bg:#081029;
      --card:#0e1a2b;
      --muted:#9fb0c8;
      --accent:#00d4ff;
      --accent2:#7c3aed;
      --glass: rgba(255,255,255,0.04);
      --radius:14px;
      --max-width:1200px;
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      color-scheme: dark;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      background: linear-gradient(180deg,#021028 0%, #071730 100%);
      color: #e8f4ff;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.45;
    }
    .container{max-width:var(--max-width);margin:0 auto;padding:28px}
    header{display:flex;align-items:center;justify-content:space-between;gap:12px}
    .brand{display:flex;align-items:center;gap:12px}
    .brand .logo{
      width:48px;height:48px;border-radius:10px;
      background:linear-gradient(135deg,var(--accent2),var(--accent));
      display:flex;align-items:center;justify-content:center;font-weight:800;color:#021028;
      box-shadow:0 6px 20px rgba(0,0,0,0.5);
    }
    nav{display:flex;gap:18px;align-items:center}
    nav a{color:var(--muted);text-decoration:none;font-weight:600;padding:8px;border-radius:8px}
    nav a:hover{color:var(--accent)}
    .btn-primary{background:linear-gradient(90deg,var(--accent),var(--accent2));padding:9px 14px;border-radius:10px;color:#021028;font-weight:800;text-decoration:none}
    .hero{
      display:grid;
      grid-template-columns: 1fr 420px;
      gap:28px;
      align-items:stretch;
      margin-top:26px;
    }
    .hero-card{
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border-radius:18px;
      padding:28px;
      box-shadow: 0 10px 40px rgba(2,6,23,0.6);
      position:relative;
      overflow:hidden;
    }
    .kicker{display:inline-block;background:rgba(255,255,255,0.04);padding:6px 10px;border-radius:999px;color:var(--muted);font-weight:700;margin-bottom:12px}
    h1{margin:6px 0 8px;font-size:34px;line-height:1.05}
    p.lead{color:var(--muted);margin:0 0 16px}
    .services-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-top:18px}
    .service{background:var(--card);padding:14px;border-radius:12px;border:1px solid rgba(255,255,255,0.02)}
    .service h4{margin:0 0 8px;font-size:15px}
    .service p{margin:0;color:var(--muted);font-size:13px}
    /* Right column */
    .visual{
      border-radius:14px;
      background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      padding:18px;
      display:flex;flex-direction:column;gap:12px;align-items:center;justify-content:center;
      min-height:360px;
    }
    .work-preview{width:100%;height:220px;border-radius:10px;background:linear-gradient(135deg,#072033,#14314a);display:flex;align-items:center;justify-content:center;color:var(--muted);font-weight:700}
    /* Featured case studies */
    .cases{margin-top:26px;display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
    .case{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:14px;border-radius:12px;border:1px solid rgba(255,255,255,0.02)}
    .case h3{margin:0 0 8px;font-size:16px}
    .case p{margin:0;color:var(--muted);font-size:13px}
    /* Insights strip */
    .insights{margin-top:26px;display:flex;gap:12px;overflow:hidden}
    .insight{min-width:300px;background:rgba(255,255,255,0.02);padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,0.02)}
    /* Footer */
    footer{margin-top:36px;color:var(--muted);display:flex;justify-content:space-between;align-items:center}
    /* small screens */
    @media (max-width:980px){
      .hero{grid-template-columns:1fr}
      .services-grid{grid-template-columns:repeat(2,1fr)}
      .cases{grid-template-columns:repeat(2,1fr)}
    }
    @media (max-width:560px){
      .services-grid{grid-template-columns:1fr}
      .cases{grid-template-columns:1fr}
      nav{display:none}
      header{justify-content:space-between}
    }
    /* subtle animated background shapes */
    .bg-shape{
      position:absolute;right:-80px;top:-40px;width:300px;height:300px;border-radius:50%;
      background:radial-gradient(circle at 30% 30%, rgba(124,58,237,0.28), rgba(0,212,255,0.12));
      filter:blur(40px);transform:scale(1.1);opacity:0.9;pointer-events:none;
    }
    /* accessible focus */
    a:focus, button:focus { outline:3px solid rgba(0,212,255,0.14); outline-offset:2px; }
  </style>
</head>
<body>
  <div class="container" role="document">
    <header>
      <div class="brand" aria-label="Brand">
        <div class="logo" aria-hidden="true">P</div>
        <div>
          <div style="font-weight:800">Pulse Studio</div>
          <div style="font-size:13px;color:var(--muted)">Digital experiences & growth</div>
        </div>
      </div>

      <nav aria-label="Main navigation">
        <a href="#services">Services</a>
        <a href="#work">Work</a>
        <a href="#insights">Insights</a>
        <a class="btn-primary" href="#contact">Contact</a>
      </nav>
    </header>

    <main>
      <section class="hero" aria-labelledby="hero-heading">
        <div class="hero-card">
          <span class="kicker">We build measurable growth</span>
          <h1 id="hero-heading">Crafting digital products & campaigns that move the needle</h1>
          <p class="lead">Strategy · Creative · Media · Analytics. We combine product thinking and performance to deliver sustainable results for ambitious brands.</p>
          <a class="btn-primary" href="#work" style="display:inline-block">See our work</a>

          <div class="services-grid" aria-hidden="false" style="margin-top:20px">
            <div class="service">
              <h4>Experience Design</h4>
              <p>UX / UI, prototyping and product strategy for customer-first experiences.</p>
            </div>
            <div class="service">
              <h4>Paid Media</h4>
              <p>Performance-driven campaigns across search and social with A/B testing.</p>
            </div>
            <div class="service">
              <h4>Creative & Content</h4>
              <p>Story-led assets and motion to elevate your voice across channels.</p>
            </div>
          </div>
        </div>

        <aside class="visual" aria-labelledby="visual-heading">
          <div class="bg-shape" aria-hidden="true"></div>
          <h2 id="visual-heading" style="margin:0 0 6px">Featured project</h2>
          <div class="work-preview" role="img" aria-label="Project preview">
            Project: Aurora — UX & Growth
          </div>
          <p style="margin:0;color:var(--muted);font-size:13px;text-align:center">A multi-channel launch that increased conversions by 37% in 6 months.</p>
        </aside>
      </section>

      <section id="work" aria-labelledby="work-heading">
        <h2 id="work-heading" style="margin-top:26px">Selected case studies</h2>
        <div class="cases">
          <article class="case" aria-labelledby="c1">
            <h3 id="c1">E-commerce replatform</h3>
            <p class="muted">Full redesign + CRO program that lifted average order value and reduced churn.</p>
          </article>
          <article class="case" aria-labelledby="c2">
            <h3 id="c2">Global product launch</h3>
            <p class="muted">End-to-end product marketing and digital PR that scaled reach worldwide.</p>
          </article>
          <article class="case" aria-labelledby="c3">
            <h3 id="c3">Brand refresh</h3>
            <p class="muted">New identity, voice and digital system for a B2B SaaS portfolio.</p>
          </article>
        </div>
      </section>

      <section id="insights" aria-labelledby="insights-heading">
        <h2 id="insights-heading" style="margin-top:26px">Insights</h2>
        <div class="insights" role="list">
          <div class="insight" role="listitem">
            <h4 style="margin:0 0 8px">How to structure high-performing campaigns</h4>
            <p class="muted" style="margin:0">Practical tips to improve ROAS and scale safely.</p>
          </div>
          <div class="insight" role="listitem">
            <h4 style="margin:0 0 8px">Design sprints for product teams</h4>
            <p class="muted" style="margin:0">Run a low-cost experiment to validate your next big feature.</p>
          </div>
          <div class="insight" role="listitem">
            <h4 style="margin:0 0 8px">Measurement & attribution</h4>
            <p class="muted" style="margin:0">Simple frameworks to connect marketing to business outcomes.</p>
          </div>
        </div>
      </section>

      <section id="services" aria-labelledby="services-heading">
        <h2 id="services-heading" style="margin-top:26px">Services</h2>
        <p class="muted">We offer modular services — pick what you need or choose a full retainer.</p>
        <div style="display:grid;grid-template-columns:1fr 320px;gap:14px;margin-top:12px">
          <div style="background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.00));padding:16px;border-radius:12px;">
            <h3 style="margin-top:0">Strategy & Planning</h3>
            <ul class="muted">
              <li>Audience research</li>
              <li>Roadmaps & KPIs</li>
              <li>Channel prioritization</li>
            </ul>

            <h3>Execution</h3>
            <ul class="muted">
              <li>Creative production</li>
              <li>Ad account management</li>
              <li>Optimization & reporting</li>
            </ul>
          </div>

          <aside style="background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.00));padding:16px;border-radius:12px;">
            <h4 style="margin:0 0 8px">Pricing starting at</h4>
            <div style="font-weight:800;font-size:20px">$2,500 / month</div>
            <p class="muted" style="margin-top:8px">Custom proposals based on scope, channels and goals.</p>
            <a class="btn-primary" href="#contact" style="margin-top:12px;display:inline-block">Request proposal</a>
          </aside>
        </div>
      </section>

      <section id="contact" aria-labelledby="contact-heading" style="margin-top:26px">
        <h2 id="contact-heading">Contact</h2>
        <div style="display:grid;grid-template-columns:1fr 320px;gap:14px;margin-top:12px">
          <form onsubmit="handleSubmit(event)" style="background:rgba(255,255,255,0.02);padding:14px;border-radius:12px;">
            <label style="display:block;font-size:13px;color:var(--muted)">Name</label>
            <input id="name" required style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:inherit" />
            <label style="display:block;font-size:13px;color:var(--muted);margin-top:10px">Email</label>
            <input id="email" type="email" required style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:inherit" />
            <label style="display:block;font-size:13px;color:var(--muted);margin-top:10px">Message</label>
            <textarea id="msg" rows="5" required style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:inherit"></textarea>
            <div style="display:flex;justify-content:flex-end;margin-top:10px">
              <button class="btn-primary" type="submit">Send message</button>
            </div>
            <p id="status" style="color:var(--muted);margin-top:8px"></p>
          </form>

          <aside style="background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.00));padding:14px;border-radius:12px;">
            <h4 style="margin:0 0 8px">Office</h4>
            <p class="muted" style="margin:0">Tallinn / Remote</p>
            <p class="muted" style="margin-top:8px">hello@pulselab.example</p>
          </aside>
        </div>
      </section>
    </main>

    <footer>
      <div>© <span id="yr"></span> Pulse Studio — digital experiences</div>
      <div class="muted">Built with accessibility and performance in mind</div>
    </footer>
  </div>

  <script>
    document.getElementById('yr').textContent = new Date().getFullYear();
    function handleSubmit(e){
      e.preventDefault();
      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      const msg = document.getElementById('msg').value.trim();
      const status = document.getElementById('status');
      if(!name || !email || !msg){ status.textContent = 'Please complete all fields.'; return; }
      status.textContent = 'Thanks! Your message was received (prototype).';
      e.target.reset();
      // Integrate with Formspree, Netlify Forms, or a backend endpoint to actually send the message.
    }

    // Small keyboard-accessible focus helper (trap mobile nav off-screen)
    (function(){
      // smooth scroll for internal links
      document.querySelectorAll('a[href^="#"]').forEach(a=>{
        a.addEventListener('click', e=>{
          e.preventDefault();
          const id = a.getAttribute('href').slice(1);
          if(!id) return;
          const el = document.getElementById(id);
          if(el) el.scrollIntoView({behavior:'smooth',block:'start'});
        });
      });
    })();
  </script>
</body>
</html>
