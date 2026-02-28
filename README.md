<div align="center">

<!--  ╔══════════════════════════════════════════════╗
      ║   KRISHNA BAROT — GitHub Profile README      ║
      ║   Theme: Dark Noir × Blush Rose              ║
      ╚══════════════════════════════════════════════╝  -->

<!-- ✦ ANIMATED HEADER — Morphing blobs + ink-drip name reveal -->
<svg width="860" height="240" viewBox="0 0 860 240" xmlns="http://www.w3.org/2000/svg">
  <defs>

    <!-- Deep dark background -->
    <radialGradient id="hBg" cx="30%" cy="50%" r="70%">
      <stop offset="0%"   stop-color="#1f0b1a"/>
      <stop offset="100%" stop-color="#06030a"/>
    </radialGradient>

    <!-- Shimmer gradient for name text -->
    <linearGradient id="nameGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%"   stop-color="#ffffff"/>
      <stop offset="40%"  stop-color="#ffc2df"/>
      <stop offset="75%"  stop-color="#ff3d8f"/>
      <stop offset="100%" stop-color="#e0608f"/>
    </linearGradient>

    <!-- Glow filter -->
    <filter id="glow" x="-30%" y="-30%" width="160%" height="160%">
      <feGaussianBlur in="SourceGraphic" stdDeviation="8" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>

    <!-- Soft glow for orbs -->
    <filter id="orbGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur in="SourceGraphic" stdDeviation="28" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>

    <!-- Clip to card -->
    <clipPath id="cardClip">
      <rect width="860" height="240" rx="18"/>
    </clipPath>

  </defs>

  <!-- Background -->
  <rect width="860" height="240" rx="18" fill="url(#hBg)"/>

  <!-- Scanlines texture -->
  <rect width="860" height="240" rx="18" fill="url(#hBg)" opacity="0"/>

  <!-- ✦ Morphing blob 1 — top left -->
  <ellipse cx="100" cy="90" rx="140" ry="110" fill="#ff3d8f" opacity="0.13" filter="url(#orbGlow)" clip-path="url(#cardClip)">
    <animateTransform attributeName="transform" type="scale"
      values="1,1;1.18,0.88;0.92,1.12;1.1,0.95;1,1"
      dur="13s" repeatCount="indefinite" additive="sum"/>
    <animate attributeName="opacity" values="0.13;0.19;0.1;0.16;0.13" dur="13s" repeatCount="indefinite"/>
  </ellipse>

  <!-- ✦ Morphing blob 2 — bottom right -->
  <ellipse cx="760" cy="170" rx="110" ry="130" fill="#8b1a4a" opacity="0.18" filter="url(#orbGlow)" clip-path="url(#cardClip)">
    <animateTransform attributeName="transform" type="scale"
      values="1,1;0.85,1.2;1.15,0.9;0.95,1.08;1,1"
      dur="17s" repeatCount="indefinite" additive="sum"/>
  </ellipse>

  <!-- ✦ Morphing blob 3 — center -->
  <ellipse cx="480" cy="110" rx="80" ry="70" fill="#ff85be" opacity="0.09" filter="url(#orbGlow)" clip-path="url(#cardClip)">
    <animateTransform attributeName="transform" type="scale"
      values="1,1;1.3,0.8;0.9,1.2;1.1,1;1,1"
      dur="10s" repeatCount="indefinite" additive="sum"/>
    <animate attributeName="cx" values="480;500;460;490;480" dur="10s" repeatCount="indefinite"/>
  </ellipse>

  <!-- ✦ Spinning dashed ring -->
  <circle cx="430" cy="118" r="95" fill="none" stroke="#ff3d8f" stroke-width="0.8"
          stroke-dasharray="4 8" opacity="0.2">
    <animateTransform attributeName="transform" type="rotate"
      values="0 430 118;360 430 118" dur="22s" repeatCount="indefinite"/>
  </circle>

  <!-- ✦ Spinning dot on ring -->
  <circle cx="525" cy="118" r="3.5" fill="#ff3d8f" opacity="0.6"
          filter="url(#glow)">
    <animateTransform attributeName="transform" type="rotate"
      values="0 430 118;360 430 118" dur="22s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.4;0.9;0.4" dur="2s" repeatCount="indefinite"/>
  </circle>

  <!-- ✦ Outer faint ring -->
  <circle cx="430" cy="118" r="130" fill="none" stroke="#ff85be" stroke-width="0.4" opacity="0.08">
    <animateTransform attributeName="transform" type="rotate"
      values="360 430 118;0 430 118" dur="35s" repeatCount="indefinite"/>
  </circle>

  <!-- ✦ Name — ink drip reveal -->
  <text x="430" y="125"
        font-family="Georgia, 'Times New Roman', serif"
        font-size="58" font-weight="bold" font-style="italic"
        text-anchor="middle"
        fill="url(#nameGrad)"
        filter="url(#glow)"
        letter-spacing="2"
        opacity="0">
    Krishna Barot
    <animate attributeName="opacity"   values="0;0;1"           dur="1.4s" fill="freeze"/>
    <animate attributeName="font-size" values="44;62;58"         dur="1.4s" fill="freeze"/>
  </text>

  <!-- ✦ Subtitle — fade up -->
  <text x="430" y="166"
        font-family="Georgia, serif" font-style="italic"
        font-size="12" text-anchor="middle"
        fill="#6b3858" letter-spacing="7" opacity="0">
    AI ENGINEER  ·  ML RESEARCHER  ·  FINAL YEAR
    <animate attributeName="opacity"    values="0;0;0;0.85"        dur="2.2s" fill="freeze"/>
    <animate attributeName="letter-spacing" values="2;7"           dur="1.2s" begin="0.8s" fill="freeze"/>
  </text>

  <!-- Corner brackets -->
  <path d="M22,38 L22,18 L42,18" stroke="#ff3d8f" stroke-width="1.5" fill="none" opacity="0.7"/>
  <path d="M838,38 L838,18 L818,18" stroke="#ff3d8f" stroke-width="1.5" fill="none" opacity="0.7"/>
  <path d="M22,202 L22,222 L42,222" stroke="#ff3d8f" stroke-width="1.5" fill="none" opacity="0.7"/>
  <path d="M838,202 L838,222 L818,222" stroke="#ff3d8f" stroke-width="1.5" fill="none" opacity="0.7"/>

  <!-- Thin border -->
  <rect width="860" height="240" rx="18" fill="none" stroke="#2a0f22" stroke-width="1"/>

  <!-- ✦ Floating petal particles -->
  <circle cx="80"  cy="180" r="2.5" fill="#ff85be" opacity="0.4">
    <animate attributeName="cy"      values="180;160;180" dur="4s"   repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.2;0.6;0.2" dur="4s"   repeatCount="indefinite"/>
  </circle>
  <circle cx="780" cy="60"  r="2"   fill="#ffc2df" opacity="0.35">
    <animate attributeName="cy"      values="60;44;60"    dur="3.2s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.1;0.5;0.1" dur="3.2s" repeatCount="indefinite"/>
  </circle>
  <circle cx="200" cy="30"  r="1.5" fill="#ff3d8f" opacity="0.3">
    <animate attributeName="opacity" values="0;0.7;0"     dur="2.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="640" cy="210" r="2"   fill="#ff85be" opacity="0.3">
    <animate attributeName="cy"      values="210;196;210" dur="5s"   repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.15;0.5;0.15" dur="5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="350" cy="15"  r="1.2" fill="#ffc2df" opacity="0.25">
    <animate attributeName="opacity" values="0;0.6;0"     dur="3.8s" repeatCount="indefinite"/>
  </circle>

