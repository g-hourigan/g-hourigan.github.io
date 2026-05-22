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
    filter: saturate(1.08) brightness(1.02);
  }

  #p5-network-bg canvas {
    display: block;
    width: 100% !important;
    height: 100% !important;
  }

  #p5-network-bg::after {
    content: "";
    position: fixed;
    inset: 0;
    pointer-events: none;
    background-image: linear-gradient(rgba(255, 255, 255, 0.01) 1px, transparent 1px);
    background-size: 100% 3px;
    mix-blend-mode: overlay;
    opacity: 0.10;
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

  .project-card-compact {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 1.2rem;
    padding: 1rem 1.1rem;
    text-decoration: none !important;
    transition: transform 0.2s ease, border-color 0.2s ease, background 0.2s ease;
  }

  .project-card-compact:hover {
    transform: translateY(-2px);
    border-color: rgba(0, 212, 255, 0.28);
    background: linear-gradient(
      180deg,
      rgba(16, 25, 42, 0.94),
      rgba(9, 15, 26, 0.94)
    );
  }

  .project-card-compact h3 {
    margin: 0 0 0.25rem;
    font-size: 1.05rem;
    color: #f7fbff;
  }

  .project-card-compact p {
    margin: 0;
    font-size: 0.9rem;
    line-height: 1.45;
    color: #9fb0c2;
  }

  .project-arrow {
    flex-shrink: 0;
    color: #00d4ff;
    font-size: 0.9rem;
    font-weight: 700;
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

    .project-card-compact {
      flex-direction: column;
      align-items: flex-start;
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

    <a class="project-card project-card-compact" href="/projects/life-events-rca/">
      <div>
        <h3>Life Events and Climate Action Readiness</h3>
        <p>
          A longitudinal SEM case study testing whether life events predict change in
          climate-action readiness.
        </p>
      </div>
      <span class="project-arrow">Read project →</span>
    </a>

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
      Interface: GitHub Pages / Jekyll / p5.js particle background.
    </p>
  </div>
</section>

<script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.9.4/p5.min.js"></script>
<script>
  let particles = [];
  let pointer = {
    x: 0,
    y: 0,
    active: false
  };

  const SETTINGS = {
    particleCountDesktop: 64,
    particleCountMobile: 42,
    maxNeighbors: 4,
    maxDistance: 155,
    mouseRadius: 220,
    mousePull: 0.06,
    flowScale: 0.002,
    flowSpeed: 0.002,
    flowTurns: 2.0
  };

  function setup() {
    const parent = document.getElementById("p5-network-bg");
    const canvas = createCanvas(windowWidth, windowHeight);
    canvas.parent(parent);
    pixelDensity(Math.min(window.devicePixelRatio || 1, 2));
    buildParticles();
    bindPointerEvents();
  }

  function draw() {
    clear();
    background(7, 16, 36, 0);

    for (let i = 0; i < particles.length; i++) {
      particles[i].update();
    }

    blendMode(ADD);
    drawConnections();
    drawParticles();
    drawPointerGlow();
    blendMode(BLEND);
  }

  function windowResized() {
    resizeCanvas(windowWidth, windowHeight);
    buildParticles();
  }

  function bindPointerEvents() {
    window.addEventListener("pointermove", (e) => {
      pointer.x = e.clientX;
      pointer.y = e.clientY;
      pointer.active = true;
    });

    window.addEventListener("pointerdown", (e) => {
      pointer.x = e.clientX;
      pointer.y = e.clientY;
      pointer.active = true;
    });

    window.addEventListener("pointerleave", () => {
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

  function buildParticles() {
    particles = [];
    const isMobile = windowWidth < 760;
    const count = isMobile ? SETTINGS.particleCountMobile : SETTINGS.particleCountDesktop;

    for (let i = 0; i < count; i++) {
      particles.push(new Particle());
    }
  }

  function drawConnections() {
    for (let i = 0; i < particles.length; i++) {
      const p = particles[i];
      const distances = [];

      for (let j = i + 1; j < particles.length; j++) {
        const q = particles[j];
        const d = dist(p.x, p.y, q.x, q.y);
        distances.push({ index: j, distance: d });
      }

      distances.sort((a, b) => a.distance - b.distance);

      for (let k = 0; k < Math.min(SETTINGS.maxNeighbors, distances.length); k++) {
        const entry = distances[k];

        if (entry.distance < SETTINGS.maxDistance) {
          const q = particles[entry.index];
          const alpha = map(entry.distance, 0, SETTINGS.maxDistance, 150, 0);
          const weight = map(entry.distance, 0, SETTINGS.maxDistance, 1.55, 0.2);

          stroke(0, 240, 255, alpha * 0.9);
          strokeWeight(weight);
          line(p.x, p.y, q.x, q.y);
        }
      }
    }
  }

  function drawParticles() {
    noStroke();

    for (let i = 0; i < particles.length; i++) {
      const p = particles[i];

      fill(255, 61, 171, 28);
      circle(p.x, p.y, p.size * 3.2);

      fill(255, 61, 171, 205);
      circle(p.x, p.y, p.size * 1.55);
    }
  }

  function drawPointerGlow() {
    if (!pointer.active) return;

    noStroke();
    fill(0, 240, 255, 10);
    circle(pointer.x, pointer.y, 42);
    fill(255, 255, 255, 190);
    circle(pointer.x, pointer.y, 4.5);
  }

  class Particle {
    constructor() {
      this.reset();
    }

    reset() {
      this.x = random(width);
      this.y = random(height);
      this.vx = random(-0.4, 0.4);
      this.vy = random(-0.4, 0.4);
      this.seed = random(10000);
      this.size = random(1.6, 3.4);
    }

    update() {
      const t = (frameCount + this.seed) * SETTINGS.flowSpeed;
      const angle = noise(
        this.x * SETTINGS.flowScale,
        this.y * SETTINGS.flowScale,
        t
      ) * TWO_PI * SETTINGS.flowTurns;

      this.vx += cos(angle) * 0.06;
      this.vy += sin(angle) * 0.06;

      this.vx *= 0.92;
      this.vy *= 0.92;

      this.x += this.vx;
      this.y += this.vy;

      if (pointer.active) {
        const dMouse = dist(this.x, this.y, pointer.x, pointer.y);

        if (dMouse < SETTINGS.mouseRadius) {
          const force = map(dMouse, 0, SETTINGS.mouseRadius, SETTINGS.mousePull, 0);
          this.x = lerp(this.x, pointer.x + cos(this.seed) * 8, force);
          this.y = lerp(this.y, pointer.y + sin(this.seed) * 8, force);
        }
      }

      const margin = 8;

      if (this.x < -margin) this.x = width + margin;
      if (this.x > width + margin) this.x = -margin;
      if (this.y < -margin) this.y = height + margin;
      if (this.y > height + margin) this.y = -margin;
    }
  }
</script>
