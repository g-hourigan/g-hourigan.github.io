---
layout: default
title: Home
permalink: /
---

<style>
  .masthead,
  .masthead__inner-wrap,
  .greedy-nav,
  .page__footer,
  .author__avatar,
  .author__content,
  .page__meta,
  .pagination,
  .toc,
  .sidebar {
    display: none !important;
  }

  .initial-content {
    margin-top: 0 !important;
  }

  .layout--default .page,
  .layout--single .page {
    float: none !important;
    width: 100% !important;
    padding-right: 0 !important;
  }

  .page__inner-wrap,
  .page__content {
    max-width: none !important;
    width: 100% !important;
    margin: 0 !important;
    padding: 0 !important;
  }

  html {
    scroll-behavior: smooth;
  }

  body {
    margin: 0;
    background:
      radial-gradient(circle at 18% 20%, rgba(0, 212, 255, 0.06), transparent 28%),
      radial-gradient(circle at 82% 18%, rgba(255, 78, 205, 0.05), transparent 22%),
      radial-gradient(circle at 50% 82%, rgba(0, 212, 255, 0.04), transparent 28%),
      #050914;
    color: #dbe7ef;
    font-family: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    overflow-x: hidden;
  }

  ::selection {
    background: rgba(255, 78, 205, 0.24);
    color: #ffffff;
  }

  ::-moz-selection {
    background: rgba(255, 78, 205, 0.24);
    color: #ffffff;
  }

  #p5-network-bg {
    position: fixed;
    inset: 0;
    z-index: 0;
    pointer-events: none;
    opacity: 1;
    filter: saturate(1.15) brightness(1.08);
  }

  #p5-network-bg canvas {
    display: block;
    width: 100% !important;
    height: 100% !important;
  }

  .site-shell {
    position: relative;
    z-index: 1;
    max-width: 1120px;
    margin: 0 auto;
    padding: 2.4rem 1.2rem 3rem;
  }

  .site-panel {
    position: relative;
    overflow: hidden;
    border: 1px solid rgba(111, 142, 182, 0.18);
    border-radius: 28px;
    background: linear-gradient(
      180deg,
      rgba(8, 13, 24, 0.86) 0%,
      rgba(6, 10, 18, 0.93) 100%
    );
    box-shadow:
      0 0 0 1px rgba(255, 255, 255, 0.02) inset,
      0 30px 80px rgba(0, 0, 0, 0.35),
      0 0 80px rgba(0, 212, 255, 0.05);
    backdrop-filter: blur(12px);
    -webkit-backdrop-filter: blur(12px);
    padding: 2rem 2rem 1.6rem;
  }

  .site-panel::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
      linear-gradient(90deg, rgba(0, 212, 255, 0.05), transparent 18%, transparent 82%, rgba(255, 78, 205, 0.04)),
      linear-gradient(180deg, rgba(255, 255, 255, 0.02), transparent 25%);
    pointer-events: none;
  }

  .section-label {
    position: relative;
    z-index: 1;
    margin: 0 0 0.9rem;
    font-size: 0.92rem;
    font-weight: 700;
    letter-spacing: 0.18em;
    color: #8c99ad;
    text-transform: uppercase;
  }

  .section-divider {
    position: relative;
    z-index: 1;
    height: 1px;
    margin: 1.9rem 0 1.45rem;
    background: linear-gradient(
      90deg,
      rgba(255, 255, 255, 0.08),
      rgba(255, 255, 255, 0.02)
    );
  }

  .hero-title {
    position: relative;
    z-index: 1;
    margin: 0;
    max-width: 950px;
    font-size: clamp(2.5rem, 5vw, 4.3rem);
    line-height: 1.02;
    letter-spacing: -0.055em;
    font-weight: 800;
    color: #f4f8fb;
  }

  .hero-subtitle {
    position: relative;
    z-index: 1;
    max-width: 760px;
    margin: 0.95rem 0 0;
    font-size: 1.02rem;
    line-height: 1.75;
    color: #9fb0c2;
  }

  .hero-links {
    position: relative;
    z-index: 1;
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem;
    margin-top: 1.2rem;
  }

  .hero-links a,
  .link-inline,
  .project-link,
  .contact-links a {
    color: #00d4ff !important;
    text-decoration: none !important;
    transition: color 0.2s ease, border-color 0.2s ease, transform 0.2s ease;
  }

  .hero-links a {
    display: inline-flex;
    align-items: center;
    gap: 0.4rem;
    padding: 0.62rem 0.95rem;
    border: 1px solid rgba(0, 212, 255, 0.18);
    border-radius: 999px;
    background: rgba(9, 16, 28, 0.82);
    font-size: 0.92rem;
    font-weight: 700;
    color: #dffaff !important;
  }

  .hero-links a:hover,
  .contact-links a:hover,
  .link-inline:hover,
  .project-link:hover {
    color: #ff71d6 !important;
    border-color: rgba(255, 113, 214, 0.32);
    transform: translateY(-1px);
  }

  .welcome-card,
  .info-card,
  .project-card {
    position: relative;
    z-index: 1;
    border: 1px solid rgba(114, 134, 170, 0.18);
    border-radius: 18px;
    background: linear-gradient(
      180deg,
      rgba(14, 21, 35, 0.92),
      rgba(9, 15, 26, 0.92)
    );
    box-shadow: 0 12px 30px rgba(0, 0, 0, 0.18);
  }

  .welcome-card {
    margin-top: 1.45rem;
    padding: 1.3rem 1.35rem;
  }

  .welcome-card p,
  .info-card p,
  .project-card p {
    margin: 0;
    color: #aebdca;
    line-height: 1.72;
  }

  .welcome-card p + p {
    margin-top: 0.7rem;
  }

  .welcome-nav {
    margin-top: 0.9rem;
    color: #dbe7ef;
    font-size: 0.98rem;
  }

  .welcome-nav span {
    color: #8c99ad;
    margin-right: 0.45rem;
  }

  .cards-grid {
    position: relative;
    z-index: 1;
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
  }

  .info-card {
    padding: 1.1rem 1.15rem;
  }

  .card-title {
    margin: 0 0 0.55rem;
    font-size: 0.98rem;
    font-weight: 800;
    letter-spacing: 0.08em;
    color: #f2f7fb;
    text-transform: uppercase;
  }

  .project-card {
    padding: 1.25rem 1.2rem;
  }

  .project-card h3 {
    margin: 0 0 0.55rem;
    font-size: 1.35rem;
    line-height: 1.25;
    color: #f7fbff;
  }

  .project-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.48rem;
    margin: 1rem 0 0.95rem;
  }

  .project-tags span {
    display: inline-flex;
    align-items: center;
    padding: 0.28rem 0.62rem;
    border-radius: 999px;
    border: 1px solid rgba(170, 187, 211, 0.16);
    background: rgba(255, 255, 255, 0.03);
    color: #a9b6c4;
    font-size: 0.74rem;
    font-weight: 700;
    letter-spacing: 0.03em;
  }

  .project-link {
    display: inline-block;
    font-weight: 700;
    font-size: 0.95rem;
  }

  .contact-row {
    position: relative;
    z-index: 1;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 0.9rem;
    color: #dbe7ef;
    font-size: 1rem;
  }

  .contact-links {
    display: flex;
    flex-wrap: wrap;
    gap: 0.9rem;
    align-items: center;
  }

  .contact-links .sep {
    color: #4f5d74;
  }

  .footer-row {
    position: relative;
    z-index: 1;
    display: grid;
    grid-template-columns: 1fr auto;
    gap: 1rem;
    align-items: start;
    margin-top: 0.2rem;
    color: #93a1b0;
  }

  .copyright {
    font-size: 0.95rem;
    line-height: 1.7;
  }

  .system-meta {
    text-align: right;
    font-size: 0.95rem;
    line-height: 1.75;
    color: #98a6b6;
  }

  .status-live {
    color: #4cff9e;
    font-weight: 800;
  }

  .meta-note {
    margin-top: 1rem;
    font-size: 0.95rem;
    line-height: 1.7;
    color: #6f7e92;
    font-style: italic;
  }

  @media (max-width: 900px) {
    .site-shell {
      padding: 1.2rem 0.8rem 2rem;
    }

    .site-panel {
      border-radius: 22px;
      padding: 1.35rem 1.1rem 1.2rem;
    }

    .cards-grid,
    .footer-row {
      grid-template-columns: 1fr;
    }

    .footer-row,
    .system-meta {
      text-align: left;
    }

    .hero-subtitle {
      font-size: 1rem;
    }
  }

  @media (max-width: 640px) {
    .hero-links {
      gap: 0.6rem;
    }

    .hero-links a {
      width: 100%;
      justify-content: center;
    }

    .contact-links {
      gap: 0.55rem;
    }

    .contact-links .sep {
      display: none;
    }
  }
