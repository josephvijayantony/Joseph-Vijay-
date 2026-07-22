<svg width="760" height="180" viewBox="0 0 760 180" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#0d1117"/>
      <stop offset="100%" stop-color="#161b22"/>
    </linearGradient>
    <linearGradient id="lineGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#58a6ff"/>
      <stop offset="100%" stop-color="#39d353"/>
    </linearGradient>
    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="2.5" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <!-- background -->
  <rect width="760" height="180" rx="14" fill="url(#bg)"/>

  <!-- commit timeline path, draws itself in -->
  <path d="M 40 100 C 150 100, 180 40, 280 40 C 380 40, 380 140, 480 140 C 580 140, 600 100, 720 100"
        fill="none" stroke="url(#lineGrad)" stroke-width="3" stroke-linecap="round"
        stroke-dasharray="900" stroke-dashoffset="900">
    <animate attributeName="stroke-dashoffset" from="900" to="0" dur="2.8s"
             fill="freeze" calcMode="spline" keySplines="0.4 0 0.2 1"/>
  </path>

  <!-- commit nodes -->
  <g font-family="Consolas, Menlo, monospace" font-size="12" fill="#c9d1d9">

    <!-- start commit -->
    <circle cx="40" cy="100" r="0" fill="#39d353" filter="url(#glow)">
      <animate attributeName="r" values="0;7;5" keyTimes="0;0.6;1" dur="0.5s" begin="0.1s" fill="freeze"/>
    </circle>

    <!-- commit 1 -->
    <circle cx="280" cy="40" r="0" fill="#58a6ff" filter="url(#glow)">
      <animate attributeName="r" values="0;7;5" keyTimes="0;0.6;1" dur="0.5s" begin="1.0s" fill="freeze"/>
    </circle>
    <text x="280" y="24" text-anchor="middle" opacity="0">
      feat: init
      <animate attributeName="opacity" from="0" to="1" dur="0.4s" begin="1.1s" fill="freeze"/>
    </text>

    <!-- commit 2 -->
    <circle cx="480" cy="140" r="0" fill="#f778ba" filter="url(#glow)">
      <animate attributeName="r" values="0;7;5" keyTimes="0;0.6;1" dur="0.5s" begin="1.9s" fill="freeze"/>
    </circle>
    <text x="480" y="164" text-anchor="middle" opacity="0">
      fix: bug
      <animate attributeName="opacity" from="0" to="1" dur="0.4s" begin="2.0s" fill="freeze"/>
    </text>

    <!-- latest commit, pulses forever -->
    <circle cx="720" cy="100" r="0" fill="#e3b341" filter="url(#glow)">
      <animate attributeName="r" values="0;8;6" keyTimes="0;0.6;1" dur="0.5s" begin="2.7s" fill="freeze"/>
      <animate attributeName="opacity" values="1;0.4;1" dur="1.6s" begin="3.2s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- typed command line -->
  <text x="40" y="150" font-family="Consolas, Menlo, monospace" font-size="16" fill="#8b949e" opacity="0">
    git commit -m "keep shipping"
    <animate attributeName="opacity" from="0" to="1" dur="0.6s" begin="3.3s" fill="freeze"/>
  </text>

  <!-- blinking cursor -->
  <rect x="330" y="138" width="9" height="16" fill="#39d353" opacity="0">
    <animate attributeName="opacity" from="0" to="1" dur="0.1s" begin="3.3s" fill="freeze"/>
    <animate attributeName="opacity" values="1;0;1" dur="1s" begin="3.4s" repeatCount="indefinite"/>
  </rect>
</svg>
