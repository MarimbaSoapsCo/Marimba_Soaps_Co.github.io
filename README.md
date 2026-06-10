# Marimba_Soaps_Co.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Marimba Soap Co.</title>
  <style>
    :root { --green:#2f855a; --light:#f9fbfd; --soft:#edf7f0; --text:#2d3748; --accent:#5a6c7d; --orange:#dd6b20; }
    * { box-sizing: border-box; }
    body { margin:0; font-family: 'Segoe UI', Arial, sans-serif; background: var(--light); color: var(--text); line-height:1.7; font-size: 16px; }

    header {
      position: relative;
      min-height: 80vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: #fff;
      overflow: hidden;
      padding: 80px 20px;
      background: #276749;
    }

    header::before {
      content: "";
      position: absolute;
      inset: 0;
      background: linear-gradient(rgba(0,0,0,0.45), rgba(0,0,0,0.45)), url("IMG-20260609-WA0007.jpg") center/cover no-repeat;
      z-index: 0;
    }

    .hero-content {
      position: relative;
      z-index: 1;
      max-width: 900px;
    }

    header h1 { margin:0; font-size:3.2rem; font-weight:700; letter-spacing:1px; }
    header p { font-size:1.2rem; max-width:780px; margin:16px auto 0; opacity:0.98; font-weight:400; }

    .btn, .whatsapp {
      display:inline-block;
      text-decoration:none;
      border-radius:8px;
      padding:14px 24px;
      font-weight:600;
      margin-top:18px;
      transition:transform 0.2s;
    }
    .btn { background:#fff; color:var(--green); box-shadow:0 2px 8px rgba(0,0,0,0.1); }
    .whatsapp { background:#25d366; color:#fff; box-shadow:0 2px 8px rgba(0,0,0,0.15); }
    .btn:hover, .whatsapp:hover { transform: translateY(-2px); }

    .container { max-width:1000px; margin:auto; padding:35px 20px; }
    .section { background:#fff; padding:30px; border-radius:12px; margin-bottom:24px; box-shadow:0 3px 12px rgba(0,0,0,0.08); border:1px solid #e8ecf0; }
    .section h2 { margin:0 0 16px 0; color:var(--green); font-size:1.8rem; font-weight:700; }
    .section p { margin:0; font-size:1.05rem; color:var(--text); }

    .products { display:grid; grid-template-columns:repeat(auto-fit, minmax(200px, 1fr)); gap:18px; }
    .product { background:linear-gradient(135deg, var(--soft), #e8f5e9); padding:20px; border-radius:12px; border:1px solid #d5e8d8; }
    .product h3 { margin:0 0 10px 0; font-size:1.2rem; font-weight:600; color:var(--green); }
    .product p { margin:0; font-size:0.95rem; color:var(--accent); line-height:1.6; }
    .product img { width:100%; height:200px; object-fit:cover; border-radius:8px; margin-bottom:14px; box-shadow:0 2px 6px rgba(0,0,0,0.1); }

    .features ul { margin:10px 0 0 20px; padding:0; }
    .features li { margin-bottom:10px; font-size:1.02rem; color:var(--text); }

    footer { text-align:center; padding:24px; background:#e8ecf0; margin-top:30px; border-top:1px solid #dbe0e5; color:var(--accent); font-size:0.95rem; }
    .small { color:#7a8b9a; font-size:0.9rem; margin-top:10px; }
    a { text-decoration:none; color:inherit; transition:color 0.2s; }
    a:hover { color:var(--green); }
    .phone-link { color:var(--green); font-weight:600; }
    .whatsapp-second { background:#25d366; color:#fff; display:inline-block; margin-left:10px; }

    .cold-info { background:#e8f5e9; padding:18px; border-radius:10px; margin-top:18px; border:1px solid #d5e8d8; }
    .cold-info strong { color:var(--green); font-size:1.05rem; }
    .cold-info ul { margin:10px 0 0 20px; padding:0; }
    .cold-info li { margin-bottom:8px; font-size:1rem; color:var(--text); }

    .process-section { margin-bottom:10px; }
    .process-label {
      background: var(--green);
      color: #fff;
      padding: 8px 16px;
      border-radius: 6px;
      font-weight: 600;
      font-size: 1.05rem;
      margin-bottom: 18px;
      display: inline-block;
    }
    .hot-process-label { background: var(--orange); color: #fff; }

    .marimba-reasons ul { margin:10px 0 0 0; padding:0; list-style:none; }
    .marimba-reasons li {
      margin-bottom: 14px;
      font-size: 1.03rem;
      color: var(--text);
      padding-left: 28px;
      position: relative;
    }
    .marimba-reasons li::before {
      content: "✓";
      position: absolute;
      left: 0;
      color: var(--green);
      font-weight: 700;
      font-size: 1.1rem;
    }

    .detergent-note {
      background: #fef3c7;
      padding: 16px;
      border-radius: 8px;
      margin-top: 20px;
      border: 1px solid #fde68a;
    }
    .detergent-note strong { color: #92400e; font-size: 1.05rem; }

    .gallery-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 18px;
    }
    .gallery-item {
      background: #f8fafc;
      border: 1px solid #e2e8f0;
      border-radius: 12px;
      overflow: hidden;
      box-shadow: 0 2px 10px rgba(0,0,0,0.06);
    }
    .gallery-item img {
      width: 100%;
      height: 220px;
      object-fit: cover;
      display: block;
    }
    .gallery-item h3 {
      margin: 0;
      padding: 14px 16px 4px;
      color: var(--green);
      font-size: 1.15rem;
    }
    .gallery-item p {
      margin: 0;
      padding: 0 16px 16px;
      color: var(--accent);
      font-size: 0.95rem;
    }

    @media (max-width: 600px) {
      header h1 { font-size: 2.2rem; }
      header p { font-size: 1rem; }
      header { min-height: 60vh; }
    }
  </style>
</head>
<body>
  <header>
    <div class="hero-content">
      <h1>Marimba Soap Co.</h1>
      <p>Wide range of commodity soaps made in Zimbabwe — natural, ethical, and crafted for everyday use.</p>
      <a class="btn" href="#products">Shop Now</a>
    </div>
  </header>

  <div class="container">
    <div class="section">
      <h2>About Us</h2>
      <p>Marimba Soap Co. creates quality handmade soap for homes, shops, and gifts. We focus on simple, natural ingredients, delightful fragrances, and value you can trust.</p>
    </div>

    <div class="section features">
      <h2>Why Buy From Us</h2>
      <ul>
        <li>We make fresh, handmade soap in Zimbabwe with care.</li>
        <li>Simple, quality ingredients that are gentle on your skin.</li>
        <li>Affordable prices for everyday use.</li>
        <li>Delightful fragrances and long-lasting soap bars.</li>
        <li>Easy ordering by WhatsApp at +263 777 708 493 / +263 776 602 025.</li>
      </ul>
    </div>

    <div class="section marimba-reasons">
      <h2>Why Buy Marimba & Bathing Detergents</h2>
      <p>Choosing Marimba means supporting authentic Zimbabwean craftsmanship — locally made soap that honors our heritage while delivering quality you can trust.</p>
      <ul>
        <li><strong>Zimbabwean Heritage:</strong> Made proudly in Zimbabwe, supporting local businesses and communities in Dangamvura, Mutare.</li>
        <li><strong>Natural Ingredients:</strong> We use simple, quality natural oils and ingredients — no harsh chemicals, synthetic preservatives, or petroleum-based surfactants.</li>
        <li><strong>Ethical Production:</strong> Handcrafted with care using fair, transparent practices that respect both workers and customers.</li>
        <li><strong>Eco-Friendly Extraction:</strong> Our cold-process method uses traditional, low-energy techniques that preserve natural glycerin and minimize environmental impact.</li>
        <li><strong>Gentle on Skin:</strong> Natural glycerin attracts moisture from the air and locks it into your skin, keeping it soft and hydrated.</li>
        <li><strong>Long-Lasting Value:</strong> Handmade bars last longer than commercial soaps and produce rich, creamy lather without drying your skin.</li>
        <li><strong>Biodegradable & Safe:</strong> True soap is biodegradable and eco-friendly, breaking down naturally without harming aquatic ecosystems.</li>
      </ul>

      <div class="detergent-note">
        <strong>When to Choose Bathing Detergents:</strong>
        <p>Detergents perform better in hard water (with calcium/magnesium minerals) and for heavy-duty cleaning like laundry. However, many commercial detergents contain synthetic chemicals that are less biodegradable than natural soap. For body bathing, natural handmade soap is gentler and more moisturizing.</p>
      </div>
    </div>

    <div class="section">
      <h2>Featured Gallery</h2>
      <div class="gallery-grid">
        <div class="gallery-item">
          <img src="1000012039.jpeg" alt="Marimba Soap product collection">
          <h3>Product Collection</h3>
          <p>Our handmade soaps in a beautiful collection.</p>
        </div>
        <div class="gallery-item">
          <img src="1000012041.jpeg" alt="Marimba Soap Zimbabwe banner">
          <h3>Brand Banner</h3>
          <p>Proudly Zimbabwean, natural, and eco-friendly.</p>
        </div>
        <div class="gallery-item">
          <img src="1000012040.jpeg" alt="Marimba Soap cold process collection">
          <h3>Cold Process Range</h3>
          <p>Authentically Zimbabwean and purely natural.</p>
        </div>
      </div>
    </div>

    <div class="section" id="products">
      <h2>Our Products</h2>

      <div class="process-section">
        <span class="process-label">Cold Process Soap</span>
        <p style="margin-bottom: 18px; font-size: 1rem;">Made using the traditional method – oils and lye are mixed and left to cure naturally for several weeks. Creates a gentle, long-lasting bar with rich lather.</p>
        <div class="products">
          <div class="product">
            <img src="rosemary-ginger-soap.jpeg" alt="Rosemary Ginger Soap">
            <h3>Rosemary Ginger Soap</h3>
            <p>Refreshing herbal soap with rosemary and ginger.</p>
          </div>
          <div class="product">
            <img src="aloe-vera-soap.jpeg" alt="Aloe Vera Soap">
            <h3>Aloe Vera Soap</h3>
            <p>Gentle soap with aloe vera for soft, soothing skin.</p>
          </div>
          <div class="product">
            <img src="aloe-vera-mopane-soap.jpeg" alt="Aloe Vera and Mopane Soap">
            <h3>Aloe Vera and Mopane</h3>
            <p>Natural soap blended with aloe vera and mopane.</p>
          </div>
          <div class="product">
            <img src="honey-turmeric-soap.jpeg" alt="Honey Turmeric Soap">
            <h3>Honey Turmeric Soap</h3>
            <p>Honey and turmeric soap for glowing, healthy skin.</p>
          </div>
          <div class="product">
            <img src="plain-soap.jpeg" alt="Plain Soap">
            <h3>Plain Soap</h3>
            <p>Simple everyday soap made with a clean, classic formula.</p>
          </div>
          <div class="product">
            <img src="coconut-soap.jpeg" alt="Coconut Soap">
            <h3>Coconut Soap</h3>
            <p>Rich coconut soap with a smooth, creamy feel.</p>
          </div>
        </div>
      </div>

      <div class="process-section">
        <span class="process-label hot-process-label">Hot Process Soap</span>
        <p style="margin-bottom: 18px; font-size: 1rem;">Made with accelerated heating for faster production. Still uses quality natural ingredients with delightful fragrances, ready to use sooner.</p>
        <div class="products">
          <div class="product">
            <img src="laundry-soap.jpg" alt="Laundry Soap">
            <h3>Laundry Soap</h3>
            <p>Strong soap for clothes and household cleaning.</p>
          </div>
          <div class="product">
            <img src="lemon-soap.jpg" alt="Lemon Soap">
            <h3>Lemon Soap</h3>
            <p>Fresh lemon soap that cleanses and brightens skin.</p>
            <div class="product">
  <img src="african-black-soap.jpg" alt="African Black Soap">
  <h3>Heaven Black Soap</h3>
  <p>A rich African black soap for bathing, made for a smooth, refreshing cleanse and soft, healthy skin.</p>
</div>
          </div>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>Custom Orders</h2>
      <p>We take custom orders for birthdays, weddings, gifts, events, bulk purchases, and personalized soap designs. Choose your preferred scent, color, style, and packaging, and we’ll make it just for you.</p>
    </div>

    <div class="section">
      <h2>Cold Process Soap Benefits</h2>
      <div class="cold-info">
        <strong>Why Choose Cold Process:</strong>
        <ul>
          <li>Gentle on skin with natural glycerin</li>
          <li>Long-lasting bar that doesn't dissolve quickly</li>
          <li>Rich, creamy lather</li>
          <li>All natural ingredients, no harsh chemicals</li>
          <li>Custom scents and designs available</li>
        </ul>
      </div>
    </div>

    <div class="section">
      <h2>Order on WhatsApp</h2>
      <p>Tap below to chat and place an order.</p>
      <a class="whatsapp" href="https://wa.me/263777708493" target="_blank" rel="noopener">Chat on WhatsApp</a>
      <a class="whatsapp whatsapp-second" href="https://wa.me/263776602025" target="_blank" rel="noopener">WhatsApp 2nd Line</a>
      <p class="small">Alternate line: <a class="phone-link" href="https://wa.me/263776602025">+263 776 602 025</a></p>
    </div>

    <div class="section">
      <h2>Contact</h2>
      <p>Call / WhatsApp:</p>
      <p><a class="phone-link" href="tel:+263777708493">+263 777 708 493</a> / <a class="phone-link" href="tel:+263776602025">+263 776 602 025</a></p>
      <p>Email: marimbasoap@gmail.com</p>
      <p>Location: 4893 Area 3, Dangamvura, Mutare, Zimbabwe</p>
    </div>
  </div>

  <footer>
    <p>© 2026 Marimba Soap Co. All rights reserved.</p>
  </footer>
</body>
</html>