</svg>

<!-- ✦ ANIMATED PILLS — bloom in staggered -->
<svg width="760" height="52" viewBox="0 0 760 52" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="pillBg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0e0714"/><stop offset="100%" stop-color="#1a0f1e"/>
    </linearGradient>
  </defs>

  <!-- Pill 1 -->
  <g opacity="0">
    <rect x="8" y="9" width="128" height="34" rx="17" fill="url(#pillBg)" stroke="#ff3d8f" stroke-width="0.8"/>
    <text x="72" y="31" font-family="Georgia,serif" font-style="italic" font-size="12" fill="#ffc2df" text-anchor="middle">✦ Gen AI</text>
    <animate attributeName="opacity" values="0;0;1" dur="0.5s" begin="0.1s" fill="freeze"/>
  </g>
  <!-- Pill 2 -->
  <g opacity="0">
    <rect x="148" y="9" width="150" height="34" rx="17" fill="url(#pillBg)" stroke="#ff3d8f" stroke-width="0.8"/>
    <text x="223" y="31" font-family="Georgia,serif" font-style="italic" font-size="12" fill="#ffc2df" text-anchor="middle">✦ Deep Learning</text>
    <animate attributeName="opacity" values="0;0;1" dur="0.5s" begin="0.3s" fill="freeze"/>
  </g>
  <!-- Pill 3 -->
  <g opacity="0">
    <rect x="310" y="9" width="146" height="34" rx="17" fill="url(#pillBg)" stroke="#ff3d8f" stroke-width="0.8"/>
    <text x="383" y="31" font-family="Georgia,serif" font-style="italic" font-size="12" fill="#ffc2df" text-anchor="middle">✦ RAG Systems</text>
    <animate attributeName="opacity" values="0;0;1" dur="0.5s" begin="0.5s" fill="freeze"/>
  </g>
  <!-- Pill 4 -->
  <g opacity="0">
    <rect x="468" y="9" width="88" height="34" rx="17" fill="url(#pillBg)" stroke="#ff3d8f" stroke-width="0.8"/>
    <text x="512" y="31" font-family="Georgia,serif" font-style="italic" font-size="12" fill="#ffc2df" text-anchor="middle">✦ LLMs</text>
    <animate attributeName="opacity" values="0;0;1" dur="0.5s" begin="0.7s" fill="freeze"/>
  </g>
  <!-- Pill 5 -->
  <g opacity="0">
    <rect x="568" y="9" width="146" height="34" rx="17" fill="url(#pillBg)" stroke="#ff3d8f" stroke-width="0.8"/>
    <text x="641" y="31" font-family="Georgia,serif" font-style="italic" font-size="12" fill="#ffc2df" text-anchor="middle">✦ Software Dev</text>
    <animate attributeName="opacity" values="0;0;1" dur="0.5s" begin="0.9s" fill="freeze"/>
  </g>
