# Gulshan-<!DOCTYPE html>
<html lang="hi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title> DESI SNACK's| Mobile Friendly</title>
  <meta name="description" content="मोबाइल से बनी एक तेज़, responsive और modern वेबसाइट का टेम्पलेट।" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0b1220;/* गहरा नीला */
      --card:#111a2e;/* कार्ड बैकग्राउंड */
      --muted:#6b7a90;/* हल्का टेक्स्ट */
      --text:#eaeef7;/* मुख्य टेक्स्ट */
      --brand:#4f8cff;/* ब्रांड कलर */
      --brand2:#22c55e;/* सेकेंडरी */
      --ring: 0 0 0 3px rgba(79,140,255,.25);
      --radius: 16px;
      --shadow: 0 10px 25px rgba(0,0,0,.35);
      --shadow-soft: 0 6px 16px rgba(0,0,0,.25);
    }
    *{box-sizing:border-box}
    html,body{margin:0;padding:0;background:linear-gradient(180deg,#08101d, #0d1628 40%, #0b1220);color:var(--text);font-family:Inter,system-ui,Segoe UI,Roboto,Arial,sans-serif}
    a{color:inherit;text-decoration:none}
    img{max-width:100%;display:block}

    /* Layout */
    .container{width:min(1100px,90%);margin-inline:auto}
    header{position:sticky;top:0;z-index:50;background:rgba(11,18,32,.7);backdrop-filter: blur(10px);border-bottom:1px solid rgba(255,255,255,.06)}
    .nav{display:flex;align-items:center;justify-content:space-between;padding:14px 0}
    .brand{display:flex;align-items:center;gap:10px;font-weight:800}
    .brand .logo{width:36px;height:36px;border-radius:10px;background:linear-gradient(135deg,var(--brand),#a78bfa);display:grid;place-items:center;box-shadow:var(--shadow-soft)}
    .brand span{letter-spacing:.3px}
    .nav a{opacity:.9}
    .menu{display:flex;gap:18px}
    .menu a:hover{opacity:1}
    .cta{padding:10px 16px;border-radius:999px;background:linear-gradient(90deg,var(--brand),#60a5fa);font-weight:600;box-shadow:var(--shadow-soft)}
    .burger{display:none}

    /* Hero */
    .hero{padding:64px 0 24px}
    .pill{display:inline-flex;gap:10px;align-items:center;border:1px solid rgba(255,255,255,.12);padding:6px 10px;border-radius:999px;color:var(--muted);background:rgba(255,255,255,.03)}
    .hero h1{font-size:clamp(28px,4.5vw,48px);line-height:1.15;margin:14px 0}
    .lead{color:#c9d6ff;opacity:.95;max-width:720px;font-size:clamp(14px,2.8vw,18px)}
    .hero-cta{margin-top:18px;display:flex;gap:12px;flex-wrap:wrap}
    .btn{display:inline-flex;align-items:center;gap:10px;padding:12px 16px;border-radius:12px;border:1px solid rgba(255,255,255,.12);background:rgba(255,255,255,.04);font-weight:600}
    .btn.primary{background:linear-gradient(90deg,var(--brand),#60a5fa);border:none}
    .btn:focus-visible{outline:none;box-shadow:var(--ring)}

    /* Feature grid */
    .grid{display:grid;gap:18px;grid-template-columns:repeat(12,1fr)}
    .card{grid-column:span 4;background:var(--card);border:1px solid rgba(255,255,255,.06);border-radius:var(--radius);padding:18px;box-shadow:var(--shadow)}
    .card h3{margin:8px 0 8px;font-size:18px}
    .card p{color:var(--muted);font-size:14px;line-height:1.6}
    .card .icon{width:36px;height:36px;border-radius:10px;display:grid;place-items:center;background:rgba(79,140,255,.15);border:1px solid rgba(79,140,255,.35)}

    /* Showcase */
    .section{padding:38px 0}
    .section h2{font-size:clamp(22px,3.8vw,32px);margin:0 0 12px}
    .muted{color:var(--muted)}
    .showcase{display:grid;gap:18px;grid-template-columns:repeat(12,1fr)}
    .shot{grid-column:span 6;border-radius:18px;overflow:hidden;border:1px solid rgba(255,255,255,.06);background:#0a1323}
    .shot img{aspect-ratio:16/10;object-fit:cover}

    /* Contact */ +918521412902
    form{display:grid;gap:12px;grid-template-columns:repeat(12,1fr)}
    .field{grid-column:span 6;display:grid;gap:6px}
    .field.full{grid-column:span 12}
    input,textarea{background:#0e1830;border:1px solid rgba(255,255,255,.1);border-radius:12px;padding:12px 14px;color:var(--text)}
    textarea{min-height:120px;resize:vertical}
    label{font-size:13px;color:#c6d1ea}
    .note{font-size:12px;color:var(--muted)}

    /* Footer */
    footer{padding:28px 0 60px;color:var(--muted)}

    /* Responsive */
    @media (max-width:900px){
      .card{grid-column:span 6}
      .shot{grid-column:span 12}
    }
    @media (max-width:680px){
      .menu{display:none}
      .burger{display:inline-flex;background:#10203a;border:1px solid rgba(255,255,255,.12);padding:8px 10px;border-radius:10px}
      .drawer{position:fixed;inset:0 0 0 auto;width:min(80%,320px);background:#0d1628;border-left:1px solid rgba(255,255,255,.08);transform:translateX(100%);transition:transform .3s ease;display:flex;flex-direction:column;padding:16px;gap:6px;box-shadow:var(--shadow)}
      .drawer.open{transform:translateX(0)}
      .drawer a{padding:10px 8px;border-radius:10px}
      .drawer .close{margin-left:auto}
      .card{grid-column:span 12}
      .field{grid-column:span 12}
    }
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <a class="brand" href="#home">
        <div class="logo" aria-hidden="true">⚡</div>
        <span>Desi snack's</span>
      </a>
      <nav class="menu" aria-label="Primary">
        <a href="#features">सेवाएँ</a>
        <a href="#work">काम</a>
        <a href="#contact">संपर्क</a>
        <a class="cta" href="#contact">कोटेशन पाएं</a>
      </nav>
      <button class="burger" aria-label="Open menu" onclick="toggleDrawer(true)">☰</button>
    </div>
  </header>

  <!-- Mobile drawer -->
  <aside id="drawer" class="drawer" aria-hidden="true">
    <button class="close btn" onclick="toggleDrawer(false)">✕ बंद</button>
    <a href="#features" onclick="toggleDrawer(false)">सेवाएँ</a>
    <a href="#work" onclick="toggleDrawer(false)">काम</a>
    <a href="#contact" onclick="toggleDrawer(false)">संपर्क</a>
    <a class="btn primary" href="#contact" onclick="toggleDrawer(false)">कोटेशन पाएं</a>
  </aside>

  <main id="home" class="container">
    <section class="hero">
      <span class="pill">🚀 मोबाइल से बनी Responsive वेबसाइट</span>
      <h1>अपना बिज़नेस Online लाएँ — तेज़, साफ़ और मॉडर्न डिज़ाइन</h1>
      <p class="lead">ये टेम्पलेट एकदम रेडी‑टू‑यूज़ है। बस नाम/लोगो, टेक्स्ट और इमेज बदलें। कोड पूरी तरह मोबाइल‑फ्रेंडली है और किसी भी मुफ्त होस्टिंग (Netlify, GitHub Pages) पर चल जाएगा।</p>
      <div class="hero-cta">
        <a class="btn primary" href="#contact">कॉल / संदेश भेजें</a>
        <a class="btn" href="#features">हम क्या करते हैं</a>
      </div>
    </section>

    <section id="features" class="section">
      <h2>हमारी सेवाएँ</h2>
      <p class="muted">नीचे दी गई सेवाओं में से चुनें — छोटे बिज़नेस, पोर्टफोलियो या इवेंट के लिए परफेक्ट।</p>
      <div class="grid" role="list">
        <article class="card" role="listitem">
          <div class="icon" aria-hidden="true">💼</div>
          <h3>बिज़नेस वेबसाइट</h3>
          <p>आपके ब्रांड, प्रोडक्ट और लोकेशन की जानकारी के साथ प्रोफेशनल साइट। WhatsApp/Call बटन शामिल।</p>
        </article>
        <article class="card" role="listitem">
          <div class="icon" aria-hidden="true">🖼️</div>
          <h3>पोर्टफोलियो</h3>
          <p>फोटो/प्रोजेक्ट शोकेस करने के लिए साफ़ ग्रिड। Freelancers, फोटोग्राफर्स, आर्टिस्ट्स के लिए बढ़िया।</p>
        </article>
        <article class="card" role="listitem">
          <div class="icon" aria-hidden="true">🛒</div>
          <h3>लैंडिंग पेज</h3>
          <p>एक पेज में ऑफर, टेस्टिमोनियल और CTA के साथ कन्‍वर्ज़न‑फोकस्ड डिज़ाइन।</p>
        </article>
      </div>
    </section>

    <section id="work" class="section">
      <h2>नमूना काम</h2>
      <p class="muted">यहाँ अपने प्रोजेक्ट या प्रोडक्ट की तस्वीरें लगाएँ।</p>
      <div class="showcase">
        <figure class="shot"><img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?q=80&w=1600&auto=format&fit=crop" alt="Project screenshot 1"></figure>
        <figure class="shot"><img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c?q=80&w=1600&auto=format&fit=crop" alt="Project screenshot 2"></figure>
      </div>
    </section>

    <section id="contact" class="section">
      <h2>संपर्क करें</h2>
      <p class="muted">फॉर्म भरें या सीधे WhatsApp/Call करें।</p>
      <form onsubmit="return sendMessage(event)">
        <div class="field"><label for="name">नाम</label><input id="name" name="name" required placeholder="अपना नाम" /></div>
        <div class="field"><label for="phone">फ़ोन</label><input id="phone" name="phone" placeholder="WhatsApp/मोबाइल" /></div>
        <div class="field full"><label for="msg">संदेश</label><textarea id="msg" name="message" required placeholder="हमें क्या बनवाना है?"></textarea></div>
        <div class="field full"><button class="btn primary" type="submit">संदेश भेजें</button> <span class="note">या <a href="https://wa.me/918000000000" target="_blank" rel="noreferrer">WhatsApp पर चैट करें</a></span></div>
      </form>
    </section>
  </main>

  <DESI SNACK'S>
    <div class="container">
      <small>© <span id="y"></span> आपकी कम्पनी का नाम. सभी अधिकार सुरक्षित।</small>
    </div>
  </DESI SNACK'S>

  <script>
    // Mobile drawer
    function toggleDrawer(open){
      const d = document.getElementById('drawer');
      d.classList.toggle('open', !!open);
      d.setAttribute('aria-hidden', open? 'false':'true');
    }

    // Simple contact via WhatsApp (falls back to mailto if no phone)
    function sendMessage(e){
      e.preventDefault();
      const name = document.getElementById('name').value.trim();
      const phone = document.getElementById('phone').value.trim();
      const msg = document.getElementById('msg').value.trim();
      const text = encodeURIComponent(`नमस्ते, मेरा नाम ${GULSHAN} है. ${msg}`);
      if(phone){
        const digits = phone.replace(/\D/g,'');
        window.open(`https://wa.me/${digits}?text=${text}`, '_blank');
      } else {
        window.location.href = `mailto:hello@example.com?subject=${encodeURIComponent('Website Inquiry')}&body=${text}`;
      }
      return false;
    }

    // Year
    document.getElementById('y').textContent = new Date().getFullYear();
  </script>
</body>
</html>
