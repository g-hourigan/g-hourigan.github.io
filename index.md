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
    filter: saturate(1.1) brightness(1.04);
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
      Psychology, cognition, behavioral data, and quantitative research.
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
  let nodes = [];
  let edges = [];
  let pointerBound = false;

  const pointer = {
    x: 0,
    y: 0,
    tx: 0,
    ty: 0,
    active: false
  };

  const CONFIG = {
    mobileBreakpoint: 760,
    pointerLerp: 0.18,
    nodeLerp: 0.14,
    cursorRadius: 190,
    cursorLineRadius: 170,
    maxPull: 24,
    clusterNeighborCount: 3
  };

  function setup() {
    const parent = document.getElementById("p5-network-bg");
    const cnv = createCanvas(windowWidth, windowHeight);
    cnv.parent(parent);
    pixelDensity(Math.min(window.devicePixelRatio || 1, 2));
    noFill();
    strokeCap(ROUND);
    buildScene();

    if (!pointerBound) {
      bindPointerEvents();
      pointerBound = true;
    }
  }

  function windowResized() {
    resizeCanvas(windowWidth, windowHeight);
    buildScene();
  }

  function draw() {
    clear();
    updatePointer();
    updateNodePositions();
    drawBackgroundGlow();
    drawEdges();
    drawPointerLines();
    drawNodes();
  }

  function bindPointerEvents() {
    window.addEventListener("pointermove", (e) => {
      pointer.tx = e.clientX;
      pointer.ty = e.clientY;

      if (!pointer.active) {
        pointer.x = e.clientX;
        pointer.y = e.clientY;
      }

      pointer.active = true;
    });

    window.addEventListener("pointerdown", (e) => {
      pointer.tx = e.clientX;
      pointer.ty = e.clientY;
      pointer.x = e.clientX;
      pointer.y = e.clientY;
      pointer.active = true;
    });

    document.addEventListener("pointerleave", () => {
      pointer.active = false;
    });

    window.addEventListener("pointercancel", () => {
      pointer.active = false;
    });

    window.addEventListener("mouseout", (e) => {
      if (!e.relatedTarget && !e.toElement) {
        pointer.active = false;
      }
    });
  }

  function updatePointer() {
    if (!pointer.active) return;
    pointer.x = lerp(pointer.x, pointer.tx, CONFIG.pointerLerp);
    pointer.y = lerp(pointer.y, pointer.ty, CONFIG.pointerLerp);
  }

  function buildScene() {
    nodes = [];
    edges = [];

    const mobile = width < CONFIG.mobileBreakpoint;

    const clusterDefs = mobile
      ? [
          { x: width * 0.08, y: height * 0.76, count: 8, spread: 30 },
          { x: width * 0.92, y: height * 0.22, count: 10, spread: 40 },
          { x: width * 0.90, y: height * 0.58, count: 6, spread: 30 }
        ]
      : [
          { x: width * 0.07, y: height * 0.76, count: 9, spread: 30 },
          { x: width * 0.14, y: height * 0.30, count: 4, spread: 22 },
          { x: width * 0.93, y: height * 0.18, count: 11, spread: 48 },
          { x: width * 0.90, y: height * 0.54, count: 7, spread: 34 },
          { x: width * 0.76, y: height * 0.91, count: 5, spread: 28 }
        ];

    const groups = [];

    for (const cluster of clusterDefs) {
      const group = [];

      for (let i = 0; i < cluster.count; i++) {
        const angle = random(TWO_PI);
        const radius = random(cluster.spread * 0.2, cluster.spread);
        const accent = random() > 0.72;
        const cyan = random() > 0.5;

        const homeX = cluster.x + cos(angle) * radius;
        const homeY = cluster.y + sin(angle) * radius;

        const node = {
          homeX,
          homeY,
          x: homeX,
          y: homeY,
          phaseX: random(TWO_PI),
          phaseY: random(TWO_PI),
          driftX: random(2.0, 4.8),
          driftY: random(2.0, 4.8),
          r: accent ? random(2.0, 2.8) : random(1.2, 1.7),
          color: accent
            ? (cyan ? [0, 212, 255] : [255, 78, 205])
            : [214, 225, 240]
        };

        const idx = nodes.push(node) - 1;
        group.push(idx);
      }

      groups.push(group);
    }

    for (const group of groups) {
      const groupEdges = buildGroupEdges(group, CONFIG.clusterNeighborCount);
      edges.push(...groupEdges);
    }

    for (let i = 0; i < groups.length; i++) {
      for (let j = i + 1; j < groups.length; j++) {
        const centerA = getGroupCenter(groups[i]);
        const centerB = getGroupCenter(groups[j]);
        const d = Math.hypot(centerA.x - centerB.x, centerA.y - centerB.y);

        if (d < Math.min(width, height) * 0.42) {
          const pair = findClosestPair(groups[i], groups[j]);
          if (pair) {
            edges.push({
              a: pair[0],
              b: pair[1],
              type: "bridge",
              color: [0, 212, 255]
            });
          }
        }
      }
    }

    const strayCount = mobile ? 2 : 4;

    for (let i = 0; i < strayCount; i++) {
      const x = i % 2 === 0
        ? random(24, width * 0.22)
        : random(width * 0.78, width - 24);

      const y = random(24, height - 24);

      nodes.push({
        homeX: x,
        homeY: y,
        x,
        y,
        phaseX: random(TWO_PI),
        phaseY: random(TWO_PI),
        driftX: random(1.4, 3.0),
        driftY: random(1.4, 3.0),
        r: random(1.6, 2.2),
        color: random() > 0.5 ? [255, 78, 205] : [0, 212, 255]
      });
    }
  }

  function buildGroupEdges(group, k) {
    const found = new Set();
    const result = [];

    for (const aIdx of group) {
      const candidates = [];

      for (const bIdx of group) {
        if (aIdx === bIdx) continue;

        const a = nodes[aIdx];
        const b = nodes[bIdx];
        const d = Math.hypot(a.homeX - b.homeX, a.homeY - b.homeY);

        candidates.push({ idx: bIdx, d });
      }

      candidates.sort((m, n) => m.d - n.d);

      for (const candidate of candidates.slice(0, k)) {
        const low = Math.min(aIdx, candidate.idx);
        const high = Math.max(aIdx, candidate.idx);
        const key = `${low}-${high}`;

        if (!found.has(key)) {
          found.add(key);
          result.push({
            a: low,
            b: high,
            type: "cluster",
            color: [0, 212, 255]
          });
        }
      }
    }

    return result;
  }

  function getGroupCenter(group) {
    let sx = 0;
    let sy = 0;

    for (const idx of group) {
      sx += nodes[idx].homeX;
      sy += nodes[idx].homeY;
    }

    return {
      x: sx / group.length,
      y: sy / group.length
    };
  }

  function findClosestPair(groupA, groupB) {
    let best = null;
    let bestD = Infinity;

    for (const aIdx of groupA) {
      for (const bIdx of groupB) {
        const a = nodes[aIdx];
        const b = nodes[bIdx];
        const d = Math.hypot(a.homeX - b.homeX, a.homeY - b.homeY);

        if (d < bestD) {
          bestD = d;
          best = [aIdx, bIdx];
        }
      }
    }

    return best;
  }

  function updateNodePositions() {
    const t = millis() * 0.001;

    for (const node of nodes) {
      let targetX = node.homeX + Math.cos(t * 0.78 + node.phaseX) * node.driftX;
      let targetY = node.homeY + Math.sin(t * 0.84 + node.phaseY) * node.driftY;

      if (pointer.active) {
        const dx = pointer.x - targetX;
        const dy = pointer.y - targetY;
        const d = Math.hypot(dx, dy);

        if (d < CONFIG.cursorRadius && d > 0.001) {
          const influence = 1 - d / CONFIG.cursorRadius;
          const pull = influence * influence * CONFIG.maxPull;
          targetX += (dx / d) * pull;
          targetY += (dy / d) * pull;
        }
      }

      node.x = lerp(node.x, targetX, CONFIG.nodeLerp);
      node.y = lerp(node.y, targetY, CONFIG.nodeLerp);
    }
  }

  function drawBackgroundGlow() {
    noStroke();

    fill(0, 212, 255, 4);
    circle(width * 0.50, height * 0.50, max(width, height) * 0.84);

    fill(255, 78, 205, 2);
    circle(width * 0.53, height * 0.47, max(width, height) * 0.62);

    fill(0, 212, 255, 2);
    circle(width * 0.46, height * 0.55, max(width, height) * 1.02);
  }

  function drawEdges() {
    for (const edge of edges) {
      const a = nodes[edge.a];
      const b = nodes[edge.b];
      const d = Math.hypot(a.x - b.x, a.y - b.y);

      if (edge.type === "cluster") {
        const fade = constrain(1 - d / 120, 0.12, 1);
        drawSoftLine(a.x, a.y, b.x, b.y, edge.color, 26 * fade, 74 * fade, 2.2, 1);
      } else {
        drawSoftLine(a.x, a.y, b.x, b.y, edge.color, 14, 52, 1.8, 1);
      }
    }
  }

  function drawSoftLine(x1, y1, x2, y2, color, outerAlpha, innerAlpha, outerWeight, innerWeight) {
    stroke(color[0], color[1], color[2], outerAlpha);
    strokeWeight(outerWeight);
    line(x1, y1, x2, y2);

    stroke(color[0], color[1], color[2], innerAlpha);
    strokeWeight(innerWeight);
    line(x1, y1, x2, y2);
  }

  function drawPointerLines() {
    if (!pointer.active) return;

    let nearby = 0;

    for (const node of nodes) {
      const d = Math.hypot(pointer.x - node.x, pointer.y - node.y);

      if (d < CONFIG.cursorLineRadius) {
        nearby += 1;
        const fade = 1 - d / CONFIG.cursorLineRadius;
        drawSoftLine(
          pointer.x,
          pointer.y,
          node.x,
          node.y,
          node.color,
          24 * fade,
          110 * fade,
          2.4,
          1
        );
      }
    }

    if (nearby > 0) {
      noStroke();

      fill(0, 212, 255, 10);
      circle(pointer.x, pointer.y, 44);

      fill(255, 255, 255, 230);
      circle(pointer.x, pointer.y, 5.5);
    }
  }

  function drawNodes() {
    noStroke();

    for (const node of nodes) {
      fill(node.color[0], node.color[1], node.color[2], 12);
      circle(node.x, node.y, node.r * 5.2);

      fill(node.color[0], node.color[1], node.color[2], 245);
      circle(node.x, node.y, node.r * 2);
    }
  }
</script>
