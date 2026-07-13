<svg width="1180" height="610" viewBox="0 0 1180 610" xmlns="http://www.w3.org/2000/svg">
<defs>
  <clipPath id="canvasClip"><rect width="1180" height="610" rx="24"/></clipPath>
  <clipPath id="leftPanelClip"><rect x="40" y="40" width="380" height="530" rx="20"/></clipPath>
  <clipPath id="rightPanelClip"><rect x="460" y="40" width="680" height="530" rx="20"/></clipPath>

  <linearGradient id="bgBase" x1="0" y1="0" x2="0" y2="1">
    <stop offset="0%" stop-color="#030712"/>
    <stop offset="100%" stop-color="#0B1220"/>
  </linearGradient>

  <radialGradient id="glowA" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#3B82F6" stop-opacity="0.30"/>
    <stop offset="100%" stop-color="#3B82F6" stop-opacity="0"/>
  </radialGradient>
  <radialGradient id="glowB" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#8B5CF6" stop-opacity="0.28"/>
    <stop offset="100%" stop-color="#8B5CF6" stop-opacity="0"/>
  </radialGradient>
  <radialGradient id="glowC" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#10B981" stop-opacity="0.22"/>
    <stop offset="100%" stop-color="#10B981" stop-opacity="0"/>
  </radialGradient>

  <filter id="noise" x="-20%" y="-20%" width="140%" height="140%">
    <feTurbulence type="fractalNoise" baseFrequency="0.85" numOctaves="2" stitchTiles="stitch" result="n"/>
    <feColorMatrix in="n" type="matrix" values="0 0 0 0 0.5  0 0 0 0 0.5  0 0 0 0 0.5  0 0 0 0.025 0"/>
  </filter>

  <filter id="softGlow" x="-60%" y="-60%" width="220%" height="220%">
    <feGaussianBlur stdDeviation="3" result="b"/>
    <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
  </filter>

  <filter id="strongGlow" x="-100%" y="-100%" width="300%" height="300%">
    <feGaussianBlur stdDeviation="7" result="b"/>
    <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
  </filter>

  <linearGradient id="asciiGrad" x1="0%" y1="0%" x2="100%" y2="100%">
    <stop offset="0%" stop-color="#7C3AED"/>
    <stop offset="50%" stop-color="#22D3EE"/>
    <stop offset="100%" stop-color="#10B981"/>
    <animate attributeName="x1" values="0%;100%;0%" dur="8s" repeatCount="indefinite"/>
    <animate attributeName="x2" values="100%;200%;100%" dur="8s" repeatCount="indefinite"/>
  </linearGradient>

  <linearGradient id="textGrad" x1="0%" y1="0%" x2="100%" y2="0%">
    <stop offset="0%" stop-color="#7C3AED"/>
    <stop offset="50%" stop-color="#22D3EE"/>
    <stop offset="100%" stop-color="#10B981"/>
  </linearGradient>

  <linearGradient id="borderShimmer" gradientUnits="userSpaceOnUse" x1="0" y1="0" x2="1180" y2="0">
    <stop offset="0%" stop-color="#22D3EE" stop-opacity="0"/>
    <stop offset="50%" stop-color="#22D3EE" stop-opacity="0.85"/>
    <stop offset="100%" stop-color="#22D3EE" stop-opacity="0"/>
    <animateTransform attributeName="gradientTransform" type="translate" values="-1180 0;1180 0;-1180 0" dur="7s" repeatCount="indefinite"/>
  </linearGradient>

  <linearGradient id="sheen" x1="0%" y1="0%" x2="100%" y2="100%">
    <stop offset="0%" stop-color="#ffffff" stop-opacity="0"/>
    <stop offset="45%" stop-color="#ffffff" stop-opacity="0.10"/>
    <stop offset="55%" stop-color="#ffffff" stop-opacity="0.10"/>
    <stop offset="100%" stop-color="#ffffff" stop-opacity="0"/>
  </linearGradient>

  <linearGradient id="glassSheen" x1="0" y1="0" x2="1" y2="1">
    <stop offset="0%" stop-color="#ffffff" stop-opacity="0.05"/>
    <stop offset="100%" stop-color="#ffffff" stop-opacity="0"/>
  </linearGradient>
</defs>