</style>

<div id="p5-network-bg" aria-hidden="true"></div>

<section class="site-shell">
  <div class="site-panel">
    <p class="section-label">// HOME</p>

    <h1 class="hero-title">Gerrit Hourigan</h1>

    <p class="hero-subtitle">
      Psychology, behavioral data, cognitive science, and quantitative research.
    </p>

    <div class="hero-links">
      <a href="/cv/">CV</a>
      <a href="mailto:gerrithourigan@gmail.com">Email</a>
      <a href="https://github.com/g-hourigan" target="_blank" rel="noopener noreferrer">GitHub</a>
    </div>

    <div class="welcome-card">
      <p>
        Hi, I’m Gerrit. I’m interested in psychology, cognition, and the analysis of
        behavioral data. Most of my work sits around quantitative research, individual
        differences, and questions that can be studied with careful modeling.
      </p>

      <p>
        I completed my B.Sc. in Psychology at Leuphana University Lüneburg and am
        continuing into the M.Sc. while working on research and data analysis projects.
        Outside academia, I’m also a competitive chess player.
      </p>

      <div class="welcome-nav">
        <span>Navigate:</span>
        <a class="link-inline" href="/cv/">[ cv ]</a>
        &nbsp;|&nbsp;
        <a class="link-inline" href="/projects/life-events-rca/">[ project ]</a>
      </div>
    </div>

    <div class="section-divider"></div>

    <p class="section-label">// CURRENT FOCUS</p>

    <div class="cards-grid">
      <div class="info-card">
        <p class="card-title">Research</p>
        <p>
          Latent variables, longitudinal data, measurement, individual differences,
          and behavioral outcomes that matter outside highly artificial settings.
        </p>
      </div>

      <div class="info-card">
        <p class="card-title">Tools</p>
        <p>
          R, SEM, survey-data workflows, reproducible analysis, and increasingly
          machine-learning methods for behavioral and cognitive data.
        </p>
      </div>
    </div>

    <div class="section-divider"></div>

    <p class="section-label">// SELECTED PROJECT</p>

    <div class="project-card">
      <h3>Life Events and Climate Action Readiness</h3>

      <p>
        I tested whether life events measured at T3 predicted latent change in
        readiness for climate action from T1 to T3. The project involved survey-data
        preparation, measurement invariance testing, structural equation modeling,
        and latent change modeling in R.
      </p>

      <div class="project-tags">
        <span>R</span>
        <span>lavaan</span>
        <span>SEM</span>
        <span>Longitudinal Modeling</span>
        <span>Latent Variables</span>
        <span>Survey Data</span>
      </div>

      <a class="project-link" href="/projects/life-events-rca/">
        Read project →
      </a>
    </div>

    <div class="section-divider"></div>

    <p class="section-label">// CONTACT</p>

    <div class="contact-row">
      <div class="contact-links">
        <a href="/cv/">CV</a>
        <span class="sep">|</span>
        <a href="mailto:gerrithourigan@gmail.com">Email</a>
        <span class="sep">|</span>
        <a href="https://github.com/g-hourigan" target="_blank" rel="noopener noreferrer">GitHub</a>
      </div>
    </div>

    <div class="section-divider"></div>

    <div class="footer-row">
      <div class="copyright">
        © 2026 Gerrit Hourigan<br>
        All Rights Reserved.
      </div>

      <div class="system-meta">
        STATUS: <span class="status-live">ACTIVE</span><br>
        BUILD: PSYCHOLOGY × DATA
      </div>
    </div>

    <p class="meta-note">
      Interface: GitHub Pages / Jekyll / p5.js background sketch.
    </p>
  </div>
