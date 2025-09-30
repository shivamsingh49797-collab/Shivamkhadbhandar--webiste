# Shivamkhadbhandar--webiste
Website for shivam khad bhandar
<!doctype html>

<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Shivam Khad Bhandar – Fertilizers • Pesticides • Seeds</title>
  <meta name="description" content="Shivam Khad Bhandar – Fertilizers, pesticides, and quality seeds. Call, WhatsApp, or browse our product catalog." />  <!-- Open Graph -->  <meta property="og:title" content="Shivam Khad Bhandar" />
  <meta property="og:description" content="Fertilizers • Pesticides • Seeds" />
  <meta property="og:type" content="website" />
  <meta property="og:image" content="/og-image.jpg" />  <!-- Theme -->  <meta name="theme-color" content="#1b5e20" />  <style>
    :root{
      --green-900:#0f3d1a; /* very dark */
      --green-800:#1b5e20; /* primary */
      --green-700:#2e7d32;
      --green-200:#c8e6c9;
      --sage-50:#f3f6f3;
      --sand-100:#efe9db;
      --ink:#162117;
      --muted:#5b6b5f;
      --radius:18px;
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0; font-family:system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, Noto Sans, Arial, "Apple Color Emoji", "Segoe UI Emoji";
      color:var(--ink); background:var(--sage-50);
    }
    a{color:inherit; text-decoration:none}
    img{max-width:100%; display:block}

    /* Container */
    .container{width:min(1080px, 92vw); margin-inline:auto}

    /* Nav */
    header{position:sticky; top:0; z-index:40; background:linear-gradient(180deg, rgba(255,255,255,0.9), rgba(255,255,255,0.75)); backdrop-filter:saturate(1.2) blur(6px); border-bottom:1px solid #e6efe7}
    .nav{display:flex; align-items:center; justify-content:space-between; gap:16px; padding:12px 0}
    .brand{display:flex; align-items:center; gap:12px}
    .logo{width:44px; height:44px; border-radius:50%; background:radial-gradient(circle at 30% 30%, var(--green-200), var(--green-700)); border:2px solid white; box-shadow:0 2px 6px rgba(0,0,0,.08)}
    .brand h1{font-size:1.1rem; line-height:1.1; margin:0}
    .brand small{display:block; color:var(--muted)}
    .nav-links{display:flex; gap:18px}
    .nav-links a{padding:10px 12px; border-radius:10px; font-weight:600}
    .nav-links a:hover{background:#e9f3ea}

    /* Hero */
    .hero{position:relative; isolation:isolate; background:linear-gradient(120deg, var(--sand-100), #e7f2e7 60%); overflow:hidden}
    .hero::after{content:""; position:absolute; inset:auto -10% -40% -10%; height:50vh; background:radial-gradient(70% 60% at 50% 0%, rgba(46,125,50,.18), rgba(27,94,32,.06) 60%, transparent 70%); z-index:-1}
    .hero-inner{display:grid; grid-template-columns:1.15fr .85fr; gap:28px; padding:64px 0}
    @media (max-width:900px){.hero-inner{grid-template-columns:1fr; padding:40px 0}}
    .title{font-size:clamp(2rem, 4.5vw, 3.5rem); line-height:1.05; margin:0 0 10px}
    .tagline{font-size:clamp(1rem, 2.2vw, 1.25rem); color:var(--muted)}
    .cta-row{display:flex; flex-wrap:wrap; gap:12px; margin-top:18px}
    .btn{display:inline-flex; align-items:center; gap:10px; padding:12px 16px; border-radius:999px; font-weight:700; border:1px solid transparent; transition:transform .06s ease, box-shadow .2s}
    .btn:active{transform:translateY(1px)}
    .btn.primary{background:var(--green-800); color:white; box-shadow:0 6px 16px rgba(27,94,32,.18)}
    .btn.primary:hover{background:var(--green-700)}
    .btn.ghost{background:white; border-color:#dfe9e1}

    .hero-card{background:white; border:1px solid #e7efe8; border-radius:var(--radius); padding:18px; box-shadow:0 12px 24px rgba(16,40,22,.05)}
    .hero-card h3{margin:0 0 8px}
    .hero-list{display:grid; grid-template-columns:repeat(2, minmax(0,1fr)); gap:12px}
    .hero-pill{display:flex; align-items:center; gap:10px; border:1px dashed #dfe9e1; padding:10px 12px; border-radius:12px; background:#fbfdfb}

    /* Section */
    section{padding:56px 0}
    .section-title{font-size:1.6rem; margin:0 0 12px}
    .section-sub{color:var(--muted); margin:0 0 24px}

    /* Products */
    .grid{display:grid; grid-template-columns:repeat(12, 1fr); gap:18px}
    .card{grid-column:span 4; background:white; border:1px solid #e7efe8; border-radius:16px; overflow:hidden; display:flex; flex-direction:column; transition:transform .12s ease, box-shadow .2s}
    .card:hover{transform:translateY(-3px); box-shadow:0 14px 28px rgba(12,32,18,.08)}
    .card img{aspect-ratio:4/3; object-fit:cover}
    .card-body{padding:14px 14px 16px}
    .price{font-weight:800}
    .meta{color:var(--muted); font-size:.92rem}
    @media (max-width:1000px){.card{grid-column:span 6}}
    @media (max-width:640px){.card{grid-column:span 12}}

    /* Contact */
    .contact{display:grid; grid-template-columns:1.1fr .9fr; gap:24px}
    @media (max-width:900px){.contact{grid-template-columns:1fr}}
    .contact-card{background:white; border:1px solid #e7efe8; border-radius:var(--radius); padding:18px}
    .contact-list{display:grid; gap:10px; margin:0; padding:0; list-style:none}
    .contact-list a{display:flex; align-items:center; gap:10px; padding:10px 12px; border:1px solid #e7efe8; border-radius:12px; background:#fbfdfb}

    /* Footer */
    footer{background:var(--green-900); color:#e9f7ea; margin-top:28px}
    .foot{display:grid; grid-template-columns:1.2fr .8fr; gap:28px; padding:28px 0}
    @media (max-width:900px){.foot{grid-template-columns:1fr}}
    .copyright{border-top:1px solid rgba(255,255,255,.12); padding:14px 0; color:#cde3cf}

    /* Utilities */
    .sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border:0}
  </style></head>
<body>
  <!-- Skip link -->
  <a class="sr-only" href="#main">Skip to content</a>  <!-- NAV -->  <header>
    <div class="container nav">
      <div class="brand">
        <div class="logo" aria-hidden="true"></div>
        <div>
          <h1>Shivam Khad Bhandar</h1>
          <small>Fertilizers • Pesticides • Seeds</small>
        </div>
      </div>
      <nav aria-label="Primary">
        <div class="nav-links">
          <a href="#products">Products</a>
          <a href="#contact">Contact</a>
          <a href="#map">Find us</a>
        </div>
      </nav>
    </div>
  </header>  <!-- HERO -->  <section class="hero" id="home">
    <div class="container hero-inner">
      <div>
        <h2 class="title">Shivam Khad Bhandar</h2>
        <p class="tagline">Fertilizers • Pesticides • Seeds</p>
        <div class="cta-row">
          <a class="btn primary" href="tel:+91XXXXXXXXXX" aria-label="Call us">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.8 19.8 0 0 1-8.63-3.07 19.48 19.48 0 0 1-6-6A19.8 19.8 0 0 1 2.08 4.18 2 2 0 0 1 4.06 2h3a2 2 0 0 1 2 1.72c.12.9.3 1.78.56 2.63a2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.45-1.08a2 2 0 0 1 2.11-.45c.85.26 1.73.44 2.63.56A2 2 0 0 1 22 16.92z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
            Call
          </a>
          <a class="btn ghost" href="https://wa.me/91XXXXXXXXXX" target="_blank" rel="noopener" aria-label="Chat on WhatsApp">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true"><path d="M20.52 3.48A11.73 11.73 0 0 0 12 .75C5.82.75.75 5.82.75 12c0 2.05.53 4.04 1.54 5.81L.75 23.25l5.56-1.49A11.2 11.2 0 0 0 12 23.25c6.18 0 11.25-5.07 11.25-11.25 0-3.01-1.17-5.84-3.23-7.99zM12 21a9 9 0 0 1-4.59-1.26l-.33-.2-3.29.88.88-3.29-.2-.33A9 9 0 1 1 12 21zm5.11-6.88c-.28-.14-1.65-.82-1.91-.91-.26-.1-.45-.14-.64.14-.19.28-.73.91-.9 1.09-.16.19-.33.21-.61.07-.28-.14-1.19-.44-2.27-1.4-.84-.75-1.41-1.67-1.57-1.95-.16-.28-.02-.43.12-.57.12-.12.28-.33.42-.49.14-.16.19-.28.28-.47.09-.19.05-.36-.02-.5-.07-.14-.64-1.53-.88-2.09-.23-.56-.47-.48-.64-.49h-.55c-.19 0-.5.07-.76.36-.26.28-.99.97-.99 2.36s1.02 2.74 1.16 2.93c.14.19 2.01 3.07 4.86 4.31.68.29 1.21.47 1.62.6.68.22 1.31.19 1.8.12.55-.08 1.65-.68 1.88-1.34.23-.66.23-1.22.16-1.34-.07-.12-.26-.19-.54-.33z" fill="currentColor"/></svg>
            WhatsApp
          </a>
          <a class="btn ghost" href="/catalog.pdf" target="_blank" rel="noopener" aria-label="View product catalog">📘 Catalog</a>
        </div>
      </div>
      <aside class="hero-card" aria-labelledby="why-us">
        <h3 id="why-us">Why farmers choose us</h3>
        <div class="hero-list">
          <div class="hero-pill">🌿 Trusted brands</div>
          <div class="hero-pill">🧪 Genuine products</div>
          <div class="hero-pill">📦 Fresh stock</div>
          <div class="hero-pill">🕘 Convenient hours</div>
        </div>
      </aside>
    </div>
  </section>  <main id="main">
    <!-- PRODUCTS -->
    <section id="products">
      <div class="container">
        <h2 class="section-title">Popular Products</h2>
        <p class="section-sub">A few highlights. Ask us for recommendations for your crop and soil.</p><div class="grid">
      <!-- Card 1 -->
      <article class="card">
        <img src="https://via.placeholder.com/800x600?text=NPK+Fertilizer" alt="NPK fertilizer bag placeholder" loading="lazy" />
        <div class="card-body">
          <h3>NPK Fertilizer (19-19-19)</h3>
          <p class="meta">Water-soluble, quick uptake</p>
          <p class="price">₹ —</p>
        </div>
      </article>

      <!-- Card 2 -->
      <article class="card">
        <img src="https://via.placeholder.com/800x600?text=Urea" alt="Urea bag placeholder" loading="lazy" />
        <div class="card-body">
          <h3>Urea</h3>
          <p class="meta">46% Nitrogen</p>
          <p class="price">₹ —</p>
        </div>
      </article>

      <!-- Card 3 -->
      <article class="card">
        <img src="https://via.placeholder.com/800x600?text=Pesticide" alt="Pesticide bottle placeholder" loading="lazy" />
        <div class="card-body">
          <h3>Insecticide</h3>
          <p class="meta">Broad-spectrum protection</p>
          <p class="price">₹ —</p>
        </div>
      </article>

      <!-- Card 4 -->
      <article class="card">
        <img src="https://via.placeholder.com/800x600?text=Seeds" alt="Seeds pouch placeholder" loading="lazy" />
        <div class="card-body">
          <h3>Hybrid Seeds</h3>
          <p class="meta">High germination rate</p>
          <p class="price">₹ —</p>
        </div>
      </article>

      <!-- Card 5 -->
      <article class="card">
        <img src="https://via.placeholder.com/800x600?text=Fungicide" alt="Fungicide container placeholder" loading="lazy" />
        <div class="card-body">
          <h3>Fungicide</h3>
          <p class="meta">Systemic & contact</p>
          <p class="price">₹ —</p>
        </div>
      </article>

      <!-- Card 6 -->
      <article class="card">
        <img src="https://via.placeholder.com/800x600?text=Micronutrients" alt="Micronutrient mix placeholder" loading="lazy" />
        <div class="card-body">
          <h3>Micronutrient Mix</h3>
          <p class="meta">Chelated trace elements</p>
          <p class="price">₹ —</p>
        </div>
      </article>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section id="contact">
  <div class="container contact">
    <div class="contact-card">
      <h2 class="section-title">Get in touch</h2>
      <p class="section-sub">We’re happy to help with product selection and dosage guidance.</p>
      <ul class="contact-list">
        <li><a href="tel:+91XXXXXXXXXX">📞 +91 XXXXX-XXXXX</a></li>
        <li><a href="mailto:hello@shivamkhadbhandar.example">✉️ hello@shivamkhadbhandar.example</a></li>
        <li><a href="https://wa.me/91XXXXXXXXXX" target="_blank" rel="noopener">💬 WhatsApp chat</a></li>
        <li><a href="/catalog.pdf" target="_blank" rel="noopener">📘 Download catalog (PDF)</a></li>
      </ul>

      <h3 style="margin-top:18px">Hours</h3>
      <p class="meta">Mon–Sat: 9:00 AM – 7:00 PM • Sun: 10:00 AM – 2:00 PM</p>

      <h3 style="margin-top:18px">Address</h3>
      <p class="meta">Shop no. —, Local Market, City, State, PIN —</p>
    </div>
    <div class="contact-card" id="map">
      <h2 class="section-title">Find us</h2>
      <p class="section-sub">Use the map below or search for “Shivam Khad Bhandar”.</p>
      <div style="aspect-ratio:16/9; width:100%; border-radius:16px; overflow:hidden; border:1px solid #e7efe8">
        <!-- Replace the src with your real Google Maps Embed URL -->
        <iframe
          title="Google Maps location"
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d0!2d0!3d0!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2sShivam%20Khad%20Bhandar!5e0!3m2!1sen!2sin!4v0000000000000"
          width="100%" height="100%" style="border:0" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
      </div>
    </div>
  </div>
</section>

  </main>  <footer>
    <div class="container foot">
      <div>
        <h3 style="margin:0 0 6px">Shivam Khad Bhandar</h3>
        <p class="meta">Fertilizers • Pesticides • Seeds</p>
        <p class="meta">© <span id="year"></span> Shivam Khad Bhandar. All rights reserved.</p>
      </div>
      <div>
        <h4 style="margin:0 0 8px">Quick links</h4>
        <nav aria-label="Footer">
          <ul class="contact-list" style="background:none; border:none; padding:0">
            <li><a href="#products">Products</a></li>
            <li><a href="#contact">Contact</a></li>
            <li><a href="/catalog.pdf" target="_blank" rel="noopener">Catalog</a></li>
          </ul>
        </nav>
      </div>
    </div>
    <div class="container copyright">
      <small>Crafted with care for the farming community.</small>
    </div>
  </footer>  <!-- Structured Data (LocalBusiness) -->  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "LocalBusiness",
    "name": "Shivam Khad Bhandar",
    "image": ["https://example.com/og-image.jpg"],
    "url": "https://shivamkhadbhandar.example",
    "telephone": "+91 XXXXX XXXXX",
    "address": {
      "@type": "PostalAddress",
      "streetAddress": "Shop no. —, Local Market",
      "addressLocality": "City",
      "addressRegion": "State",
      "postalCode": "PIN —",
      "addressCountry": "IN"
    },
    "sameAs": [
      "https://wa.me/91XXXXXXXXXX",
      "https://shivamkhadbhandar.example/catalog.pdf"
    ],
    "openingHoursSpecification": [{
      "@type": "OpeningHoursSpecification",
      "dayOfWeek": ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"],
      "opens": "09:00",
      "closes": "19:00"
    },{
      "@type": "OpeningHoursSpecification",
      "dayOfWeek": "Sunday",
      "opens": "10:00",
      "closes": "14:00"
    }],
    "geo": {
      "@type": "GeoCoordinates",
      "latitude": 0,
      "longitude": 0
    }
  }
  </script>  <script>
    // Auto year in footer
    document.getElementById('year').textContent = new Date().getFullYear();
  </script></body>
</html>
