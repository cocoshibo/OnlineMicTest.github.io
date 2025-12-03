<head>
  <meta charset="UTF-8">
  <title>MicFix README</title>
  <style>
    body {
      background: #0d1117;
      color: #e5e5e5;
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 0;
      padding: 20px;
    }

    h1, h2, h3 {
      color: #7dd3fc;
    }

    a {
      color: #60a5fa;
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    /* Button */
    .btn {
      display: inline-block;
      background: #3b82f6;
      color: white;
      padding: 10px 18px;
      border-radius: 8px;
      text-decoration: none;
      font-size: 16px;
      margin: 8px 0;
    }

    .btn:hover {
      background: #2563eb;
    }

    /* Dark styled code blocks */
    pre {
      background-color: #1e1e2f;
      color: #f8f8f2;
      padding: 16px;
      border-radius: 8px;
      overflow-x: auto;
      font-family: 'Fira Code', 'Courier New', monospace;
      font-size: 14px;
      line-height: 1.5;
      margin: 16px 0;
      border: 1px solid #2c2c3e;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }

    code {
      background-color: #2c2c3e;
      color: #f8f8f2;
      padding: 2px 6px;
      border-radius: 4px;
      font-family: 'Fira Code', 'Courier New', monospace;
      font-size: 13px;
    }

    footer {
      margin-top: 30px;
      font-size: 12px;
      color: #9ca3af;
      text-align: center;
    }
  </style>
</head>
<body>

<h1>🎙️ MicFix</h1>
<p>A fake web tool that pretends to fix microphone issues. For demo/portfolio use only.</p>

<h2>🔗 Visit the Fake Website</h2>
<p>
  <a href="/micfix.html" class="btn">Mic Fix</a>
</p>

<h2>🚀 What It (Pretends to) Do</h2>
<ul>
  <li>Detects “microphone issues”</li>
  <li>Resets mic settings (fake)</li>
  <li>Shows a secret message on reset</li>
  <li>100% browser-based</li>
  <li>0% actually useful</li>
</ul>

<h2>🧰 How It Works</h2>
<ol>
  <li>User clicks <code>Reset Mic Settings</code> button.</li>
  <li>JavaScript hides main screen and shows a surprise message.</li>
</ol>

<h2>📦 Tech Stack</h2>
<ul>
  <li>HTML / CSS / JavaScript</li>
  <li>Web Audio API (demo snippet)</li>
</ul>

<h3>Example: Local test snippet</h3>
<pre><code>navigator.mediaDevices.getUserMedia({ audio: true })
  .then(stream =&gt; {
    // Connect to audio analyzer here
    console.log("Mic detected ✔");
  })
  .catch(err =&gt; {
    console.error("Mic access error:", err);
  });
</code></pre>

<h3>Example Attribution (optional)</h3>
<pre><code>MicFix — demo README
copyright (c) 2025 MicFix Demo
This demo is provided "as-is" for learning and prototyping.
</code></pre>

<h2>❓ FAQ</h2>
<p><b>Does this fix microphones?</b><br>No 😄</p>
<p><b>Is this a real support tool?</b><br>Absolutely not.</p>
<p><b>Why does this exist?</b><br>For fun, chaos, and HTML practice.</p>

<h2>🛡️ Disclaimer</h2>
<p>This project is a joke. It does not fix, repair, or configure microphones. Use real tech support for actual issues.</p>

<h2>📜 License</h2>
<p>MIT License — reuse, copy, remix freely. Attribution appreciated but optional.</p>

<footer>✨ Thanks for checking out MicFix ✨</footer>

</body>
</html>
