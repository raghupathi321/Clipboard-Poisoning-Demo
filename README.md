

<body>

<h1>📋 Clipboard Poisoning Demo (Educational)</h1>

<p>
This project demonstrates how <strong>blind copy-pasting into a terminal</strong>
can be dangerous due to clipboard manipulation by web pages.
</p>

<div class="warning">
  <strong>⚠️ Warning:</strong>
  This demo is strictly for <strong>educational purposes</strong>.
  It uses only harmless commands and does <strong>not</strong> perform any destructive action.
</div>

---

<h2>🎯 Purpose of This Demo</h2>

<p>
Many users trust that what they see on a web page is exactly what will be pasted
into their terminal. This demo shows how that assumption can be broken.
</p>

<p>
The goal is to teach:
</p>

<ul>
  <li>Why blind copy-pasting is risky</li>
  <li>How clipboard poisoning works</li>
  <li>Why human behavior is part of the security threat model</li>
</ul>

---

<h2>🧪 What the Demo Does</h2>

<p>
The page displays a harmless-looking command:
</p>

<pre>echo "Hello"</pre>

<p>
However, when the user presses any key, JavaScript silently replaces the clipboard
with a <strong>different command sequence</strong>:
</p>

<pre>echo "[DEMO] Clipboard modified"; sleep 2; echo "[DEMO] This could have been worse"</pre>

<p>
If the user pastes this blindly into a terminal, the terminal executes the entire sequence.
</p>

---

<h2>🧠 Why This Works</h2>

<ul>
  <li>Browsers allow clipboard writes after a user interaction</li>
  <li>Terminals trust pasted input completely</li>
  <li>Humans assume copy-paste is safe</li>
</ul>

<p>
This is not a software vulnerability — it is a <strong>trust vulnerability</strong>.
</p>

---

<h2>🛡️ Defensive Lessons</h2>

<p>
This demo exists to promote safer habits:
</p>

<ul>
  <li><strong>Paste first, execute second</strong></li>
  <li>Always read pasted commands before pressing Enter</li>
  <li>Watch for command separators like <code>;</code>, <code>&&</code>, and <code>|</code></li>
  <li>Use clipboard inspection tools when possible</li>
</ul>

<div class="note">
  <strong>Security Rule:</strong>
  Never treat your clipboard as trusted input.
</div>

---

<h2>🔐 Scope & Ethics</h2>

<p>
This demo:
</p>

<ul>
  <li>✔ Uses only harmless shell commands</li>
  <li>✔ Does not modify files or system state</li>
  <li>✔ Does not access network or user data</li>
  <li>✔ Is safe to run locally</li>
</ul>

<p>
Any use of clipboard manipulation for real-world harm is unethical and illegal.
</p>

---



---

<h2>✅ Key Takeaway</h2>

<blockquote>
  <strong>Security is not just about systems — it is about assumptions.</strong>
</blockquote>

<p>
This demo shows how a simple habit can become an attack vector, and why
critical thinking is the strongest defense.
</p>

---

<p><em>Stay curious. Stay cautious.</em></p>

</body>
</html>