</svg>

</div>

---

## *whoami*

```python
class Krishna:
    name          =  "Krishna Barot"
    location      =  "Ahmedabad, India"
    education     =  "B.E. Final Year @ LJ Institute of Engineering & Technology"
    cgpa          =  9.2                   # pretty proud of this one ✨
    current       =  "ML Intern @ e2m Solutions  (Nov 2025 → Present)"
    prev          =  "AI/ML Intern @ Kenexai  (Dec 2024 → Jun 2025)"
    obsessed_with =  ["LLMs", "Agentic AI", "RAG", "Deep Learning"]
    fun_fact      =  "I RAG'd my own notes to study for exams. It worked 💅"
    learning      =  "Multi-agent systems & fine-tuning LLMs on domain-specific data"
```

---

## *experience*

<div align="center">

<!-- ✦ EXPERIENCE CARDS -->
<svg width="740" height="175" viewBox="0 0 740 175" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="cBg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0e0714"/><stop offset="100%" stop-color="#180d20"/>
    </linearGradient>
    <linearGradient id="accentLive" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#ff3d8f"/><stop offset="100%" stop-color="#8b1a4a"/>
    </linearGradient>
    <linearGradient id="accentPast" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#6b3858"/><stop offset="100%" stop-color="#2a0f22"/>
    </linearGradient>
    <filter id="cGlow">
      <feGaussianBlur stdDeviation="4" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <!-- Card 1: e2m Solutions -->
  <rect x="8" y="8" width="346" height="158" rx="13" fill="url(#cBg)" stroke="#2a0f22" stroke-width="1"/>
  <rect x="8" y="8" width="4"   height="158" rx="3"  fill="url(#accentLive)"/>

  <!-- Pulsing live dot -->
  <circle cx="38" cy="38" r="5" fill="#ff3d8f" filter="url(#cGlow)">
    <animate attributeName="r"       values="4;6.5;4"   dur="2s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.7;1;0.7" dur="2s" repeatCount="indefinite"/>
  </circle>
  <text x="52" y="43" font-family="Georgia,serif" font-style="italic" font-size="18" fill="#ffc2df" font-weight="bold">e2m Solutions</text>
  <text x="52" y="62" font-family="Georgia,serif" font-style="italic" font-size="11" fill="#ff85be" letter-spacing="1">ML Engineer Intern</text>

  <!-- Live badge -->
  <rect x="52" y="70" width="46" height="16" rx="8" fill="#0a1f0d"/>
  <circle cx="63" cy="78" r="3" fill="#7af0a0">
    <animate attributeName="opacity" values="1;0.3;1" dur="1.4s" repeatCount="indefinite"/>
  </circle>
  <text x="70" y="82" font-family="monospace" font-size="8" fill="#7af0a0" letter-spacing="1">LIVE</text>
  <text x="105" y="82" font-family="monospace" font-size="9" fill="#6b3858">Nov 2025 → Present</text>

  <line x1="24" y1="100" x2="344" y2="100" stroke="#2a0f22" stroke-width="1"/>
  <text x="24" y="118" font-family="monospace" font-size="10" fill="#6b3858">Building ML pipelines &amp; AI-powered</text>
  <text x="24" y="134" font-family="monospace" font-size="10" fill="#6b3858">solutions for real-world problems.</text>
  <text x="24" y="150" font-family="monospace" font-size="10" fill="#6b3858">Production-grade model deployment.</text>

  <!-- Card 2: Kenexai -->
  <rect x="386" y="8" width="346" height="158" rx="13" fill="url(#cBg)" stroke="#2a0f22" stroke-width="1"/>
  <rect x="386" y="8" width="4"   height="158" rx="3"  fill="url(#accentPast)"/>

  <circle cx="416" cy="38" r="5" fill="#6b3858"/>
  <text x="430" y="43" font-family="Georgia,serif" font-style="italic" font-size="18" fill="#ffc2df" font-weight="bold">Kenexai</text>
  <text x="430" y="62" font-family="Georgia,serif" font-style="italic" font-size="11" fill="#ff85be" letter-spacing="1">AI / ML Intern</text>
  <text x="430" y="82" font-family="monospace" font-size="9" fill="#6b3858">Dec 2024 → Jun 2025  ✓</text>

  <line x1="402" y1="100" x2="722" y2="100" stroke="#2a0f22" stroke-width="1"/>
  <text x="402" y="118" font-family="monospace" font-size="10" fill="#6b3858">Fine-tuned models with TensorFlow,</text>
  <text x="402" y="134" font-family="monospace" font-size="10" fill="#6b3858">Scikit-Learn &amp; RAG pipelines.</text>
  <text x="402" y="150" font-family="monospace" font-size="10" fill="#6b3858">LLM research &amp; evaluation.</text>