<g clip-path="url(#canvasClip)">
  <rect width="1180" height="610" fill="url(#bgBase)"/>

  <g opacity="0.9">
    <ellipse cx="120" cy="80" rx="280" ry="230" fill="url(#glowA)">
      <animate attributeName="cx" values="120;190;120" dur="13s" repeatCount="indefinite"/>
    </ellipse>
    <ellipse cx="1050" cy="130" rx="320" ry="250" fill="url(#glowB)">
      <animate attributeName="cy" values="130;190;130" dur="15s" repeatCount="indefinite"/>
    </ellipse>
    <ellipse cx="900" cy="580" rx="340" ry="210" fill="url(#glowC)">
      <animate attributeName="cx" values="900;790;900" dur="17s" repeatCount="indefinite"/>
    </ellipse>
  </g>

  <rect width="1180" height="610" filter="url(#noise)" opacity="0.5"/>

  <g>
    <circle cx="150" cy="500" r="2" fill="#22D3EE">
      <animate attributeName="cy" values="500;60;500" dur="18s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.8;0" dur="18s" repeatCount="indefinite"/>
    </circle>
    <circle cx="920" cy="550" r="1.6" fill="#7C3AED">
      <animate attributeName="cy" values="550;80;550" dur="22s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.7;0" dur="22s" repeatCount="indefinite"/>
    </circle>
    <circle cx="1060" cy="480" r="2.2" fill="#10B981">
      <animate attributeName="cy" values="480;40;480" dur="20s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.6;0" dur="20s" repeatCount="indefinite"/>
    </circle>
    <circle cx="610" cy="580" r="1.8" fill="#22D3EE">
      <animate attributeName="cy" values="580;100;580" dur="24s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.7;0" dur="24s" repeatCount="indefinite"/>
    </circle>
    <circle cx="380" cy="560" r="1.4" fill="#10B981">
      <animate attributeName="cy" values="560;120;560" dur="19s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.6;0" dur="19s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- scanline sweep -->
  <rect x="0" y="-40" width="1180" height="3" fill="#22D3EE" opacity="0.12">
    <animate attributeName="y" values="-40;650" dur="6s" repeatCount="indefinite"/>
  </rect>

  <rect x="2" y="2" width="1176" height="606" rx="22" fill="none" stroke="url(#borderShimmer)" stroke-width="1.5"/>
  <rect x="0.5" y="0.5" width="1179" height="609" rx="24" fill="none" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>

  <!-- ============ LEFT PANEL ============ -->
  <g>
    <rect x="40" y="40" width="380" height="530" rx="20" fill="rgba(15,23,42,0.55)" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>
    <rect x="40" y="40" width="380" height="530" rx="20" fill="url(#glassSheen)"/>

    <g clip-path="url(#leftPanelClip)">
      <rect x="-60" y="40" width="80" height="530" fill="url(#sheen)" transform="rotate(20 40 305)">
        <animate attributeName="x" values="-140;480;-140" dur="9s" repeatCount="indefinite"/>
      </rect>
    </g>

    <g transform="translate(60,90)">
      <animateTransform attributeName="transform" type="translate" values="60,90;60,82;60,90" dur="6s" repeatCount="indefinite" additive="sum"/>

      <g font-family="'Fira Code','Courier New',monospace" font-size="13" fill="url(#asciiGrad)" filter="url(#softGlow)" xml:space="preserve">
        <g opacity="0"><text x="35" y="0">      .------------.      </text><animate attributeName="opacity" values="0;1" dur="0.35s" begin="0.10s" fill="freeze"/></g>
        <g opacity="0"><text x="35" y="17">     /              \     </text><animate attributeName="opacity" values="0;1" dur="0.35s" begin="0.25s" fill="freeze"/></g>
        <g opacity="0"><text x="35" y="34">    |    @      @    |    </text><animate attributeName="opacity" values="0;1" dur="0.35s" begin="0.40s" fill="freeze"/></g>
        <g opacity="0"><text x="35" y="51">    |                |    </text><animate attributeName="opacity" values="0;1" dur="0.35s" begin="0.55s" fill="freeze"/></g>
        <g opacity="0"><text x="35" y="68">    |     .----.     |    </text><animate attributeName="opacity" values="0;1" dur="0.35s" begin="0.70s" fill="freeze"/></g>
        <g opacity="0"><text x="35" y="85">    |                |    </text><animate attributeName="opacity" values="0;1" dur="0.35s" begin="0.85s" fill="freeze"/></g>
        <g opacity="0"><text x="35" y="102">     \______________/     </text><animate attributeName="opacity" values="0;1" dur="0.35s" begin="1.00s" fill="freeze"/></g>
        <g opacity="0"><text x="35" y="119">             ||            </text><animate attributeName="opacity" values="0;1" dur="0.35s" begin="1.15s" fill="freeze"/></g>
        <g opacity="0"><text x="35" y="136">        .----''----.       </text><animate attributeName="opacity" values="0;1" dur="0.35s" begin="1.30s" fill="freeze"/></g>
        <g opacity="0"><text x="35" y="153">        |  &lt;/&gt;  {}  |      </text><animate attributeName="opacity" values="0;1" dur="0.35s" begin="1.45s" fill="freeze"/></g>
        <g opacity="0"><text x="35" y="170">        '------------'     </text><animate attributeName="opacity" values="0;1" dur="0.35s" begin="1.60s" fill="freeze"/></g>
        <g opacity="0"><text x="35" y="187">           |       |       </text><animate attributeName="opacity" values="0;1" dur="0.35s" begin="1.75s" fill="freeze"/></g>
        <g opacity="0"><text x="35" y="204">         ==+       +==     </text><animate attributeName="opacity" values="0;1" dur="0.35s" begin="1.90s" fill="freeze"/></g>
      </g>
    </g>

    <g font-family="'Fira Code','Courier New',monospace" font-size="12.5" xml:space="preserve">
      <g opacity="0" fill="#94A3B8"><text x="60" y="330">$ whoami</text><animate attributeName="opacity" values="0;1" dur="0.4s" begin="2.2s" fill="freeze"/></g>
      <g opacity="0" fill="#22D3EE"><text x="60" y="352">Software Engineer</text><animate attributeName="opacity" values="0;1" dur="0.4s" begin="2.6s" fill="freeze"/></g>

      <g opacity="0" fill="#94A3B8"><text x="60" y="384">$ cat focus.txt</text><animate attributeName="opacity" values="0;1" dur="0.4s" begin="3.0s" fill="freeze"/></g>
      <g opacity="0" fill="#22D3EE"><text x="60" y="406">AI + Full-Stack Development</text><animate attributeName="opacity" values="0;1" dur="0.4s" begin="3.4s" fill="freeze"/></g>

      <g opacity="0" fill="#94A3B8"><text x="60" y="438">$ echo status</text><animate attributeName="opacity" values="0;1" dur="0.4s" begin="3.8s" fill="freeze"/></g>
      <g opacity="0" fill="#10B981"><text x="60" y="460">Open to opportunities_</text><animate attributeName="opacity" values="0;1" dur="0.4s" begin="4.2s" fill="freeze"/></g>
    </g>
    <rect x="235" y="450" width="7" height="14" fill="#10B981">
      <animate attributeName="opacity" values="0;0;1;0;1" keyTimes="0;0.42;0.44;0.72;0.74" dur="1s" begin="4.2s" repeatCount="indefinite"/>
    </rect>
  </g>

  <!-- ============ RIGHT PANEL ============ -->
  <g>
    <rect x="460" y="40" width="680" height="530" rx="20" fill="rgba(15,23,42,0.55)" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>
    <rect x="460" y="40" width="680" height="530" rx="20" fill="url(#glassSheen)"/>

    <g clip-path="url(#rightPanelClip)">
      <rect x="380" y="40" width="110" height="530" fill="url(#sheen)" transform="rotate(20 460 305)">
        <animate attributeName="x" values="-160;900;-160" dur="11s" repeatCount="indefinite"/>
      </rect>
    </g>

    <line x1="460" y1="88" x2="1140" y2="88" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>
    <circle cx="486" cy="64" r="6" fill="#FF5F56"/>
    <circle cx="506" cy="64" r="6" fill="#FFBD2E"/>
    <circle cx="526" cy="64" r="6" fill="#27C93F"/>
    <text x="800" y="69" text-anchor="middle" font-family="'Fira Code','Courier New',monospace" font-size="12" fill="#94A3B8">husain — zsh</text>

    <g font-family="'Fira Code','Courier New',monospace">
      <g opacity="0" fill="#94A3B8"><text x="500" y="128" font-size="19">Hi</text><animate attributeName="opacity" values="0;1" dur="0.5s" begin="0.15s" fill="freeze"/></g>
      <g opacity="0"><text x="538" y="128" font-size="19">👋</text>
        <animate attributeName="opacity" values="0;1" dur="0.5s" begin="0.35s" fill="freeze"/>
        <animateTransform attributeName="transform" type="rotate" values="0 546 120;18 546 120;0 546 120;-14 546 120;0 546 120" dur="2.2s" begin="1s" repeatCount="indefinite"/>
      </g>
      <g opacity="0"><text x="500" y="170" font-family="'Segoe UI',Arial,sans-serif" font-size="34" font-weight="700" fill="url(#textGrad)" filter="url(#softGlow)">I'm Husain</text>
        <animate attributeName="opacity" values="0;1" dur="0.6s" begin="0.55s" fill="freeze"/>
      </g>
    </g>

    <!-- typing role -->
    <g font-family="'Fira Code','Courier New',monospace" font-size="20" font-weight="500" fill="url(#textGrad)">
      <clipPath id="clipR0"><rect x="498" y="196" width="0" height="32"><animate attributeName="width" values="0;220;220" keyTimes="0;0.04;1" dur="20s" repeatCount="indefinite"/></rect></clipPath>
      <clipPath id="clipR1"><rect x="498" y="196" width="0" height="32"><animate attributeName="width" values="0;0;256;256" keyTimes="0;0.20;0.24;1" dur="20s" repeatCount="indefinite"/></rect></clipPath>
      <clipPath id="clipR2"><rect x="498" y="196" width="0" height="32"><animate attributeName="width" values="0;0;292;292" keyTimes="0;0.40;0.44;1" dur="20s" repeatCount="indefinite"/></rect></clipPath>
      <clipPath id="clipR3"><rect x="498" y="196" width="0" height="32"><animate attributeName="width" values="0;0;136;136" keyTimes="0;0.60;0.64;1" dur="20s" repeatCount="indefinite"/></rect></clipPath>
      <clipPath id="clipR4"><rect x="498" y="196" width="0" height="32"><animate attributeName="width" values="0;0;160;160" keyTimes="0;0.80;0.84;1" dur="20s" repeatCount="indefinite"/></rect></clipPath>

      <text x="500" y="220" clip-path="url(#clipR0)" opacity="0">Frontend Engineer
        <animate attributeName="opacity" values="0;1;1;0;0" keyTimes="0;0.04;0.16;0.20;1" dur="20s" repeatCount="indefinite"/>
      </text>
      <text x="500" y="220" clip-path="url(#clipR1)" opacity="0">Full Stack Developer
        <animate attributeName="opacity" values="0;0;1;1;0;0" keyTimes="0;0.20;0.24;0.36;0.40;1" dur="20s" repeatCount="indefinite"/>
      </text>
      <text x="500" y="220" clip-path="url(#clipR2)" opacity="0">Open Source Contributor
        <animate attributeName="opacity" values="0;0;1;1;0;0" keyTimes="0;0.40;0.44;0.56;0.60;1" dur="20s" repeatCount="indefinite"/>
      </text>
      <text x="500" y="220" clip-path="url(#clipR3)" opacity="0">UI Engineer
        <animate attributeName="opacity" values="0;0;1;1;0;0" keyTimes="0;0.60;0.64;0.76;0.80;1" dur="20s" repeatCount="indefinite"/>
      </text>
      <text x="500" y="220" clip-path="url(#clipR4)" opacity="0">AI Enthusiast
        <animate attributeName="opacity" values="0;0;1;1;0" keyTimes="0;0.80;0.84;0.96;1" dur="20s" repeatCount="indefinite"/>
      </text>
    </g>
    <rect y="198" width="3" height="24" fill="#22D3EE">
      <animate attributeName="x" values="500;720;756;792;636;660" keyTimes="0;0.04;0.24;0.44;0.64;0.84" calcMode="discrete" dur="20s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="1;0;1" dur="0.9s" repeatCount="indefinite"/>
    </rect>

    <!-- info rows -->
    <g font-family="'Segoe UI',Arial,sans-serif" font-size="13.5">
      <g opacity="0"><text x="500" y="255"><tspan fill="#94A3B8">📍  Location&#160;&#160;&#160;</tspan><tspan fill="#F8FAFC" font-weight="600">Johannesburg, South Africa</tspan></text>
        <animate attributeName="opacity" values="0;1" dur="0.5s" begin="1.4s" fill="freeze"/>
      </g>
      <g opacity="0"><text x="500" y="281"><tspan fill="#94A3B8">🎓  Education&#160;&#160;</tspan><tspan fill="#F8FAFC" font-weight="600">BSc Software Engineering, Eduvos</tspan></text>
        <animate attributeName="opacity" values="0;1" dur="0.5s" begin="1.6s" fill="freeze"/>
      </g>
      <g opacity="0"><text x="500" y="307"><tspan fill="#94A3B8">💡  Focus&#160;&#160;&#160;&#160;&#160;&#160;&#160;</tspan><tspan fill="#F8FAFC" font-weight="600">Graduate Software Roles, 2026</tspan></text>
        <animate attributeName="opacity" values="0;1" dur="0.5s" begin="1.8s" fill="freeze"/>
      </g>
      <g opacity="0"><text x="500" y="333"><tspan fill="#94A3B8">🔗  Portfolio&#160;&#160;</tspan><tspan fill="#F8FAFC" font-weight="600">github.com/HusainMamoojee</tspan></text>
        <animate attributeName="opacity" values="0;1" dur="0.5s" begin="2.0s" fill="freeze"/>
      </g>
      <g opacity="0"><text x="500" y="359"><tspan fill="#94A3B8">✉️  Email&#160;&#160;&#160;&#160;&#160;&#160;</tspan><tspan fill="#F8FAFC" font-weight="600">mamooghusain@gmail.com</tspan></text>
        <animate attributeName="opacity" values="0;1" dur="0.5s" begin="2.2s" fill="freeze"/>
      </g>
    </g>

    <line x1="500" y1="378" x2="1100" y2="378" stroke="rgba(255,255,255,0.08)"/>
    <text x="500" y="402" font-family="'Segoe UI',Arial,sans-serif" font-size="12" fill="#94A3B8" letter-spacing="2">SKILLS</text>

    <!-- pills -->
    <g font-family="'Segoe UI',Arial,sans-serif" font-size="12" font-weight="600">
      <g><rect x="500" y="416" width="68" height="28" rx="14" fill="rgba(255,255,255,0.05)" stroke="#22D3EE" stroke-opacity="0.5" filter="url(#softGlow)"><animate attributeName="stroke-opacity" values="0.3;0.8;0.3" dur="3s" begin="0.0s" repeatCount="indefinite"/></rect><text x="534" y="434" text-anchor="middle" fill="#F8FAFC">React</text></g>
      <g><rect x="578" y="416" width="84" height="28" rx="14" fill="rgba(255,255,255,0.05)" stroke="#22D3EE" stroke-opacity="0.5" filter="url(#softGlow)"><animate attributeName="stroke-opacity" values="0.3;0.8;0.3" dur="3s" begin="0.15s" repeatCount="indefinite"/></rect><text x="620" y="434" text-anchor="middle" fill="#F8FAFC">Next.js</text></g>
      <g><rect x="672" y="416" width="84" height="28" rx="14" fill="rgba(255,255,255,0.05)" stroke="#22D3EE" stroke-opacity="0.5" filter="url(#softGlow)"><animate attributeName="stroke-opacity" values="0.3;0.8;0.3" dur="3s" begin="0.30s" repeatCount="indefinite"/></rect><text x="714" y="434" text-anchor="middle" fill="#F8FAFC">Node.js</text></g>
      <g><rect x="766" y="416" width="106" height="28" rx="14" fill="rgba(255,255,255,0.05)" stroke="#22D3EE" stroke-opacity="0.5" filter="url(#softGlow)"><animate attributeName="stroke-opacity" values="0.3;0.8;0.3" dur="3s" begin="0.45s" repeatCount="indefinite"/></rect><text x="819" y="434" text-anchor="middle" fill="#F8FAFC">TypeScript</text></g>
      <g><rect x="882" y="416" width="90" height="28" rx="14" fill="rgba(255,255,255,0.05)" stroke="#22D3EE" stroke-opacity="0.5" filter="url(#softGlow)"><animate attributeName="stroke-opacity" values="0.3;0.8;0.3" dur="3s" begin="0.60s" repeatCount="indefinite"/></rect><text x="927" y="434" text-anchor="middle" fill="#F8FAFC">Tailwind</text></g>
      <g><rect x="982" y="416" width="76" height="28" rx="14" fill="rgba(255,255,255,0.05)" stroke="#22D3EE" stroke-opacity="0.5" filter="url(#softGlow)"><animate attributeName="stroke-opacity" values="0.3;0.8;0.3" dur="3s" begin="0.75s" repeatCount="indefinite"/></rect><text x="1020" y="434" text-anchor="middle" fill="#F8FAFC">Python</text></g>

      <g><rect x="500" y="454" width="76" height="28" rx="14" fill="rgba(255,255,255,0.05)" stroke="#10B981" stroke-opacity="0.5" filter="url(#softGlow)"><animate attributeName="stroke-opacity" values="0.3;0.8;0.3" dur="3s" begin="0.90s" repeatCount="indefinite"/></rect><text x="538" y="472" text-anchor="middle" fill="#F8FAFC">Docker</text></g>
      <g><rect x="586" y="454" width="90" height="28" rx="14" fill="rgba(255,255,255,0.05)" stroke="#10B981" stroke-opacity="0.5" filter="url(#softGlow)"><animate attributeName="stroke-opacity" values="0.3;0.8;0.3" dur="3s" begin="1.05s" repeatCount="indefinite"/></rect><text x="631" y="472" text-anchor="middle" fill="#F8FAFC">Postgres</text></g>
      <g><rect x="686" y="454" width="54" height="28" rx="14" fill="rgba(255,255,255,0.05)" stroke="#10B981" stroke-opacity="0.5" filter="url(#softGlow)"><animate attributeName="stroke-opacity" values="0.3;0.8;0.3" dur="3s" begin="1.20s" repeatCount="indefinite"/></rect><text x="713" y="472" text-anchor="middle" fill="#F8FAFC">AWS</text></g>
      <g><rect x="750" y="454" width="54" height="28" rx="14" fill="rgba(255,255,255,0.05)" stroke="#10B981" stroke-opacity="0.5" filter="url(#softGlow)"><animate attributeName="stroke-opacity" values="0.3;0.8;0.3" dur="3s" begin="1.35s" repeatCount="indefinite"/></rect><text x="777" y="472" text-anchor="middle" fill="#F8FAFC">Git</text></g>
      <g><rect x="814" y="454" width="68" height="28" rx="14" fill="rgba(255,255,255,0.05)" stroke="#10B981" stroke-opacity="0.5" filter="url(#softGlow)"><animate attributeName="stroke-opacity" values="0.3;0.8;0.3" dur="3s" begin="1.50s" repeatCount="indefinite"/></rect><text x="848" y="472" text-anchor="middle" fill="#F8FAFC">Figma</text></g>
    </g>

    <text x="800" y="505" text-anchor="middle" font-family="'Segoe UI',Arial,sans-serif" font-size="12" fill="#94A3B8" letter-spacing="1">LET'S BUILD SOMETHING TOGETHER</text>

    <!-- socials -->
    <g font-family="'Segoe UI',Arial,sans-serif" font-size="11" font-weight="700">
      <g>
        <circle cx="669" cy="535" r="15" fill="rgba(255,255,255,0.05)" stroke="url(#textGrad)" stroke-width="1.2" filter="url(#softGlow)">
          <animateTransform attributeName="transform" type="scale" values="1;1.08;1" additive="sum" dur="3s" begin="0s" repeatCount="indefinite"/>
        </circle>
        <text x="669" y="539" text-anchor="middle" fill="#F8FAFC">GH</text>
      </g>
      <g>
        <circle cx="727" cy="535" r="15" fill="rgba(255,255,255,0.05)" stroke="url(#textGrad)" stroke-width="1.2" filter="url(#softGlow)">
          <animateTransform attributeName="transform" type="scale" values="1;1.08;1" additive="sum" dur="3s" begin="0.4s" repeatCount="indefinite"/>
        </circle>
        <text x="727" y="539" text-anchor="middle" fill="#F8FAFC">in</text>
      </g>
      <g>
        <circle cx="785" cy="535" r="15" fill="rgba(255,255,255,0.05)" stroke="url(#textGrad)" stroke-width="1.2" filter="url(#softGlow)">
          <animateTransform attributeName="transform" type="scale" values="1;1.08;1" additive="sum" dur="3s" begin="0.8s" repeatCount="indefinite"/>
        </circle>
        <text x="785" y="539" text-anchor="middle" fill="#F8FAFC">X</text>
      </g>
      <g>
        <circle cx="843" cy="535" r="15" fill="rgba(255,255,255,0.05)" stroke="url(#textGrad)" stroke-width="1.2" filter="url(#softGlow)">
          <animateTransform attributeName="transform" type="scale" values="1;1.08;1" additive="sum" dur="3s" begin="1.2s" repeatCount="indefinite"/>
        </circle>
        <text x="843" y="539" text-anchor="middle" fill="#F8FAFC">PF</text>
      </g>
    </g>
  </g>
</g>
</svg>