</section>

<script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.9.4/p5.min.js"></script>
<script>
  let clusters = [];
  let strayNodes = [];
  let bridgePairs = [];
  let pointerActive = false;

  const CURSOR_RADIUS = 240;
  const CURSOR_PULL = 0.085;
  const CURSOR_CONNECTION_RADIUS = 220;

  function setup() {
    const parent = document.getElementById("p5-network-bg");
    const cnv = createCanvas(windowWidth, windowHeight);
    cnv.parent(parent);
    noFill();
    pixelDensity(Math.min(window.devicePixelRatio || 1, 2));
  }

  function draw() {
    clear();

    if (!clusters.length) {
      buildScene();
    }

    const t = millis() * 0.001;

    drawBackgroundGlow();
    updateClusters(t);
    updateStrayNodes();
    drawClusterConnections();
    drawBridges();
    drawPointerConnections();
    drawNodes();
  }

  function windowResized() {
    resizeCanvas(windowWidth, windowHeight);
    buildScene();
  }

  function buildScene() {
    clusters = [];
    strayNodes = [];
    bridgePairs = [];

    const mobile = windowWidth < 760;

    const layout = mobile
      ? [
          { x: width * 0.08, y: height * 0.74, count: 9, spread: 36 },
          { x: width * 0.92, y: height * 0.20, count: 11, spread: 48 },
          { x: width * 0.90, y: height * 0.58, count: 8, spread: 34 }
        ]
      : [
          { x: width * 0.06, y: height * 0.74, count: 10, spread: 36 },
          { x: width * 0.13, y: height * 0.26, count: 6, spread: 26 },
          { x: width * 0.94, y: height * 0.18, count: 12, spread: 56 },
          { x: width * 0.91, y: height * 0.53, count: 9, spread: 40 },
          { x: width * 0.76, y: height * 0.92, count: 7, spread: 34 }
        ];

    for (let i = 0; i < layout.length; i++) {
      const item = layout[i];

      const cluster = {
        baseX: item.x,
        baseY: item.y,
        x: item.x,
        y: item.y,
        spread: item.spread,
        ampX: random(4, 14),
        ampY: random(4, 14),
        phaseX: random(TWO_PI),
        phaseY: random(TWO_PI),
        nodes: []
      };

      for (let j = 0; j < item.count; j++) {
        const angle = random(TWO_PI);
        const radius = random(item.spread * 0.18, item.spread);
        const accent = random() > 0.72;
        const cyan = random() > 0.5;

        cluster.nodes.push({
          ox: cos(angle) * radius,
          oy: sin(angle) * radius,
          x: cluster.x,
          y: cluster.y,
          vx: 0,
          vy: 0,
          phase: random(TWO_PI),
          wobble: random(1.2, 3.2),
          r: accent ? random(2.1, 2.9) : random(1.3, 1.9),
          color: accent
            ? (cyan ? [0, 212, 255] : [255, 78, 205])
            : [214, 225, 240]
        });
      }

      clusters.push(cluster);
    }

    for (let i = 0; i < clusters.length; i++) {
      for (let j = i + 1; j < clusters.length; j++) {
        const a = clusters[i];
        const b = clusters[j];
        const d = dist(a.baseX, a.baseY, b.baseX, b.baseY);

        if (d < min(width, height) * 0.44) {
          bridgePairs.push([i, j]);
        }
      }
    }

    const strayCount = mobile ? 3 : 6;

    for (let i = 0; i < strayCount; i++) {
      strayNodes.push({
        x: i % 2 === 0 ? random(24, width * 0.22) : random(width * 0.78, width - 24),
        y: random(24, height - 24),
        vx: random(-0.08, 0.08),
        vy: random(-0.08, 0.08),
        r: random(1.8, 2.6),
        color: random() > 0.5 ? [255, 78, 205] : [0, 212, 255]
      });
    }
  }

  function drawBackgroundGlow() {
    noStroke();

    fill(0, 212, 255, 6);
    circle(width * 0.5, height * 0.5, max(width, height) * 0.82);

    fill(255, 78, 205, 4);
    circle(width * 0.52, height * 0.47, max(width, height) * 0.60);

    fill(0, 212, 255, 3);
    circle(width * 0.47, height * 0.54, max(width, height) * 1.02);
  }

  function updateClusters(t) {
    for (const cluster of clusters) {
      cluster.x = cluster.baseX + sin(t * 0.48 + cluster.phaseX) * cluster.ampX;
      cluster.y = cluster.baseY + cos(t * 0.42 + cluster.phaseY) * cluster.ampY;

      for (const node of cluster.nodes) {
        const tx = cluster.x + node.ox + cos(t * 1.18 + node.phase) * node.wobble;
        const ty = cluster.y + node.oy + sin(t * 1.05 + node.phase) * node.wobble;

        node.vx += (tx - node.x) * 0.03;
        node.vy += (ty - node.y) * 0.03;

        if (pointerActive) {
          const dx = mouseX - node.x;
          const dy = mouseY - node.y;
          const d = sqrt(dx * dx + dy * dy);

          if (d < CURSOR_RADIUS && d > 0.001) {
            const falloff = 1 - d / CURSOR_RADIUS;
            const pull = falloff * CURSOR_PULL;

            node.vx += dx * pull * 0.035;
            node.vy += dy * pull * 0.035;
          }
        }

        node.vx *= 0.89;
        node.vy *= 0.89;

        node.x += node.vx;
        node.y += node.vy;
      }
    }
  }

  function updateStrayNodes() {
    for (const node of strayNodes) {
      node.x += node.vx;
      node.y += node.vy;

      if (node.x < 8 || node.x > width - 8) node.vx *= -1;
      if (node.y < 8 || node.y > height - 8) node.vy *= -1;
    }
  }

  function drawGlowLine(x1, y1, x2, y2, col, alphaCore, alphaGlow, coreWeight, glowWeight) {
    push();
    drawingContext.shadowBlur = 16;
    drawingContext.shadowColor = `rgba(${col[0]}, ${col[1]}, ${col[2]}, ${alphaGlow / 255})`;
    stroke(col[0], col[1], col[2], alphaGlow);
    strokeWeight(glowWeight);
    line(x1, y1, x2, y2);
    pop();

    stroke(col[0], col[1], col[2], alphaCore);
    strokeWeight(coreWeight);
    line(x1, y1, x2, y2);
  }

  function drawClusterConnections() {
    for (const cluster of clusters) {
      for (let i = 0; i < cluster.nodes.length; i++) {
        const a = cluster.nodes[i];
        const neighbors = [];

        for (let j = 0; j < cluster.nodes.length; j++) {
          if (i === j) continue;

          const b = cluster.nodes[j];
          neighbors.push({
            node: b,
            d: dist(a.x, a.y, b.x, b.y)
          });
        }

        neighbors.sort((m, n) => m.d - n.d);

        for (const item of neighbors.slice(0, 3)) {
          const alpha = max(0.1, 1 - item.d / (cluster.spread * 2.4));
          drawGlowLine(
            a.x,
            a.y,
            item.node.x,
            item.node.y,
            [0, 212, 255],
            80 * alpha,
            42 * alpha,
            1,
            2.6
          );
        }
      }
    }
  }

  function drawBridges() {
    for (const pair of bridgePairs) {
      const clusterA = clusters[pair[0]];
      const clusterB = clusters[pair[1]];

      let bestA = null;
      let bestB = null;
      let bestD = Infinity;

      for (const a of clusterA.nodes) {
        for (const b of clusterB.nodes) {
          const d = dist(a.x, a.y, b.x, b.y);
          if (d < bestD) {
            bestD = d;
            bestA = a;
            bestB = b;
          }
        }
      }

      if (bestA && bestB) {
        const alpha = bestD < 220 ? 1 : 0.45;
        drawGlowLine(
          bestA.x,
          bestA.y,
          bestB.x,
          bestB.y,
          [0, 212, 255],
          70 * alpha,
          34 * alpha,
          1,
          2.2
        );
      }
    }
  }

  function drawPointerConnections() {
    if (!pointerActive) return;

    const allNodes = [
      ...clusters.flatMap(cluster => cluster.nodes),
      ...strayNodes
    ];

    let nearby = 0;

    for (const node of allNodes) {
      const d = dist(mouseX, mouseY, node.x, node.y);

      if (d < CURSOR_CONNECTION_RADIUS) {
        nearby++;
        const alpha = 1 - d / CURSOR_CONNECTION_RADIUS;

        drawGlowLine(
          mouseX,
          mouseY,
          node.x,
          node.y,
          node.color,
          130 * alpha,
          65 * alpha,
          1,
          2.8
        );
      }
    }

    if (nearby > 0) {
      noStroke();

      push();
      drawingContext.shadowBlur = 18;
      drawingContext.shadowColor = "rgba(0,212,255,0.9)";
      fill(255, 255, 255, 240);
      circle(mouseX, mouseY, 6.5);
      pop();

      fill(0, 212, 255, 18);
      circle(mouseX, mouseY, 28);

      fill(0, 212, 255, 8);
      circle(mouseX, mouseY, 52);
    }
  }

  function drawNodes() {
    const allNodes = [
      ...clusters.flatMap(cluster => cluster.nodes),
      ...strayNodes
    ];

    noStroke();

    for (const node of allNodes) {
      fill(node.color[0], node.color[1], node.color[2], 18);
      circle(node.x, node.y, node.r * 5.8);

      push();
      drawingContext.shadowBlur = 14;
      drawingContext.shadowColor = `rgba(${node.color[0]}, ${node.color[1]}, ${node.color[2]}, 0.9)`;
      fill(node.color[0], node.color[1], node.color[2], 250);
      circle(node.x, node.y, node.r * 2.15);
      pop();
    }
  }

  function mouseMoved() {
    pointerActive = true;
  }

  function mouseDragged() {
    pointerActive = true;
  }

  function mouseOut() {
    pointerActive = false;
  }

  function touchMoved() {
    pointerActive = true;
    return true;
  }

  function touchEnded() {
    pointerActive = false;
  }
</script>