</svg>

</div>

---

## *featured projects*

<div align="center">

<!-- ✦ PROJECT CARDS with shimmer sweep -->
<svg width="740" height="205" viewBox="0 0 740 205" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="pBg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0e0714"/><stop offset="100%" stop-color="#18091a"/>
    </linearGradient>
    <!-- Shimmer sweep for project cards -->
    <linearGradient id="sweep" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%"   stop-color="#ff3d8f" stop-opacity="0"/>
      <stop offset="50%"  stop-color="#ff3d8f" stop-opacity="0.07"/>
      <stop offset="100%" stop-color="#ff3d8f" stop-opacity="0">
        <animate attributeName="offset" values="0.5;1.5" dur="4s" repeatCount="indefinite"/>
      </stop>
      <stop offset="0%" stop-color="#ff3d8f" stop-opacity="0">
        <animate attributeName="offset" values="-0.5;0.5" dur="4s" repeatCount="indefinite"/>
      </stop>
    </linearGradient>
    <clipPath id="pc1"><rect x="8"   y="8" width="346" height="188" rx="13"/></clipPath>
    <clipPath id="pc2"><rect x="386" y="8" width="346" height="188" rx="13"/></clipPath>
  </defs>

  <!-- IntelliScan -->
  <rect x="8"   y="8" width="346" height="188" rx="13" fill="url(#pBg)" stroke="#2a0f22" stroke-width="1"/>
  <rect x="8"   y="8" width="346" height="188" rx="13" fill="url(#sweep)" clip-path="url(#pc1)"/>

  <!-- Tag -->
  <rect x="24" y="24" width="100" height="20" rx="10" fill="#1f0b1a" stroke="#ff3d8f" stroke-width="0.8"/>
  <text x="74" y="38" font-family="monospace" font-size="9" fill="#ff3d8f" text-anchor="middle" letter-spacing="1">RAG · NLP · LLM</text>

  <text x="24" y="80" font-family="Georgia,serif" font-style="italic" font-size="26" fill="#ffc2df">IntelliScan</text>
  <text x="24" y="98" font-family="Georgia,serif" font-style="italic" font-size="10" fill="#6b3858" letter-spacing="2">QUERY-BASED AI SUMMARIZATION</text>
  <line x1="24" y1="110" x2="340" y2="110" stroke="#2a0f22" stroke-width="1"/>
  <text x="24" y="128" font-family="monospace" font-size="10" fill="#6b3858">Ask questions → get precise answers.</text>
  <text x="24" y="144" font-family="monospace" font-size="10" fill="#6b3858">Auto-generates MCQs from content.</text>
  <text x="24" y="160" font-family="monospace" font-size="10" fill="#6b3858">RAG + external knowledge sources.</text>
  <text x="330" y="188" font-family="monospace" font-size="13" fill="#ff3d8f" text-anchor="middle" opacity="0.7">→</text>

  <!-- DrConnect-AI -->
  <rect x="386" y="8" width="346" height="188" rx="13" fill="url(#pBg)" stroke="#2a0f22" stroke-width="1"/>
  <rect x="386" y="8" width="346" height="188" rx="13" fill="url(#sweep)" clip-path="url(#pc2)"/>

  <rect x="402" y="24" width="128" height="20" rx="10" fill="#1f0b1a" stroke="#ff85be" stroke-width="0.8"/>
  <text x="466" y="38" font-family="monospace" font-size="9" fill="#ff85be" text-anchor="middle" letter-spacing="1">AGENTS · VISION · CREWAI</text>

  <text x="402" y="80" font-family="Georgia,serif" font-style="italic" font-size="26" fill="#ffc2df">DrConnect-AI</text>
  <text x="402" y="98" font-family="Georgia,serif" font-style="italic" font-size="10" fill="#6b3858" letter-spacing="2">MEDICAL IMAGE AI SYSTEM</text>
  <line x1="402" y1="110" x2="718" y2="110" stroke="#2a0f22" stroke-width="1"/>
  <text x="402" y="128" font-family="monospace" font-size="10" fill="#6b3858">Analyzes CT scans, X-rays &amp; MRIs.</text>
  <text x="402" y="144" font-family="monospace" font-size="10" fill="#6b3858">Multi-agent collaboration via CrewAI.</text>
  <text x="402" y="160" font-family="monospace" font-size="10" fill="#6b3858">AI-powered clinical decision support.</text>
  <text x="708" y="188" font-family="monospace" font-size="13" fill="#ff85be" text-anchor="middle" opacity="0.7">→</text>
