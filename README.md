<svg xmlns="http://www.w3.org/2000/svg" width="480" height="120" viewBox="0 0 480 120">
  <defs>
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0d1117"/>
      <stop offset="100%" stop-color="#161b22"/>
    </linearGradient>
    <linearGradient id="accent" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#58a6ff"/>
      <stop offset="100%" stop-color="#79c0ff"/>
    </linearGradient>
    <clipPath id="reveal">
      <rect x="0" y="0" width="0" height="30">
        <animate attributeName="width" from="0" to="330" dur="2.6s" begin="0s;reveal.end+2.5s" fill="freeze" id="reveal"/>
      </rect>
    </clipPath>
  </defs>

  <rect x="1" y="1" width="478" height="118" rx="14" fill="url(#bg)" stroke="#30363d" stroke-width="1"/>

  <circle cx="24" cy="24" r="5" fill="#ff5f56"/>
  <circle cx="42" cy="24" r="5" fill="#ffbd2e"/>
  <circle cx="60" cy="24" r="5" fill="#27c93f"/>
  <text x="240" y="28" text-anchor="middle" font-family="Menlo, Consolas, monospace" font-size="11" fill="#8b949e">commit.sh</text>
  <line x1="0" y1="44" x2="480" y2="44" stroke="#21262d" stroke-width="1"/>

  <g transform="translate(30,62)">
    <line x1="6" y1="0" x2="6" y2="36" stroke="#30363d" stroke-width="2"/>
    <circle cx="6" cy="0" r="5" fill="#8b949e"/>
    <circle cx="6" cy="36" r="6" fill="url(#accent)">
      <animate attributeName="r" values="6;8;6" dur="1.6s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="1;0.6;1" dur="1.6s" repeatCount="indefinite"/>
    </circle>
    <circle cx="6" cy="36" r="10" fill="none" stroke="#58a6ff" stroke-width="1.5" opacity="0">
      <animate attributeName="r" values="6;16" dur="1.6s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.6;0" dur="1.6s" repeatCount="indefinite"/>
    </circle>
  </g>

  <g font-family="Menlo, Consolas, monospace" font-size="15">
    <text x="60" y="72" fill="#7ee787">$</text>
    <g clip-path="url(#reveal)">
      <text x="78" y="72" fill="#c9d1d9">git commit -m "shipped something great"</text>
    </g>
    <rect x="78" y="60" width="9" height="16" fill="#79c0ff">
      <animate attributeName="x" from="78" to="408" dur="2.6s" begin="0s;reveal.end+2.5s" fill="freeze"/>
      <animate attributeName="opacity" values="1;0;1" dur="0.8s" repeatCount="indefinite"/>
    </rect>
  </g>

  <text x="60" y="100" font-family="Menlo, Consolas, monospace" font-size="12" fill="#8b949e">
    1 file changed
    <animate attributeName="opacity" from="0" to="1" dur="0.6s" begin="reveal.end+0.2s" fill="freeze"/>
  </text>
  <text x="175" y="100" font-family="Menlo, Consolas, monospace" font-size="12" fill="#3fb950">
    +12
    <animate attributeName="opacity" from="0" to="1" dur="0.6s" begin="reveal.end+0.4s" fill="freeze"/>
  </text>
  <text x="210" y="100" font-family="Menlo, Consolas, monospace" font-size="12" fill="#f85149">
    -3
    <animate attributeName="opacity" from="0" to="1" dur="0.6s" begin="reveal.end+0.4s" fill="freeze"/>
  </text>
</svg>
