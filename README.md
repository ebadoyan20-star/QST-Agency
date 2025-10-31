<!--
Marketing agency single-file website (Armenian)
Save as: marketing-index.html
Features:
 - Home (հիմնական)
 - Services (ծառայությունների տեսակներ)
 - Pricing (գներ)
 - Contact form (խնդիր: form is prototype — connect to backend or Formspree)

To deploy: GitHub Pages / Netlify / Vercel
-->
<!doctype html>
<html lang="hy">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>Մարկետինգային Ծառայություններ — Ձեր Բրենդը Մեծացնելու Ամպլիֆիկատոր</title>
  <meta name="description" content="Միջին և փոքր բիզնեսների համար մարկետինգային ծառայություններ՝ բրենդինգ, սոց.մեդիա, խթանում և վեբ գովազդ. պարզ գներ և ծառայություններ">
  <style>
    :root{--bg:#ffffff;--text:#0f1724;--muted:#6b7280;--accent:#2563eb;--card:#f8fafc}
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter, system-ui, Arial;line-height:1.5;color:var(--text);background:linear-gradient(180deg,#fbfdff, #f1f5f9)}
    .wrap{max-width:1100px;margin:28px auto;padding:20px}
    header{display:flex;align-items:center;justify-content:space-between;gap:12px}
    .logo{font-weight:800;color:var(--accent)}
    nav a{margin-left:14px;text-decoration:none;color:var(--muted);font-weight:600}
    nav a.primary{background:var(--accent);color:white;padding:8px 12px;border-radius:10px}

    .hero{display:flex;gap:20px;align-items:center;margin-top:20px}
    .hero .left{flex:1}
    .hero h1{margin:0;font-size:28px}
    .hero p{color:var(--muted)}
    .cta{display:inline-block;padding:10px 14px;background:var(--accent);color:white;border-radius:10px;text-decoration:none;margin-top:12px}

    .cards{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin-top:18px}
    .card{background:var(--card);padding:16px;border-radius:12px}
    .card h4{margin:0 0 8px}
    .tag{display:inline-block;padding:6px 8px;border-radius:8px;background:#eef2ff;color:#3730a3;font-weight:700;font-size:13px}

    section{margin-top:26px}
    .services-list{display:grid;grid-template-columns:1fr 1fr;gap:12px}
    .service{background:white;padding:14px;border-radius:10px;border:1px solid #eef2ff}

    .pricing{display:grid;grid-template-columns:repeat(3,1fr);gap:12px}
    .price{background:white;padding:16px;border-radius:12px;border:1px solid #e6eef8}
    .price h3{margin:0}
    .price .cost{font-size:22px;font-weight:800;margin-top:6px}
    .price ul{margin:12px 0 0;padding-left:18px;color:var(--muted)}

    .contact{display:grid;grid-template-columns:1fr 360px;gap:18px}
    form input, form textarea{width:100%;padding:10px;margin-top:6px;border-radius:8px;border:1px solid #e6eef8}
    .muted{color:var(--muted)}

    footer{margin-top:26px;padding-top:12px;border-top:1px solid #eef2ff;color:var(--muted);font-size:14px}

    @media (max-width:900px){.cards{grid-template-columns:1fr 1fr}.pricing{grid-template-columns:1fr 1fr}.contact{grid-template-columns:1fr}}
    @media (max-width:520px){.cards{grid-template-columns:1fr}.hero{flex-direction:column}.pricing{grid-template-columns:1fr}}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="logo">BrandLift</div>
      <nav aria-label="Navigation">
        <a href="#home">Մեր մասին</a>
        <a href="#services">Ծառայություններ</a>
        <a href="#pricing">Գներ</a>
        <a class="primary" href="#contact">Կապ</a>
      </nav>
    </header>

    <main id="home">
      <section class="hero">
        <div class="left">
          <h1>Բարձրացնենք ձեր բրենդի տեսանելիությունը  և հաճախորդների ներգրավվածությունը</h1>
          <p class="muted">Մենք առաջարկում ենք ամբողջական մարքեթինգային փաթեթներ՝ սոցիալական մեդիա, կոնտենտ, գովազդ, և վերլուծություն՝ փոքր և միջին բիզնեսի համար:</p>
          <a class="cta" href="#contact">Անգամ հիմա կապվել</a>

          <div class="cards" aria-hidden="false">
            <div class="card">
              <div class="tag">Մասնագիտացված</div>
              <h4>Տարածածքային մենեջմենթ</h4>
              <p class="muted">Հագեցած ռազմավարություն՝ ձեր նպատակային լսարանին հասցնելու համար:</p>
            </div>
            <div class="card">
              <div class="tag">Արդյունքասեր</div>
              <h4>Խթանում & գովազդ</h4>
              <p class="muted">Paid search & social համար ժամանակակից մոտեցումներ:</p>
            </div>
            <div class="card">
              <div class="tag">Հասանելի</div>
              <h4>Արշավների հաշվետվություն</h4>
              <p class="muted">Մաքուր, թարգմանելի մետրիկներ՝ ROI-ի չափման համար:</p>
            </div>
          </div>
        </div>
        <div class="illustration">
          <!-- Placeholder svg -->
          <svg width="260" height="200" viewBox="0 0 260 200" fill="none" xmlns="http://www.w3.org/2000/svg" style="border-radius:12px;background:linear-gradient(180deg,#eef2ff,#fff)">
            <rect width="260" height="200" rx="12" fill="#fff"/>
            <text x="20" y="40" fill="#1f2937" font-size="20" font-weight="700">BrandLift</text>
            <text x="20" y="72" fill="#6b7280" font-size="13">Growth-focused marketing</text>
          </svg>
        </div>
      </section>

      <section id="services">
        <h2>Ծառայությունների տեսակներ</h2>
        <p class="muted">Մենք հարմարեցնում ենք ծառայությունները ըստ ձեր բյուջեի և բիզնեսի նպատակների:</p>
        <div class="services-list">
          <div class="service">
            <h4>Սոց․ մեդիա մենեջմենթ</h4>
            <p class="muted">Պլանավորում, կոնտենտ, weekly հրապարակումներ, և համայնքի հետ աշխատանք:</p>
            <strong>Ներառում է:</strong>
            <ul>
              <li>Պոստեր ամսական 8-12</li>
              <li>Վիզուալ և copywriting</li>
              <li>Համայնքային մոդերացիա</li>
            </ul>
          </div>

          <div class="service">
            <h4>Միջֆունկցիոնալ գովազդ (Ads)</h4>
            <p class="muted">Facebook/Instagram/Google Ads՝ conversion-ների համար օպտիմալացված:</p>
            <strong>Ներառում է:</strong>
            <ul>
              <li>Կամպեյնների ստեղծում և կառավարում</li>
              <li>Ա/B թեստավորում</li>
              <li>Արդյունքների հաշվետվություններ</li>
            </ul>
          </div>

          <div class="service">
            <h4>SEO & Տեղական SEO</h4>
            <p class="muted">Բովանդակության օպտիմիզացում և տեխնիկական աուդիտ:</p>
            <ul>
              <li>Կայքի արագության և on-page օպտիմիզացիա</li>
              <li>Keywords ռազմավարություն</li>
            </ul>
          </div>

          <div class="service">
            <h4>Բրենդինգ և վեբ դիզայն</h4>
            <p class="muted">Բրենդայդենթիթի ստեղծում, լոգո և կայքի սահմանում:</p>
            <ul>
              <li>Logo & color system</li>
              <li>Landing page (1-3 էջ)</li>
            </ul>
          </div>
        </div>
      </section>

      <section id="pricing">
        <h2>Գներ (պայմ)</h2>
        <p class="muted">Սա օրինակային գներ են՝ կարող ենք կազմել վեց-ընթաց՝ ըստ կոնկրետ պահանջների:</p>
        <div class="pricing">
          <div class="price">
            <h3>Սկսնակ</h3>
            <div class="cost">$300 / ամսական</div>
            <ul>
              <li>Սոց․մեդիա՝ 8 պոստ/ամիս</li>
              <li>Անվճար խորհրդատվություն՝ 1 ժամ</li>
              <li>Աշխատանքի հաշվետվություն՝ ամսական</li>
            </ul>
            <div style="margin-top:10px"><a class="cta" href="#contact">Ընդայմ</a></div>
          </div>

          <div class="price">
            <h3>Պրոֆ</h3>
            <div class="cost">$700 / ամսական</div>
            <ul>
              <li>Սոց․մեդիա՝ 16 պոստ/ամիս</li>
              <li>Ads բյուջետ + կառավարում</li>
              <li>A/B թեստավորում</li>
            </ul>
            <div style="margin-top:10px"><a class="cta" href="#contact">Ընդգրկվել</a></div>
          </div>

          <div class="price">
            <h3>Բիզնես</h3>
            <div class="cost">Մասնագիտական առաջարկ</div>
            <ul>
              <li>Ամբողջական growth փաթեթ</li>
              <li>Custom KPI-ներ և SLA</li>
              <li>Միանորդային աջակցություն</li>
            </ul>
            <div style="margin-top:10px"><a class="cta" href="#contact">Հետադարձ կապ</a></div>
          </div>
        </div>
      </section>

      <section id="contact">
        <h2>Կապ</h2>
        <div class="contact">
          <div>
            <p class="muted">Ուղարկեք հակիրճ հաղորդագրություն — կամ գրեք մեզ՝ hello@brandlift.example</p>
            <form onsubmit="handleSubmit(event)">
              <label>Անուն</label>
              <input id="name" required placeholder="Ձեր անունը">

              <label>Էլ․ փոստ</label>
              <input id="email" type="email" required placeholder="name@example.com">

              <label>Ծառայություն (պայման)</label>
              <select id="service">
                <option>Սոց.մեդիա</option>
                <option>Ads</option>
                <option>SEO</option>
                <option>Բրենդինգ</option>
              </select>

              <label>Հաղորդագրություն</label>
              <textarea id="message" rows="5" required placeholder="Ինչն եք ուզում հասնել..."></textarea>

              <div style="margin-top:10px;display:flex;gap:10px;justify-content:flex-end">
                <button class="cta" type="submit">Ուղարկել</button>
              </div>
              <p id="status" class="muted" style="margin-top:8px"></p>
            </form>
          </div>

          <aside style="background:#fff;padding:14px;border-radius:10px;border:1px solid #eef2ff">
            <h4>Մեր տվյալները</h4>
            <p class="muted">Երևան, Հայաստան<br>+374 99 123456<br>hello@brandlift.example</p>
            <p class="muted">Նշում. Անկյունային փաթեթների գները կարող են տարբեր լինել՝ ըստ ճանապարհորդության և հատուկ աշխատատեղի պահանջների:</p>
          </aside>
        </div>
      </section>

    </main>

    <footer>
      <div>© <span id="year"></span> BrandLift — Մարկետինգային ծառայություններ</div>
      <div class="muted">Կայքը պատրաստվել է արագ պրոտոտիպի համար — GitHub Pages/Netlify հեշտ տեղադրում</div>
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
    function handleSubmit(e){
      e.preventDefault();
      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      const message = document.getElementById('message').value.trim();
      const status = document.getElementById('status');
      if(!name || !email || !message){ status.textContent='Խնդրում ենք լրացնել բոլոր դաշտերը.'; return; }
      status.textContent = 'Շնորհակալություն! Ձեր խնդրանքը ուղարկվել է (փրոտոտիպ).';
      e.target.reset();
      // To send real emails, integrate with Formspree/Netlify Forms or your backend
    }
  </script>
</body>
</html>