</svg>

</div>

---

## *skills*

<div align="center">

<!-- ✦ SKILL BARS — staggered fill animation -->
<svg width="740" height="295" viewBox="0 0 740 295" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="barHot" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#ff3d8f"/><stop offset="100%" stop-color="#ff85be"/>
    </linearGradient>
    <linearGradient id="barWarm" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#8b1a4a"/><stop offset="100%" stop-color="#6b3858"/>
    </linearGradient>
  </defs>

  <text x="4" y="22" font-family="Georgia,serif" font-style="italic" font-size="11" fill="#6b3858" letter-spacing="4">PROFICIENCY</text>

  <!-- Python -->
  <text x="4"   y="54" font-family="Georgia,serif" font-style="italic" font-size="14" fill="#ffc2df">Python</text>
  <rect x="140" y="44" width="556" height="7" rx="3.5" fill="#180d20"/>
  <rect x="140" y="44" width="0"   height="7" rx="3.5" fill="url(#barHot)">
    <animate attributeName="width" from="0" to="528" dur="1.5s" begin="0.1s" fill="freeze" calcMode="spline" keySplines="0.4 0 0.2 1"/>
  </rect>
  <text x="706" y="54" font-family="monospace" font-size="10" fill="#ff3d8f" text-anchor="end">95%</text>

  <!-- Gen AI / LLMs -->
  <text x="4"   y="90" font-family="Georgia,serif" font-style="italic" font-size="14" fill="#ffc2df">Gen AI / LLMs</text>
  <rect x="140" y="80" width="556" height="7" rx="3.5" fill="#180d20"/>
  <rect x="140" y="80" width="0"   height="7" rx="3.5" fill="url(#barHot)">
    <animate attributeName="width" from="0" to="500" dur="1.5s" begin="0.3s" fill="freeze" calcMode="spline" keySplines="0.4 0 0.2 1"/>
  </rect>
  <text x="706" y="90" font-family="monospace" font-size="10" fill="#ff3d8f" text-anchor="end">90%</text>

  <!-- RAG Systems -->
  <text x="4"   y="126" font-family="Georgia,serif" font-style="italic" font-size="14" fill="#ffc2df">RAG Systems</text>
  <rect x="140" y="116" width="556" height="7" rx="3.5" fill="#180d20"/>
  <rect x="140" y="116" width="0"   height="7" rx="3.5" fill="url(#barHot)">
    <animate attributeName="width" from="0" to="484" dur="1.5s" begin="0.5s" fill="freeze" calcMode="spline" keySplines="0.4 0 0.2 1"/>
  </rect>
  <text x="706" y="126" font-family="monospace" font-size="10" fill="#ff3d8f" text-anchor="end">87%</text>

  <!-- Deep Learning -->
  <text x="4"   y="162" font-family="Georgia,serif" font-style="italic" font-size="14" fill="#ffc2df">Deep Learning</text>
  <rect x="140" y="152" width="556" height="7" rx="3.5" fill="#180d20"/>
  <rect x="140" y="152" width="0"   height="7" rx="3.5" fill="url(#barWarm)">
    <animate attributeName="width" from="0" to="472" dur="1.5s" begin="0.7s" fill="freeze" calcMode="spline" keySplines="0.4 0 0.2 1"/>
  </rect>
  <text x="706" y="162" font-family="monospace" font-size="10" fill="#6b3858" text-anchor="end">85%</text>

  <!-- SQL / Databases -->
  <text x="4"   y="198" font-family="Georgia,serif" font-style="italic" font-size="14" fill="#ffc2df">SQL / Databases</text>
  <rect x="140" y="188" width="556" height="7" rx="3.5" fill="#180d20"/>
  <rect x="140" y="188" width="0"   height="7" rx="3.5" fill="url(#barWarm)">
    <animate attributeName="width" from="0" to="445" dur="1.5s" begin="0.9s" fill="freeze" calcMode="spline" keySplines="0.4 0 0.2 1"/>
  </rect>
  <text x="706" y="198" font-family="monospace" font-size="10" fill="#6b3858" text-anchor="end">80%</text>

  <!-- Cloud / Docker -->
  <text x="4"   y="234" font-family="Georgia,serif" font-style="italic" font-size="14" fill="#ffc2df">Cloud / Docker</text>
  <rect x="140" y="224" width="556" height="7" rx="3.5" fill="#180d20"/>
  <rect x="140" y="224" width="0"   height="7" rx="3.5" fill="url(#barWarm)">
    <animate attributeName="width" from="0" to="390" dur="1.5s" begin="1.1s" fill="freeze" calcMode="spline" keySplines="0.4 0 0.2 1"/>
  </rect>
  <text x="706" y="234" font-family="monospace" font-size="10" fill="#6b3858" text-anchor="end">70%</text>

  <!-- Divider + tools -->
  <line x1="4" y1="256" x2="736" y2="256" stroke="#2a0f22" stroke-width="1"/>
  <text x="4" y="272" font-family="monospace" font-size="9" fill="#3a1530" letter-spacing="1">
    TensorFlow  ·  PyTorch  ·  Scikit-Learn  ·  HuggingFace  ·  LangChain  ·  CrewAI  ·  AWS  ·  Docker
  </text>
