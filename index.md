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
    max-width: 1080px;
    margin: 0 auto;
    padding: 3rem 1.25rem;
  }

  .site-panel {
    position: relative;
    overflow: hidden;
    min-height: calc(100vh - 6rem);
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
    padding: clamp(2rem, 5vw, 4.5rem);
  }

  .site-panel::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
      linear-gradient(90deg, rgba(0, 212, 255, 0.04), transparent 20%, transparent 80%, rgba(255, 78, 205, 0.035)),
      linear-gradient(180deg, rgba(255, 255, 255, 0.02), transparent 25%);
    pointer-events: none;
  }

  .content {
    position: relative;
    z-index: 1;
    max-width: 820px;
  }

  .hero-title {
    margin: 0;
    font-size: clamp(3rem, 8vw, 6rem);
    line-height: 0.95;
    letter-spacing: -0.065em;
    font-weight: 800;
    color: #f4f8fb;
  }

  .hero-subtitle {
    max-width: 760px;
    margin: 1.35rem 0 0;
    font-size: clamp(1.05rem, 2vw, 1.3rem);
    line-height: 1.65;
    color: #9fb0c2;
  }

  .intro {
    max-width: 760px;
    margin-top: 4.5rem;
  }

  .intro p {
    margin: 0;
    font-size: 1.08rem;
    line-height: 1.9;
    color: #b5c2cf;
  }

  .section {
    max-width: 760px;
    margin-top: 4.5rem;
  }

  .section-title {
    margin: 0 0 1.35rem;
    font-size: 0.82rem;
    font-weight: 800;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: #7f8da1;
  }

  .update-list {
    border-top: 1px solid rgba(255, 255, 255, 0.08);
  }

  .update-item {
    display: grid;
    grid-template-columns: 8rem 1fr;
    gap: 1.5rem;
    padding: 1.35rem 0;
    border-bottom: 1px solid rgba(255, 255, 255, 0.08);
  }

  .update-date {
    color: #7f8da1;
    font-size: 0.95rem;
  }

  .update-title {
    margin: 0;
    font-size: 1.05rem;
    font-weight: 700;
    color: #edf4f8;
  }

  .update-text {
    margin: 0.35rem 0 0;
    line-height: 1.65;
    color: #9fb0c2;
  }

  .footer {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    gap: 1.25rem;
    max-width: 760px;
    margin-top: 4.5rem;
    padding-top: 1.4rem;
    border-top: 1px solid rgba(255, 255, 255, 0.08);
    color: #718096;
    font-size: 0.95rem;
  }

  .footer-links {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
  }

  .footer a {
    color: #aebdca !important;
    text-decoration: none !important;
    transition: color 0.2s ease;
  }

  .footer a:hover {
    color: #f4f8fb !important;
  }

  @media (max-width: 720px) {
    .site-shell {
      padding: 1rem 0.7rem;
    }

    .site-panel {
      min-height: calc(100vh - 2rem);
      border-radius: 22px;
      padding: 2rem 1.25rem;
    }

    .intro,
    .section,
    .footer {
      margin-top: 3.5rem;
    }

    .update-item {
      grid-template-columns: 1fr;
      gap: 0.45rem;
    }
  }
</style>

<div id="p5-network-bg" aria-hidden="true"></div>

<section class="site-shell">
  <main class="site-panel">
    <div class="content">
      <header>
        <h1 class="hero-title">Gerrit Hourigan</h1>
        <p class="hero-subtitle">
          Psychology, cognition, behavioral data, and quantitative research.
        </p>
      </header>

      <section class="intro" aria-label="About">
        <p>
          I study how people think, learn, and differ—and how these questions can be
          addressed through careful measurement and statistical modeling. This site is
          a small home for papers, research notes, and other work I find worth sharing.
        </p>
      </section>

      <section class="section" aria-labelledby="updates-title">
        <h2 class="section-title" id="updates-title">Updates</h2>

        <div class="update-list">
          <article class="update-item">
            <time class="update-date" datetime="2026-07">July 2026</time>
            <div>
              <h3 class="update-title">Website online</h3>
              <p class="update-text">
                A simple space for publications, research notes, and occasional updates.
              </p>
            </div>
          </article>

          <!-- Duplicate the block below whenever you want to add a new update.
          <article class="update-item">
            <time class="update-date" datetime="2026-08">August 2026</time>
            <div>
              <h3 class="update-title">
                <a href="YOUR-LINK-HERE">Title of paper or update</a>
              </h3>
              <p class="update-text">One brief sentence about it.</p>
            </div>
          </article>
          -->
        </div>
      </section>

      <footer class="footer">
        <span>© 2026 Gerrit Hourigan</span>

        <nav class="footer-links" aria-label="Contact links">
          <a href="/cv/">CV</a>
          <a href="mailto:gerrithourigan@gmail.com">Email</a>
          <a href="https://github.com/g-hourigan" target="_blank" rel="noopener noreferrer">GitHub</a>
        </nav>
      </footer>
    </div>
  </main>
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
