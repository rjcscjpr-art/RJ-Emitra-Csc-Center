# RJ-Emitra-Csc-Center
<!DOCTYPE html>
<html lang="hi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>RJ Emitra & CSC Center</title>
  <meta name="description" content="RJ Emitra & CSC Center - Sabhi सरकारी एवं online सेवाएँ ek hi chhat ke neeche." />

  <!-- Google Font (optional) -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet" />

  <!-- Icons (optional for phone/whatsapp icons) -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" integrity="sha512-PHPGv..." crossorigin="anonymous" referrerpolicy="no-referrer" />

  <style>
    :root {
      --primary: #2563eb;
      --primary-dark: #1d4ed8;
      --accent: #16a34a;
      --bg: #f3f4f6;
      --text: #111827;
      --muted: #6b7280;
      --white: #ffffff;
      --radius-lg: 1.25rem;
      --shadow-soft: 0 20px 30px rgba(15, 23, 42, 0.15);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: "Inter", system-ui, -apple-system, BlinkMacSystemFont, sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.6;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    img {
      max-width: 100%;
      display: block;
    }

    /* Layout */
    .container {
      width: 100%;
      max-width: 1100px;
      margin: 0 auto;
      padding: 0 1rem;
    }

    /* Navbar */
    header {
      position: sticky;
      top: 0;
      z-index: 20;
      background: rgba(243, 244, 246, 0.9);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid rgba(148, 163, 184, 0.3);
    }

    .nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0.7rem 0;
    }

    .logo {
      font-weight: 700;
      font-size: 1.1rem;
      display: flex;
      flex-direction: column;
    }

    .logo span:first-child {
      text-transform: uppercase;
      letter-spacing: 0.06em;
      font-size: 0.75rem;
      color: var(--primary);
    }

    .logo span:last-child {
      font-size: 1.1rem;
    }

    .nav-links {
      display: none;
      gap: 1.5rem;
      font-size: 0.9rem;
    }

    .nav-links a {
      color: var(--muted);
      font-weight: 500;
    }

    .nav-links a:hover {
      color: var(--primary-dark);
    }

    .nav-cta {
      display: none;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 0.35rem;
      border-radius: 999px;
      padding: 0.55rem 1.1rem;
      font-size: 0.9rem;
      font-weight: 600;
      border: none;
      cursor: pointer;
      transition: transform 0.1s ease, box-shadow 0.15s ease, background 0.15s ease;
      text-decoration: none;
      white-space: nowrap;
    }

    .btn-primary {
      background: var(--primary);
      color: var(--white);
      box-shadow: 0 14px 28px rgba(37, 99, 235, 0.35);
    }

    .btn-primary:hover {
      background: var(--primary-dark);
      transform: translateY(-1px);
      box-shadow: 0 18px 36px rgba(37, 99, 235, 0.4);
    }

    .btn-outline {
      background: transparent;
      border: 1px solid rgba(148, 163, 184, 0.8);
      color: var(--text);
    }

    .btn-outline:hover {
      background: var(--white);
      box-shadow: 0 14px 28px rgba(15, 23, 42, 0.08);
    }

    .tag {
      display: inline-flex;
      align-items: center;
      gap: 0.4rem;
      padding: 0.25rem 0.75rem;
      border-radius: 999px;
      background: rgba(37, 99, 235, 0.06);
      color: var(--primary-dark);
      font-size: 0.75rem;
      font-weight: 500;
    }

    /* Hero */
    .hero {
      padding: 2.5rem 0 2rem;
    }

    .hero-inner {
      display: grid;
      grid-template-columns: 1.1fr;
      gap: 2rem;
      align-items: center;
    }

    .hero-text h1 {
      font-size: 1.9rem;
      line-height: 1.2;
      margin: 0.8rem 0;
    }

    .hero-text h1 span {
      color: var(--primary);
    }

    .hero-text p {
      color: var(--muted);
      font-size: 0.95rem;
      max-width: 32rem;
    }

    .hero-badges {
      margin: 1rem 0 1.3rem;
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 0.75rem;
      margin-bottom: 0.7rem;
    }

    .hero-note {
      display: flex;
      align-items: center;
      gap: 0.4rem;
      font-size: 0.8rem;
      color: var(--muted);
    }

    .hero-note i {
      color: var(--accent);
    }

    .hero-card {
      background: radial-gradient(circle at top left, #dbeafe, #f9fafb);
      border-radius: var(--radius-lg);
      padding: 1.3rem;
      box-shadow: var(--shadow-soft);
    }

    .hero-card-title {
      font-size: 0.95rem;
      font-weight: 600;
      margin-bottom: 0.6rem;
    }

    .hero-list {
      list-style: none;
      font-size: 0.85rem;
      color: var(--muted);
    }

    .hero-list li {
      margin-bottom: 0.3rem;
      display: flex;
      align-items: flex-start;
      gap: 0.35rem;
    }

    .hero-list li i {
      margin-top: 0.18rem;
      font-size: 0.8rem;
      color: var(--primary-dark);
    }

    /* Sections */
    section {
      padding: 2.2rem 0;
    }

    section:nth-of-type(even) {
      background: #e5e7eb;
    }

    .section-header {
      margin-bottom: 1.5rem;
    }

    .section-eyebrow {
      font-size: 0.7rem;
      font-weight: 600;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: var(--primary-dark);
      margin-bottom: 0.2rem;
    }

    .section-title {
      font-size: 1.3rem;
      margin-bottom: 0.3rem;
    }

    .section-subtitle {
      font-size: 0.9rem;
      color: var(--muted);
      max-width: 34rem;
    }

    /* About */
    .about-grid {
      display: grid;
      gap: 1.2rem;
    }

    .about-card {
      background: var(--white);
      border-radius: var(--radius-lg);
      padding: 1.1rem 1rem;
      box-shadow: 0 14px 28px rgba(15, 23, 42, 0.08);
      border: 1px solid rgba(148, 163, 184, 0.35);
    }

    .about-card h3 {
      font-size: 1rem;
      margin-bottom: 0.4rem;
    }

    .about-card p {
      font-size: 0.86rem;
      color: var(--muted);
    }

    .about-grid ul {
      list-style: none;
      font-size: 0.85rem;
      color: var(--muted);
      margin-top: 0.3rem;
    }

    .about-grid li {
      margin-bottom: 0.25rem;
      display: flex;
      gap: 0.4rem;
    }

    .about-grid li::before {
      content: "•";
      color: var(--primary-dark);
      font-size: 1rem;
      margin-top: -0.15rem;
    }

    /* Services */
    .services-grid {
      display: grid;
      gap: 0.9rem;
    }

    .service-card {
      background: var(--white);
      border-radius: 1rem;
      padding: 0.9rem 0.9rem 0.9rem;
      border: 1px solid rgba(148, 163, 184, 0.35);
      box-shadow: 0 10px 24px rgba(15, 23, 42, 0.06);
      display: flex;
      flex-direction: column;
      gap: 0.2rem;
    }

    .service-title {
      font-size: 0.95rem;
      font-weight: 600;
    }

    .service-tagline {
      font-size: 0.78rem;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      color: var(--primary);
    }

    .service-desc {
      font-size: 0.82rem;
      color: var(--muted);
    }

    /* Info rows (Timing / Docs / Contact) */
    .info-grid {
      display: grid;
      gap: 0.9rem;
    }

    .info-card {
      background: var(--white);
      border-radius: 1rem;
      padding: 0.95rem 0.95rem;
      border: 1px solid rgba(148, 163, 184, 0.3);
      box-shadow: 0 12px 24px rgba(15, 23, 42, 0.07);
    }

    .info-card h3 {
      font-size: 0.98rem;
      margin-bottom: 0.35rem;
    }

    .info-card p,
    .info-card li {
      font-size: 0.85rem;
      color: var(--muted);
    }

    .info-list {
      list-style: none;
      margin-top: 0.2rem;
    }

    .info-list li {
      margin-bottom: 0.25rem;
    }

    .badge-soft {
      display: inline-flex;
      align-items: center;
      padding: 0.2rem 0.5rem;
      border-radius: 999px;
      background: rgba(37, 99, 235, 0.08);
      font-size: 0.72rem;
      font-weight: 500;
      color: var(--primary-dark);
      margin-right: 0.35rem;
      margin-bottom: 0.25rem;
    }

    /* Contact / Map */
    .contact-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
      margin-top: 0.7rem;
    }

    .contact-detail {
      font-size: 0.86rem;
      color: var(--muted);
      margin-bottom: 0.3rem;
    }

    .contact-detail strong {
      color: var(--text);
    }

    .map-wrapper {
      margin-top: 0.9rem;
      border-radius: 1rem;
      overflow: hidden;
      border: 1px solid rgba(148, 163, 184, 0.4);
      box-shadow: 0 12px 24px rgba(15, 23, 42, 0.07);
    }

    .map-wrapper iframe {
      border: 0;
      width: 100%;
      height: 260px;
    }

    /* Footer */
    footer {
      padding: 1.5rem 0 1.7rem;
      font-size: 0.8rem;
      color: var(--muted);
      text-align: center;
    }

    footer span {
      display: block;
    }

    /* Responsive */
    @media (min-width: 640px) {
      .hero-inner {
        grid-template-columns: 1.1fr 1fr;
      }

      .hero-text h1 {
        font-size: 2.2rem;
      }

      .about-grid {
        grid-template-columns: 1.2fr 1fr;
      }

      .services-grid {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }

      .info-grid {
        grid-template-columns: repeat(3, minmax(0, 1fr));
      }

      .nav-links {
        display: flex;
      }

      .nav-cta {
        display: block;
      }
    }

    @media (min-width: 900px) {
      .hero-text h1 {
        font-size: 2.4rem;
      }
    }
  </style>