</svg>

</div>

---

## *education*

<div align="center">

<!-- ✦ TIMELINE with pulsing nodes -->
<svg width="740" height="155" viewBox="0 0 740 155" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <filter id="ndGlow">
      <feGaussianBlur stdDeviation="3" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <!-- Timeline spine -->
  <line x1="20" y1="16" x2="20" y2="138" stroke="#2a0f22" stroke-width="1.5"/>
  <!-- Gradient overlay on spine -->
  <line x1="20" y1="16" x2="20" y2="60" stroke="#ff3d8f" stroke-width="1.5" opacity="0.5"/>

  <!-- Node 1 — LJ Engineering (active) -->
  <circle cx="20" cy="28" r="7" fill="#ff3d8f" filter="url(#ndGlow)">
    <animate attributeName="r"       values="6;8.5;6"   dur="2.5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.8;1;0.8" dur="2.5s" repeatCount="indefinite"/>
  </circle>
  <text x="42" y="26" font-family="Georgia,serif" font-style="italic" font-size="16" fill="#ffc2df" font-weight="bold">LJ Institute of Engineering &amp; Technology</text>
  <text x="42" y="42" font-family="Georgia,serif" font-style="italic" font-size="11" fill="#ff85be">B.E. Computer Engineering · 2022 – Present</text>
  <text x="42" y="56" font-family="monospace" font-size="10" fill="#ff3d8f">9.2 CGPA ✦</text>

  <!-- Node 2 -->
  <circle cx="20" cy="88" r="5.5" fill="#6b3858"/>
  <text x="42" y="86"  font-family="Georgia,serif" font-style="italic" font-size="15" fill="#ffc2df">Divine Life School</text>
  <text x="42" y="101" font-family="Georgia,serif" font-style="italic" font-size="11" fill="#6b3858">HSC · 2021 – 2022 · 85 Percentile</text>

  <!-- Node 3 -->
  <circle cx="20" cy="128" r="5" fill="#3a1530"/>
  <text x="42" y="126" font-family="Georgia,serif" font-style="italic" font-size="15" fill="#ffc2df">Divine Life School</text>
  <text x="42" y="141" font-family="Georgia,serif" font-style="italic" font-size="11" fill="#6b3858">SSC · 2020 – 2021 · 98 Percentile 🏆</text>
