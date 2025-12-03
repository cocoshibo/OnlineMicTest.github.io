<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>MicFix — README</title>
  <meta name="description" content="MicFix — Quick & Easy Microphone Troubleshooting (fake demo README page)" />
  <style>
    /* Simple, clean styling for a README page */
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --accent:#7dd3fc;
      --muted:#9aa4b2;
      --glass: rgba(255,255,255,0.03);
      --radius:12px;
      --mono: "Courier New", monospace;
      color-scheme: dark;
    }
    html,body{height:100%;margin:0;font-family:Inter,system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial;}
    body{
      background: linear-gradient(180deg,#071427 0%, #071a2a 60%);
      color:#e6eef6;
      padding:32px;
      display:flex;
      align-items:flex-start;
      justify-content:center;
      line-height:1.5;
    }
    .wrap{
      width:100%;
      max-width:980px;
    }
    header{
      display:flex;
      gap:18px;
      align-items:center;
      margin-bottom:22px;
    }
    .logo{
      width:72px;height:72px;border-radius:14px;background:linear-gradient(135deg,var(--accent),#60a5fa);
      display:flex;align-items:center;justify-content:center;font-weight:700;color:#042c3a;
      box-shadow: 0 6px 18px rgba(7,18,36,0.6);
      font-family:var(--mono);
      font-size:20px;
    }
    h1{margin:0;font-size:28px}
    p.lead{margin:6px 0 0;color:var(--muted)}
    main{
      background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border-radius:var(--radius);
      padding:22px;
      box-shadow: 0 8px 40px rgba(2,6,23,0.6);
      border:1px solid rgba(255,255,255,0.03);
    }
    .grid{display:grid;grid-template-columns:1fr 320px;gap:18px}
    .card{background:var(--card);border-radius:10px;padding:16px;border:1px solid rgba(255,255,255,0.02)}
    .feature-list{display:grid;gap:10px}
    .feature{
      padding:10px;border-radius:8px;background:var(--glass);
      display:flex;gap:12px;align-items:flex-start;
    }
    .feature b{display:block}
    .muted{color:var(--muted);font-size:13px}
    .cta{display:inline-block;padding:10px 14px;border-radius:10px;background:linear-gradient(90deg,var(--accent),#60a5fa);color:#042c3a;font-weight:700;text-decoration:none;margin-top:10px}
    code, pre{background:rgba(255,255,255,0.02);padding:6px;border-radius:6px;font-family:var(--mono);font-size:13px}
    pre{overflow:auto}
    footer{margin-top:16px;color:var(--muted);font-size:13px;text-align:right}
    .faq dt{font-weight:700;margin-top:12px}
    .faq dd{margin:6px 0 0;color:var(--muted)}
    @media (max-width:880px){
      .grid{grid-template-columns:1fr; }
      header{gap:12px}
      .logo{width:56px;height:56px;font-size:18px}
      h1{font-size:22px}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="logo">MF</div>
      <div>
        <h1>MicFix — Quick &amp; Easy Microphone Troubleshooting</h1>
        <p class="lead">A friendly, browser-based guide to diagnose and fix common microphone problems. (Demo / fake project)</p>
      </div>
    </header>

    <main>
      <div class="grid">
        <section class="card">
          <h2>Overview</h2>
          <p class="muted">MicFix helps users identify microphone issues (no input, low volume, permissions, incorrect device selection) and provides step-by-step, local tests to confirm fixes. This README is for the demo README website — not a real service.</p>

          <h3 style="margin-top:14px">How it works</h3>
          <ol class="muted">
            <li><strong>Check Microphone:</strong> Performs local checks using the browser Web Audio / MediaDevices APIs.</li>
            <li><strong>Guided Fixes:</strong> Shows tailored instructions: OS settings, browser permissions, device selection.</li>
            <li><strong>Live Test:</strong> Displays a live level meter to confirm input — processed locally; nothing is uploaded.</li>
          </ol>

          <h3 style="margin-top:14px">Primary (Fake) Features</h3>
          <div class="feature-list">
            <div class="feature"><div><strong>Auto-Volume Booster</strong><div class="muted">Suggests gain changes for low input level.</div></div></div>
            <div class="feature"><div><strong>Smart Echo Eliminator</strong><div class="muted">Guides users to reduce echo (speaker/mic bleed).</div></div></div>
            <div class="feature"><div><strong>Privacy Mode</strong><div class="muted">All tests run locally in the browser — no voice data stored.</div></div></div>
            <div class="feature"><div><strong>Cross-platform tips</strong><div class="muted">Windows, macOS, Chrome/Edge/Firefox troubleshooting steps included.</div></div></div>
          </div>

          <h3 style="margin-top:14px">Quick Start</h3>
          <p class="muted">Open <code>index.html</code> in your browser and click <strong>Check Microphone</strong>. Follow the prompts. (Demo only.)</p>

          <h3 style="margin-top:14px">Example: Local test snippet</h3>
          <pre><code>navigator.mediaDevices.getUserMedia({ audio: true })
  .then(stream =&gt; { /* analyze audio locally, draw level meter */ })
  .catch(err =&gt; { /* show permission or device error */ })</code></pre>
        </section>

        <aside class="card">
          <h3>Support &amp; Contact</h3>
          <p class="muted">This is a fictional demo. For questions or to adapt this README for a real project, contact:</p>
          <p style="margin-top:10px"><strong>support@micfix.fake</strong></p>

          <h3 style="margin-top:18px">Platforms</h3>
          <p class="muted">Works as a browser-based demo on modern Chrome, Edge, Firefox, and supported on Windows/macOS.</p>

          <h3 style="margin-top:18px">Dev Notes</h3>
          <p class="muted">This README and demo code are MIT-friendly: copy, modify, and reuse for learning or prototyping.</p>
          <a class="cta" href="#features">View Features</a>
        </aside>
      </div>

      <section style="margin-top:18px" class="card">
        <h2 id="features">FAQ</h2>
        <dl class="faq">
          <dt>Does MicFix record my voice?</dt>
          <dd>Short answer: <strong>No.</strong> The demo processes microphone input locally via the browser. It does not upload or store audio.</dd>

          <dt>My microphone isn't detected — what can I do?</dt>
          <dd class="muted">Try unplugging/re-plugging the mic, ensure system drivers are installed, check OS privacy settings (Windows: Privacy &gt; Microphone; macOS: System Settings &gt; Microphone), and verify the browser has permission to use the mic.</dd>

          <dt>Is this a real product?</dt>
          <dd class="muted">No — this README describes a fictional demo project intended for design, documentation, or portfolio use.</dd>
        </dl>
      </section>

      <section style="margin-top:18px" class="card">
        <h2>License &amp; Attribution</h2>
        <p class="muted">This project is a playful demo. Use however you like. If you republish, a short nod to the original demo is appreciated but not required.</p>

        <h3 style="margin-top:12px">Example Attribution (optional)</h3>
        <pre><code>MicFix — demo README
copyright (c) 2025 MicFix Demo
This demo is provided "as-is" for learning and prototyping.</code></pre>
      </section>

      <footer>MicFix README • Demo only • Built with ❤️</footer>
    </main>
  </div>
</body>
