<!DOCTYPE html>
<html lang="sv">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Testsida</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #f0f4f8;
      color: #333;
      min-height: 100vh;
    }

    header {
      background: linear-gradient(135deg, #4f46e5, #7c3aed);
      color: white;
      padding: 40px 20px;
      text-align: center;
    }

    header h1 {
      font-size: 2.5rem;
      margin-bottom: 8px;
    }

    header p {
      font-size: 1.1rem;
      opacity: 0.85;
    }

    nav {
      background: white;
      display: flex;
      justify-content: center;
      gap: 24px;
      padding: 14px 20px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.08);
    }

    nav a {
      text-decoration: none;
      color: #4f46e5;
      font-weight: 600;
      font-size: 0.95rem;
      transition: color 0.2s;
    }

    nav a:hover {
      color: #7c3aed;
    }

    main {
      max-width: 900px;
      margin: 40px auto;
      padding: 0 20px;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 24px;
    }

    .card {
      background: white;
      border-radius: 12px;
      padding: 28px;
      box-shadow: 0 2px 12px rgba(0,0,0,0.07);
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .card:hover {
      transform: translateY(-4px);
      box-shadow: 0 6px 20px rgba(0,0,0,0.12);
    }

    .card .icon {
      font-size: 2rem;
      margin-bottom: 12px;
    }

    .card h2 {
      font-size: 1.2rem;
      margin-bottom: 8px;
      color: #1e1b4b;
    }

    .card p {
      font-size: 0.9rem;
      line-height: 1.6;
      color: #666;
    }

    .form-section {
      max-width: 900px;
      margin: 0 auto 40px;
      padding: 0 20px;
    }

    .form-section form {
      background: white;
      border-radius: 12px;
      padding: 32px;
      box-shadow: 0 2px 12px rgba(0,0,0,0.07);
      display: flex;
      flex-direction: column;
      gap: 16px;
    }

    .form-section h2 {
      font-size: 1.3rem;
      color: #1e1b4b;
      margin-bottom: 4px;
    }

    .form-section input,
    .form-section textarea {
      padding: 12px 14px;
      border: 1.5px solid #e2e8f0;
      border-radius: 8px;
      font-size: 0.95rem;
      font-family: inherit;
      transition: border-color 0.2s;
      outline: none;
    }

    .form-section input:focus,
    .form-section textarea:focus {
      border-color: #4f46e5;
    }

    .form-section textarea {
      resize: vertical;
      min-height: 100px;
    }

    .form-section button {
      background: linear-gradient(135deg, #4f46e5, #7c3aed);
      color: white;
      border: none;
      padding: 12px 28px;
      border-radius: 8px;
      font-size: 1rem;
      font-weight: 600;
      cursor: pointer;
      align-self: flex-start;
      transition: opacity 0.2s;
    }

    .form-section button:hover {
      opacity: 0.88;
    }

    footer {
      text-align: center;
      padding: 24px;
      font-size: 0.85rem;
      color: #999;
      border-top: 1px solid #e2e8f0;
    }
  </style>
</head>
<body>

  <header>
    <h1>🚀 Min Testsida</h1>
    <p>Välkommen! Det här är en enkel HTML-testsida.</p>
  </header>

  <nav>
    <a href="#">Hem</a>
    <a href="#">Om oss</a>
    <a href="#">Tjänster</a>
    <a href="#">Kontakt</a>
  </nav>

  <main>
    <div class="card">
      <div class="icon">🎨</div>
      <h2>Design</h2>
      <p>Det här är ett exempelkort som visar hur innehåll kan presenteras på ett snyggt och tydligt sätt.</p>
    </div>
    <div class="card">
      <div class="icon">⚡</div>
      <h2>Prestanda</h2>
      <p>Sidan är byggd med ren HTML och CSS, utan externa bibliotek – snabb och lätt.</p>
    </div>
    <div class="card">
      <div class="icon">📱</div>
      <h2>Responsiv</h2>
      <p>Layouten anpassar sig automatiskt till olika skärmstorlekar – mobil, surfplatta och dator.</p>
    </div>
  </main>

  <div class="form-section">
    <form onsubmit="hanteraFormular(event)">
      <h2>📬 Kontakta oss</h2>
      <input type="text" placeholder="Ditt namn" required />
      <input type="email" placeholder="Din e-postadress" required />
      <textarea placeholder="Ditt meddelande..."></textarea>
      <button type="submit">Skicka meddelande</button>
    </form>
  </div>

  <footer>
    <p>© 2026 Testsida · Byggd med HTML &amp; CSS</p>
  </footer>

  <script>
    function hanteraFormular(e) {
      e.preventDefault();
      alert('Tack för ditt meddelande! (Detta är bara ett test)');
      e.target.reset();
    }
  </script>

</body>
</html>