</svg>

</div>

---

## *github stats*

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Krishnabarot13&show_icons=true&bg_color=06030a&title_color=ff3d8f&text_color=6b3858&icon_color=ff3d8f&border_color=2a0f22&hide_border=false&rank_icon=github" height="158"/>
&nbsp;&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Krishnabarot13&layout=compact&bg_color=06030a&title_color=ff3d8f&text_color=6b3858&border_color=2a0f22" height="158"/>

<br/><br/>

<img src="https://github-readme-streak-stats.herokuapp.com?user=Krishnabarot13&background=06030a&ring=ff3d8f&fire=ff85be&currStreakLabel=ff3d8f&sideLabels=6b3858&dates=3a1530&border=2a0f22&stroke=2a0f22"/>

</div>

---

## *let's connect*

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-0e0714?style=for-the-badge&logo=github&logoColor=ffc2df&labelColor=0e0714)](https://github.com/Krishnabarot13)&nbsp;
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0e0714?style=for-the-badge&logo=linkedin&logoColor=ff85be&labelColor=0e0714)](https://linkedin.com/in/krishnabarot13)&nbsp;
[![Gmail](https://img.shields.io/badge/Gmail-0e0714?style=for-the-badge&logo=gmail&logoColor=ff3d8f&labelColor=0e0714)](mailto:krishnasb1355@gmail.com)

</div>

---

<div align="center">

<!-- ✦ FOOTER with heartbeat line animation -->
<svg width="740" height="100" viewBox="0 0 740 100" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="ftBg" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%"   stop-color="#06030a"/>
      <stop offset="50%"  stop-color="#0e0714"/>
      <stop offset="100%" stop-color="#06030a"/>
    </linearGradient>
    <filter id="hbGlow">
      <feGaussianBlur stdDeviation="2" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <rect width="740" height="100" rx="14" fill="url(#ftBg)" stroke="#2a0f22" stroke-width="1"/>

  <!-- Heartbeat line -->
  <polyline
    points="10,40 80,40 105,18 122,62 139,24 156,54 172,40 740,40"
    fill="none" stroke="#ff3d8f" stroke-width="1.5"
    filter="url(#hbGlow)" opacity="0.6"
    stroke-dasharray="800" stroke-dashoffset="800">
    <animate attributeName="stroke-dashoffset" values="800;0" dur="2.5s" fill="freeze"/>
    <animate attributeName="opacity" values="0.6;0.3;0.6" dur="3s" begin="2.5s" repeatCount="indefinite"/>
  </polyline>

  <!-- Footer text -->
  <text x="370" y="68" font-family="Georgia,serif" font-style="italic" font-size="20"
        fill="#ff85be" text-anchor="middle" opacity="0">
    thanks for stopping by  ♡
    <animate attributeName="opacity" values="0;0;0;1" dur="3s" fill="freeze"/>
  </text>
  <text x="370" y="86" font-family="monospace" font-size="9"
        fill="#3a1530" text-anchor="middle" letter-spacing="3" opacity="0">
    BUILT WITH CURIOSITY &amp; WAY TOO MUCH CAFFEINE
    <animate attributeName="opacity" values="0;0;0;0.8" dur="3.5s" fill="freeze"/>
  </text>
</svg>

</div>