</head>

<body>
  <!-- Navbar -->
  <header>
    <div class="container nav">
      <div class="logo">
        <span>RJ EMITRA & CSC</span>
        <span><!-- TODO: Yahan apne center ka naam thoda detail me likhen -->RJ Emitra & CSC Center</span>
      </div>

      <nav class="nav-links">
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#docs">Documents</a>
        <a href="#contact">Contact</a>
      </nav>

      <div class="nav-cta">
        <!-- TODO: yahan apna mobile no. lagayein -->
        <a href="tel:+918233801367" class="btn btn-primary">
          <i class="fa-solid fa-phone"></i>
          Call Now
        </a>
      </div>
    </div>
  </header>

  <!-- Hero -->
  <main>
    <section class="hero">
      <div class="container hero-inner">
        <div class="hero-text">
          <span class="tag">
            <i class="fa-solid fa-circle-check"></i>
            Rajasthan eMitra & CSC Seva
          </span>
          <h1>
            Sabhi <span>सरकारी & Online सेवाएँ</span> ek hi chhat ke neeche.
          </h1>
          <p>
            Electricity bill, money transfer, Aadhar update, PAN card, banking, scholarship, ticket booking
            aur bhi bahut kuch. <strong>Fast service · Transparent fees · Customer support.</strong>
          </p>

          <div class="hero-badges">
            <span class="badge-soft">Authorized eMitra Center</span>
            <span class="badge-soft">Digital Seva / CSC</span>
            <span class="badge-soft">Online Payment Facility</span>
          </div>

          <div class="hero-actions">
            <!-- TODO: Phone & WhatsApp link update karein -->
            <a href="tel:+918233801367" class="btn btn-primary">
              <i class="fa-solid fa-phone"></i>
              Turant Call Karein
            </a>
            <a href="https://wa.me/918233801367?text=Namaste%20RJ%20Emitra%20%26%20CSC%20Center%2C%20mujhe%20ek%20seva%20chahiye" class="btn btn-outline" target="_blank" rel="noopener">
              <i class="fa-brands fa-whatsapp"></i>
              WhatsApp Message
            </a>
          </div>

          <div class="hero-note">
            <i class="fa-solid fa-clock"></i>
            <span><!-- TODO: Timing change karein -->Rozana: Subah 9:00 se Shaam 7:00 baje tak (Sunday half day)</span>
          </div>
        </div>

        <aside class="hero-card" aria-label="Quick info">
          <div class="hero-card-title">Aaj hi ye services available:</div>
          <ul class="hero-list">
            <li>
              <i class="fa-solid fa-bolt"></i>
              <span>Bijli, Pani, Mobile, DTH bill payment bina line me khade hue.</span>
            </li>
            <li>
              <i class="fa-solid fa-id-card"></i>
              <span>Aadhaar update / print, PAN card apply, voter ID services.</span>
            </li>
            <li>
              <i class="fa-solid fa-building-columns"></i>
              <span>Banking / CSP: cash deposit, withdrawal, balance enquiry (अलग से उपलब्ध होने पर).</span>
            </li>
            <li>
              <i class="fa-solid fa-train"></i>
              <span>Online ticket booking – bus, train & flight (availability ke anusaar).</span>
            </li>
            <li>
              <i class="fa-solid fa-file-lines"></i>
              <span>Scholarship, online forms, e-Mitra se judi sabhi सेवाएँ.</span>
            </li>
          </ul>
        </aside>
      </div>
    </section>

    <!-- About -->
    <section id="about">
      <div class="container">
        <div class="section-header">
          <div class="section-eyebrow">About Center</div>
          <h2 class="section-title">RJ Emitra & CSC Center ke baare me</h2>
          <p class="section-subtitle">
            Humara lakshya hai ki gaon/shaahar ke logon ko <strong>saare सरकारी kaam ek hi jagah</strong> par, aasaan
            bhasha me aur sahi samay par mil sakein.
          </p>
        </div>

        <div class="about-grid">
          <div class="about-card">
            <h3><!-- TODO: Center owner ka naam -->Online Service Provider: <span style="font-weight:600;">Shri _______ ji</span></h3>
            <p>
              RJ Emitra & CSC Center par hum aapke har tarah ke online aur डिजिटल kaam ko surakshit tarike se
              complete karte hain.
            </p>
            <ul>
              <li>Customer friendly environment</li>
              <li>Transparent charges – har seva ka rate pehle hi bataya jata hai</li>
              <li>Data safety & privacy ka vishesh dhyaan</li>
            </ul>
          </div>

          <div class="about-card">
            <h3>Why choose humara center?</h3>
            <ul>
              <li>Fast processing & कम प्रतीक्षा समय</li>
              <li>Form fill-up & documentation me full support</li>
              <li>WhatsApp / phone se enquiry support</li>
              <li>Most major सरकारी websites & portals ka अनुभव</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <!-- Services -->
    <section id="services">
      <div class="container">
        <div class="section-header">
          <div class="section-eyebrow">Services</div>
          <h2 class="section-title">Yahaan milengi ye प्रमुख सेवाएँ</h2>
          <p class="section-subtitle">
            Niche diye gaye list me se adhikansh सेवाएँ hamare center par regularly की जाती hain. Kuch सेवाएँ
            state / portal availability par depend karti hain.
          </p>
        </div>

        <div class="services-grid">
          <div class="service-card">
            <div class="service-tagline">Bill Payment</div>
            <div class="service-title">Electricity, Water, Mobile & DTH bill</div>
            <p class="service-desc">
              Sabhi प्रमुख कंपनियों ke bill yahan turant online jama kiye jate hain, SMS / receipt ke sath.
            </p>
          </div>

          <div class="service-card">
            <div class="service-tagline">Aadhaar / PAN</div>
            <div class="service-title">Aadhaar update & PAN card</div>
            <p class="service-desc">
              Address / mobile update, Aadhaar print, PAN card apply, correction & reprint related सेवाएँ (availability ke saath).
            </p>
          </div>

          <div class="service-card">
            <div class="service-tagline">Banking / CSP</div>
            <div class="service-title">Mini banking services</div>
            <p class="service-desc">
              AEPS / mini statement, balance check, cash deposit/withdrawal (agar banking सुविधा enabled hai to).
            </p>
          </div>

          <div class="service-card">
            <div class="service-tagline">Government Forms</div>
            <div class="service-title">Scholarship & अन्य सरकारी form</div>
            <p class="service-desc">
              Scholarship, pension, ration card, labour card, caste/income certificate, exam forms इत्यादि ka online
              form भरना.
            </p>
          </div>

          <div class="service-card">
            <div class="service-tagline">Booking</div>
            <div class="service-title">Ticket & अन्य online booking</div>
            <p class="service-desc">
              Railway, bus, flight, hotel booking (license/portal availability ke anusaar).
            </p>
          </div>

          <div class="service-card">
            <div class="service-tagline">Print / Online</div>
            <div class="service-title">Lam, Photocopy & Online kaam</div>
            <p class="service-desc">
              Print, scan, lamination, photocopy, email, PDF banwana, document upload, online registration इत्यादि.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Documents & Timing -->
    <section id="docs">
      <div class="container">
        <div class="section-header">
          <div class="section-eyebrow">Information</div>
          <h2 class="section-title">Required Documents & Timing</h2>
          <p class="section-subtitle">
            Har service ke liye kuch basic दस्तावेज़ jaruri hote hain. Niche general list di gayi hai. Exact
            requirement ke liye humse WhatsApp / call par confirm karein.
          </p>
        </div>

        <div class="info-grid">
          <div class="info-card">
            <h3>General Documents</h3>
            <ul class="info-list">
              <li>Aadhaar card ki photocopy / scan</li>
              <li>Mobile number jo aap use karte hain</li>
              <li>1–2 passport size photographs (kuch सेवाओं ke liye)</li>
              <li>Bank passbook / account details (banking / scholarship ke liye)</li>
            </ul>
          </div>

          <div class="info-card">
            <h3>Center Timing</h3>
            <ul class="info-list">
              <!-- TODO: yahan apne exact timing change karein -->
              <li><strong>Monday – Saturday:</strong> 10:00 AM – 8:00 PM</li>
              <li><strong>Sunday:</strong> 10:00 AM – 8:00 PM (only selected services)</li>
              <li>Festival / सरकारी छुट्टी par timing alag ho sakti hai.</li>
            </ul>
          </div>

          <div class="info-card">
            <h3>Payment Options</h3>
            <ul class="info-list">
              <!-- TODO: Jo options aap de sakte hain wo rakhein -->
              <li>Cash payment available</li>
              <li>UPI (PhonePe / GPay / Paytm) supported</li>
              <li>Receipt / payment confirmation SMS/print diya jata hai</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact & Location -->
    <section id="contact">
      <div class="container">
        <div class="section-header">
          <div class="section-eyebrow">Contact & Location</div>
          <h2 class="section-title">RJ Emitra & CSC Center ka pata</h2>
          <p class="section-subtitle">
            Neeche diye gaye address par humara केंद्र स्थित hai. Aap seedhe aa sakte hain, ya pehle call / WhatsApp
            par location share karwa sakte hain.
          </p>
        </div>

        <div class="info-grid">
          <div class="info-card">
            <h3>Address</h3>
            <p class="contact-detail">
              <!-- TODO: Yahan apna exact full address daalein -->
              <strong>RJ Emitra & CSC Center</strong><br />
              Bharat Mata Chowk Niwaru 302012<br />
              Rajasthan (India)
            </p>
            <p class="contact-detail">
              <strong>Nearby landmark:</strong> Bharat Mata Chowk.
            </p>
            <div class="contact-actions">
              <!-- TODO: Phone & WhatsApp update karein -->
              <a href="tel:+918233801367" class="btn btn-primary">
                <i class="fa-solid fa-phone"></i>
                Call Center
              </a>
              <a href="https://wa.me/918233801367?text=Namaste%2C%20location%20share%20kar%20dijiye" class="btn btn-outline" target="_blank" rel="noopener">
                <i class="fa-brands fa-whatsapp"></i>
                Location on WhatsApp
              </a>
            </div>
          </div>

          <div class="info-card">
            <h3>Location Map</h3>
            <p class="contact-detail">
              Google Maps location share karne ke liye, apne business ka map open karke
              <strong>Share → Embed a map → iframe code</strong> copy karein aur niche paste kar dein.
            </p>
            <div class="map-wrapper">
              <!-- TODO: is iframe ko apne actual Google Maps embed code se replace karein -->
              <iframe
                title="RJ Emitra & CSC Center Location"
                src="https://www.google.com/maps/embed?pb="
                loading="lazy"
                referrerpolicy="no-referrer-when-downgrade">
              </iframe>
            </div>
          </div>

          <div class="info-card">
            <h3>Quick Contact Info</h3>
            <ul class="info-list">
              <!-- TODO: Nimn jagah apni details daalein -->
              <li><strong>Mobile:</strong> +91-8233801367</li>
              <li><strong>Alternate Mobile:</strong> +91-8233801367</li>
              <li><strong>Email:</strong> yourmail@example.com</li>
              <li><strong>Facebook Page:</strong> RJ Emitra & CSC Center (agar ho to)</li>
              <li><strong>WhatsApp Broadcast:</strong> Offers & updates ke liye WhatsApp par “Hi” bhejein.</li>
            </ul>
          </div>
        </div>
      </div>
    </section>
  </main>

  <!-- Footer -->
  <footer>
    <div class="container">
      <span>© <span id="year"></span> RJ Emitra & CSC Center. All rights reserved.</span>
      <span style="margin-top: 0.2rem;">Digital सेवाएँ – aasaan bhasha me, sahi samay par.</span>
    </div>
  </footer>

  <script>
    // Current year auto update
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>
