<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:00F7FF&height=150&section=header&text=Joseph%20Vijay&fontSize=45&fontColor=fff&animation=fadeIn&fontAlignY=40" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=00F7FF&center=true&vCenter=true&width=500&lines=Robotics+%7C+AI%2FML+%7C+IoT+%7C+Full-Stack;Building+real+products+from+concept+to+launch" />

<br/><br/>



![Profile Views](https://komarev.com/ghpvc/?username=YOUR-GITHUB-USERNAME&color=00F7FF&style=flat)



</div>

---

🛠 Tech Stack

<div align="center">

**Robotics & Hardware**
<br/>
<img src="https://skillicons.dev/icons?i=raspberrypi,arduino" />

**AI / ML**
<br/>
<img src="https://skillicons.dev/icons?i=tensorflow,pytorch,opencv,sklearn" />

**Languages**
<br/>
<img src="https://skillicons.dev/icons?i=python,javascript,java,c,cpp" />

**Full-Stack & Web**
<br/>
<img src="https://skillicons.dev/icons?i=react,nodejs,html,css,express" />

**Tools & Platforms**
<br/>
<img src="https://skillicons.dev/icons?i=git,github,linux,figma,docker" />

</div>


---
<picture>
  <source
    media="(prefers-color-scheme: dark)"
    srcset="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg"
  />
  <source
    media="(prefers-color-scheme: light)"
    srcset="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake.svg"
  />
  <img
    alt="github contribution grid snake animation"
    src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake.svg"
    />
</picture>
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Neural Commit Grid</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Share+Tech+Mono&display=swap');

  body {
    margin: 0;
    padding: 40px;
    background: #050508;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    font-family: 'Orbitron', sans-serif;
  }

  .ai-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 14px;
    padding: 28px;
    background: #0d1117;
    border-radius: 14px;
    font-family: 'Orbitron', sans-serif;
    color: #c9d1d9;
    width: fit-content;
    border: 1px solid #2a2a3a;
    box-shadow: 
      0 0 0 1px #21262d,
      0 20px 60px rgba(0,0,0,0.5);
    position: relative;
    overflow: hidden;
  }

  .ai-container::before {
    content: '';
    position: absolute;
    inset: 0;
    background: 
      radial-gradient(ellipse at 30% 20%, rgba(88, 166, 255, 0.05) 0%, transparent 50%),
      radial-gradient(ellipse at 70% 80%, rgba(163, 113, 247, 0.03) 0%, transparent 50%);
    pointer-events: none;
  }

  .epoch-badge {
    position: absolute;
    top: 8px;
    right: 12px;
    font-size: 9px;
    color: #484f58;
    background: #161b22;
    padding: 2px 6px;
    border-radius: 3px;
    border: 1px solid #21262d;
    font-family: 'Share Tech Mono', monospace;
  }

  .ai-header {
    font-size: 18px;
    font-weight: 700;
    color: #58a6ff;
    letter-spacing: 3px;
    text-transform: uppercase;
    text-shadow: 0 0 12px #58a6ff33;
    z-index: 5;
  }

  .neural-grid {
    display: grid;
    grid-template-columns: repeat(53, 9px);
    grid-template-rows: repeat(7, 9px);
    gap: 2px;
    position: relative;
    z-index: 5;
    padding: 12px;
    background: rgba(22, 27, 34, 0.4);
    border: 1px solid #21262d;
    border-radius: 8px;
  }

  .n-cell {
    width: 9px;
    height: 9px;
    border-radius: 1px;
    background: #161b22;
    transition: all 0.2s cubic-bezier(0.4, 0, 0.2, 1);
    position: relative;
  }

  .n-cell.infer-0 { background: #161b22; }
  .n-cell.infer-1 { background: #0e4429; }
  .n-cell.infer-2 { background: #006d32; }
  .n-cell.infer-3 { background: #26a641; box-shadow: 0 0 4px #26a64133; }
  .n-cell.infer-4 { background: #39d353; box-shadow: 0 0 6px #39d35366; }
  .n-cell.neuron {
    background: #58a6ff;
    box-shadow: 0 0 6px #58a6ff, 0 0 12px #58a6ff44;
    border-radius: 50%;
    transform: scale(1.3);
    z-index: 2;
  }
  .n-cell.synapse {
    background: #a371f7;
    box-shadow: 0 0 3px #a371f744;
  }
  .n-cell.activating {
    animation: activate 0.4s ease-out;
  }
  @keyframes activate {
    0% { transform: scale(1.8); filter: brightness(2); }
    100% { transform: scale(1); filter: brightness(1); }
  }
  .n-cell.pulse-ring::after {
    content: '';
    position: absolute;
    inset: -2px;
    border: 1px solid #39d35388;
    border-radius: 50%;
    animation: ringExpand 0.6s ease-out forwards;
    pointer-events: none;
  }
  @keyframes ringExpand {
    0% { transform: scale(0.8); opacity: 1; }
    100% { transform: scale(2.2); opacity: 0; }
  }

  .ai-metrics {
    display: flex;
    gap: 24px;
    font-size: 11px;
    margin-top: 8px;
    z-index: 5;
  }

  .metric {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 3px;
  }

  .metric-label { 
    color: #8b949e; 
    font-size: 9px; 
    font-family: 'Share Tech Mono', monospace;
    letter-spacing: 1px;
  }

  .metric-value { 
    color: #39d353; 
    font-weight: 700; 
    font-size: 16px;
    font-family: 'Share Tech Mono', monospace;
  }

  .metric-value.blue { color: #58a6ff; text-shadow: 0 0 8px #58a6ff33; }
  .metric-value.purple { color: #a371f7; text-shadow: 0 0 8px #a371f733; }
  .metric-value.green { color: #39d353; text-shadow: 0 0 8px #39d35333; }

  .loss-graph {
    width: 320px;
    height: 40px;
    background: #161b22;
    border-radius: 4px;
    position: relative;
    overflow: hidden;
    border: 1px solid #21262d;
    z-index: 5;
  }

  .loss-line {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    height: 100%;
  }

  .loss-line svg { width: 100%; height: 100%; }

  .phase-indicator {
    position: absolute;
    bottom: 8px;
    left: 12px;
    font-size: 9px;
    color: #484f58;
    font-family: 'Share Tech Mono', monospace;
    letter-spacing: 1px;
    z-index: 5;
  }
</style>
</head>
<body>

<div class="ai-container">
  <div class="epoch-badge" id="epochBadge">Epoch 0</div>
  <div class="ai-header">Neural Commit Grid</div>

  <div class="neural-grid" id="nGrid"></div>

  <div class="loss-graph">
    <div class="loss-line" id="lossLine"></div>
  </div>

  <div class="ai-metrics">
    <div class="metric">
      <div class="metric-label">Neurons</div>
      <div class="metric-value blue" id="neuronCount">0</div>
    </div>
    <div class="metric">
      <div class="metric-label">Activations</div>
      <div class="metric-value green" id="activationCount">0</div>
    </div>
    <div class="metric">
      <div class="metric-label">Loss</div>
      <div class="metric-value purple" id="lossVal">1.000</div>
    </div>
    <div class="metric">
      <div class="metric-label">Accuracy</div>
      <div class="metric-value" id="accVal">0%</div>
    </div>
  </div>

  <div class="phase-indicator" id="phaseInd">Phase: FORWARD_PASS</div>
</div>

<script>
  const nGrid = document.getElementById('nGrid');
  const neuronEl = document.getElementById('neuronCount');
  const actEl = document.getElementById('activationCount');
  const lossEl = document.getElementById('lossVal');
  const accEl = document.getElementById('accVal');
  const epochEl = document.getElementById('epochBadge');
  const lossLine = document.getElementById('lossLine');
  const phaseInd = document.getElementById('phaseInd');

  const COLS = 53;
  const ROWS = 7;
  const cells = [];
  const neurons = [];
  let epoch = 0;
  let loss = 1.0;
  let accuracy = 0;
  let totalActivations = 0;
  let lossHistory = [];
  let phase = 'forward';
  let phaseTimer = 0;
  let synapsePaths = [];

  for (let r = 0; r < ROWS; r++) {
    for (let c = 0; c < COLS; c++) {
      const cell = document.createElement('div');
      cell.className = 'n-cell';
      nGrid.appendChild(cell);
      cells.push({
        el: cell,
        x: c, y: r,
        isNeuron: false,
        activation: 0,
        weight: Math.random() * 2 - 1,
        gradient: 0
      });
    }
  }

  function idx(x, y) { return y * COLS + x; }
  function get(x, y) {
    if (x < 0 || x >= COLS || y < 0 || y >= ROWS) return null;
    return cells[idx(x, y)];
  }

  function spawnNeuronLayer() {
    neurons.length = 0;
    const layers = [8, 18, 28, 38, 48];
    layers.forEach((lx, li) => {
      const count = li === 0 || li === 4 ? 3 : 5;
      const startY = Math.floor((ROWS - count) / 2);
      for (let i = 0; i < count; i++) {
        const cell = get(lx, startY + i);
        if (cell) {
          cell.isNeuron = true;
          cell.activation = Math.random();
          neurons.push(cell);
          cell.el.className = 'n-cell neuron';
        }
      }
    });
  }

  function drawSynapses() {
    cells.forEach(c => {
      if (!c.isNeuron && c.el.classList.contains('synapse')) {
        c.el.className = 'n-cell';
      }
    });

    for (let i = 0; i < neurons.length; i++) {
      for (let j = i + 1; j < neurons.length; j++) {
        const a = neurons[i];
        const b = neurons[j];
        const dist = Math.sqrt((a.x - b.x)**2 + (a.y - b.y)**2);
        if (dist < 12 && dist > 2) {
          const steps = Math.ceil(dist);
          for (let s = 1; s < steps; s++) {
            const tx = Math.round(a.x + (b.x - a.x) * (s / steps));
            const ty = Math.round(a.y + (b.y - a.y) * (s / steps));
            const cell = get(tx, ty);
            if (cell && !cell.isNeuron && Math.random() > 0.3) {
              cell.el.className = 'n-cell synapse';
            }
          }
        }
      }
    }
  }

  function forwardPass() {
    phase = 'forward';
    phaseInd.textContent = 'Phase: FORWARD_PASS';
    const startY = Math.floor(Math.random() * ROWS);
    let cx = 0;
    let cy = startY;

    const path = [];
    while (cx < COLS) {
      const cell = get(cx, cy);
      if (cell) {
        path.push(cell);
        cell.activation = Math.min(4, cell.activation + 1);
        cell.el.className = 'n-cell infer-' + Math.min(4, cell.activation) + ' activating';
        if (Math.random() > 0.7) {
          cell.el.classList.add('pulse-ring');
          setTimeout(() => cell.el.classList.remove('pulse-ring'), 600);
        }
        totalActivations++;
      }
      cx += Math.floor(Math.random() * 2) + 1;
      cy += Math.floor(Math.random() * 3) - 1;
      cy = Math.max(0, Math.min(ROWS - 1, cy));
    }

    neurons.forEach(n => {
      n.activation = Math.random() * 4;
      const level = Math.min(4, Math.floor(n.activation));
      n.el.className = 'n-cell neuron infer-' + level + ' activating';
    });
  }

  function backprop() {
    phase = 'backprop';
    phaseInd.textContent = 'Phase: BACKPROP';
    for (let i = 0; i < 15; i++) {
      const x = Math.floor(Math.random() * COLS);
      const y = Math.floor(Math.random() * ROWS);
      const cell = get(x, y);
      if (cell && !cell.isNeuron) {
        cell.el.style.background = '#a371f7';
        cell.el.style.boxShadow = '0 0 4px #a371f7';
        setTimeout(() => {
          cell.el.style.background = '';
          cell.el.style.boxShadow = '';
          const level = Math.min(4, Math.floor(cell.activation));
          cell.el.className = 'n-cell infer-' + level;
        }, 300);
      }
    }

    loss = Math.max(0.01, loss * 0.95 + Math.random() * 0.05);
    accuracy = Math.min(99.9, accuracy + Math.random() * 3);
  }

  function optimize() {
    phase = 'optimize';
    phaseInd.textContent = 'Phase: OPTIMIZE';
    cells.forEach(c => {
      if (!c.isNeuron && c.activation > 0) {
        c.activation = Math.max(0, c.activation - 0.5);
        const level = Math.min(4, Math.floor(c.activation));
        c.el.className = 'n-cell infer-' + level;
      }
    });

    loss = Math.max(0.001, loss * 0.92);
    accuracy = Math.min(99.9, accuracy + 1);

    epoch++;
    epochEl.textContent = 'Epoch ' + epoch;

    lossHistory.push(loss);
    if (lossHistory.length > 50) lossHistory.shift();
    drawLossGraph();
  }

  function drawLossGraph() {
    if (lossHistory.length < 2) return;
    const maxLoss = Math.max(...lossHistory, 1);
    const width = 320;
    const height = 40;
    let path = `M0,${height}`;
    lossHistory.forEach((l, i) => {
      const x = (i / (lossHistory.length - 1)) * width;
      const y = height - (l / maxLoss) * height * 0.9;
      path += ` L${x},${y}`;
    });
    lossLine.innerHTML = `
      <svg viewBox="0 0 ${width} ${height}" preserveAspectRatio="none">
        <path d="${path}" fill="none" stroke="#a371f7" stroke-width="1.5" opacity="0.8"/>
        <path d="${path} L${width},${height} L0,${height}" fill="url(#grad)" opacity="0.15"/>
        <defs>
          <linearGradient id="grad" x1="0" y1="0" x2="0" y2="1">
            <stop offset="0%" stop-color="#a371f7"/>
            <stop offset="100%" stop-color="#a371f7" stop-opacity="0"/>
          </linearGradient>
        </defs>
      </svg>
    `;
  }

  function updateMetrics() {
    neuronEl.textContent = neurons.length;
    actEl.textContent = totalActivations.toLocaleString();
    lossEl.textContent = loss.toFixed(3);
    accEl.textContent = accuracy.toFixed(1) + '%';
  }

  spawnNeuronLayer();
  drawSynapses();

  let tick = 0;
  function loop() {
    tick++;

    if (tick % 3 === 0) forwardPass();
    if (tick % 20 === 0) backprop();
    if (tick % 40 === 0) optimize();
    if (tick % 100 === 0) drawSynapses();

    updateMetrics();
    requestAnimationFrame(loop);
  }

  requestAnimationFrame(loop);
</script>

</body>
</html>

