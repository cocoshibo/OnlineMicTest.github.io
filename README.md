<h1 align="center">🎙️ MicFix</h1>

<p align="center">
  A fictional web tool that helps users diagnose and fix microphone issues.
  <br>
  <em>Demo project — not a real service.</em>
</p>

<hr>

<h2>🚀 Features</h2>
<ul>
  <li><b>Microphone Detection</b> — Lists available input devices.</li>
  <li><b>Live Input Meter</b> — Visual bar display of mic volume.</li>
  <li><b>Browser Permissions Tips</b> — Helps fix blocked mic access.</li>
  <li><b>Local Processing</b> — No audio saved or transmitted.</li>
</ul>

<h2>🧰 How It Works</h2>
<ol>
  <li>User clicks <code>Check Microphone</code>.</li>
  <li>The browser requests microphone permission via WebRTC.</li>
  <li>Mic audio stream is analyzed locally with the Web Audio API.</li>
  <li>UI gives suggestions if input is too low or unavailable.</li>
</ol>

<h2>📦 Tech Stack</h2>
<ul>
  <li>HTML + CSS + JavaScript</li>
  <li>MediaDevices API</li>
  <li>Web Audio API</li>
</ul>

<pre>
<code style="
    background-color: #2c2c3e; 
    color: #f8f8f2; 
    padding: 2px 6px; 
    border-radius: 4px; 
    font-family: 'Fira Code', monospace;>
navigator.mediaDevices.getUserMedia({ audio: true })
  .then(stream => {
    console.log("Mic detected ✔");
  })
  .catch(err => {
    console.error("Problem accessing microphone:", err);
  });
</code>
</pre>

<h2>📝 Use Cases</h2>
<ul>
  <li>Streamers with a muted USB mic</li>
  <li>Gamers with Discord voice issues</li>
  <li>Students using Zoom/Google Meet</li>
  <li>New laptop users with OS privacy restrictions</li>
</ul>

<h2>❓ FAQ</h2>

<p><b>Does MicFix record my voice?</b><br>
No. All audio streams stay in your browser and are never transmitted.</p>

<p><b>My mic doesn't show — what do I do?</b><br>
Check OS privacy settings:
<br>🔹 Windows → Settings → Privacy → Microphone
<br>🔹 macOS → System Settings → Privacy → Microphone
<br>Then restart your browser.</p>

<p><b>Is this a real product?</b><br>
No — it’s a demonstration/portfolio project.</p>

<h2>📧 Contact (Fake)</h2>
<p>support@micfix.fake</p>

<hr>

<h2>📜 License</h2>
<p>
MIT License — use, modify, or repurpose freely.
<br>Attribution appreciated but not required.
</p>

<p align="center">✨ Thanks for checking out MicFix ✨</p>
