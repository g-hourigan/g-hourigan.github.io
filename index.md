---
layout: default
title: Home
permalink: /
---

<style>
  /* Hide theme chrome */
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
    width: 100% !important;
    max-width: none !important;
    margin: 0 !important;
    padding: 0 !important;
  }

  * {
    box-sizing: border-box;
  }

  html,
  body {
    min-height: 100%;
  }

  body {
    margin: 0;
    overflow-x: hidden;
    background:
      radial-gradient(circle at 16% 18%, rgba(0, 220, 255, 0.045), transparent 28%),
      radial-gradient(circle at 84% 16%, rgba(255, 65, 170, 0.04), transparent 24%),
      #030711;
    color: #dbe4ec;
    font-family:
      Inter,
      ui-sans-serif,
      system-ui,
      -apple-system,
      BlinkMacSystemFont,
      "Segoe UI",
      sans-serif;
    -webkit-font-smoothing: antialiased;
    text-rendering: optimizeLegibility;
  }

  ::selection {
    background: rgba(255, 65, 170, 0.22);
    color: #ffffff;
  }

  /* Animated background */
  #p5-network-bg {
    position: fixed;
    inset: 0;
    z-index: 0;
    pointer-events: none;
    opacity: 0.8;
  }

  #p5-network-bg canvas {
    display: block;
    width: 100% !important;
    height: 100% !important;
  }

  /* Main panel */
  .site-panel {
    position: relative;
    z-index: 1;
    width: min(100% - 2rem, 820px);
    min-height: 100vh;
    margin: 0 auto;
    padding: clamp(3.2rem, 7vw, 5rem) clamp(1.8rem, 4vw, 3.2rem) 2.4rem;
    display: flex;
    flex-direction: column;
    background: rgba(3, 7, 17, 0.86);
    border-left: 1px solid rgba(255, 255, 255, 0.03);
    border-right: 1px solid rgba(255, 255, 255, 0.03);
    box-shadow: 0 0 50px rgba(0, 0, 0, 0.2);
    backdrop-filter: blur(2px);
    -webkit-backdrop-filter: blur(2px);
  }

  /* Hero */
  .hero {
    display: grid;
    grid-template-columns: 4px 1fr;
    gap: 1.6rem;
    align-items: start;
    margin-bottom: 4rem;
  }

  .hero-accent {
    width: 4px;
    min-height: 15rem;
    border-radius: 999px;
    background: #ff3da9;
    box-shadow: 0 0 14px rgba(255, 61, 169, 0.16);
  }

  .name {
    margin: 0;
    color: #f3f7fa;
    font-size: clamp(2.5rem, 5.8vw, 4.3rem);
    font-weight: 700;
    line-height: 0.98;
    letter-spacing: -0.05em;
  }

  .role {
    margin: 0.95rem 0 0;
    color: #8e9daf;
    font-size: clamp(1rem, 2vw, 1.15rem);
    font-weight: 450;
    line-height: 1.5;
  }

  .interest {
    margin: 2rem 0 0;
    max-width: 640px;
    color: #c0ccd7;
    font-size: clamp(1.15rem, 2.4vw, 1.55rem);
    line-height: 1.65;
    letter-spacing: -0.02em;
  }

  .interest strong {
    color: #eef3f7;
    font-weight: 600;
  }

  /* Sections */
  .section {
    margin-top: 3rem;
  }

  .section-heading {
    display: flex;
    align-items: center;
    gap: 0.8rem;
    margin: 0 0 1.15rem;
    color: #7f8ea1;
    font-size: 0.76rem;
    font-weight: 700;
    letter-spacing: 0.16em;
    text-transform: uppercase;
  }

  .section-heading::after {
    content: "";
    flex: 1;
    height: 1px;
    background: rgba(255, 255, 255, 0.06);
  }

  .slashes {
    color: #00e2f4;
  }

  .about-text {
    max-width: 660px;
    margin: 0;
    color: #9eacbb;
    font-size: 1rem;
    line-height: 1.75;
  }

  /* Contact */
  .contact-links {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    align-items: center;
  }

  .contact-links a {
    color: #a7b5c3 !important;
    text-decoration: none !important;
    transition: color 0.18s ease;
  }

  .contact-links a:hover {
    color: #00e2f4 !important;
  }

  .contact-separator {
    color: #4a5868;
  }

  /* Optional work section */
  .work-list {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .work-item {
    display: grid;
    grid-template-columns: 5rem 1fr;
    gap: 1.3rem;
    padding: 1rem 0;
    border-bottom: 1px solid rgba(255, 255, 255, 0.06);
  }

  .work-item:first-child {
    border-top: 1px solid rgba(255, 255, 255, 0.06);
  }

  .work-date {
    color: #647286;
    font-size: 0.86rem;
    line-height: 1.5;
  }

  .work-title {
    margin: 0;
    color: #e5edf3;
    font-size: 1rem;
    font-weight: 600;
  }

  .work-title a {
    color: inherit !important;
    text-decoration: none !important;
    transition: color 0.18s ease;
  }

  .work-title a:hover {
    color: #00e2f4 !important;
  }

  .work-text {
    margin: 0.25rem 0 0;
    color: #8e9dad;
    line-height: 1.65;
  }

  /* Footer */
  .footer {
    margin-top: auto;
    padding-top: 3.8rem;
    color: #526172;
    font-size: 0.8rem;
  }

  /* Responsive */
  @media (max-width: 620px) {
    .site-panel {
      width: 100%;
      padding: 2.8rem 1.3rem 2rem;
      border-left: none;
      border-right: none;
      background: rgba(3, 7, 17, 0.84);
    }

    .hero {
      grid-template-columns: 3px 1fr;
      gap: 1rem;
      margin-bottom: 3.2rem;
    }

    .hero-accent {
      min-height: 12.5rem;
      width: 3px;
    }

    .interest {
      margin-top: 1.6rem;
    }

    .work-item {
      grid-template-columns: 1fr;
      gap: 0.25rem;
    }

    .contact-links {
      gap: 0.7rem;
    }
  }

  @media (prefers-reduced-motion: reduce) {
    #p5-network-bg {
      opacity: 0.58;
    }
  }
</style>

<div id="p5-network-bg" aria-hidden="true"></div>

<main class="site-panel">
  <header class="hero">
    <div class="hero-accent" aria-hidden="true"></div>

    <div class="hero-copy">
      <h1 class="name">Gerrit Hourigan</h1>

      <p class="role">Psychology student</p>

      <p class="interest">
        Interested in
        <strong>statistical and computational approaches to studying human behavior.</strong>
      </p>
    </div>
  </header>

  <section class="section" aria-labelledby="about-heading">
    <h2 class="section-heading" id="about-heading">
      <span class="slashes">//</span>
      About
    </h2>

    <p class="about-text">
      I am a psychology student with a particular interest in statistics,
      data science, and computational methods.
    </p>
  </section>

  <!--
  Uncomment this section once you have a paper or project you want to feature.

  <section class="section" aria-labelledby="work-heading">
    <h2 class="section-heading" id="work-heading">
      <span class="slashes">//</span>
      Selected work
    </h2>

    <ol class="work-list">
      <li class="work-item">
        <time class="work-date" datetime="2026">2026</time>

        <div>
          <h3 class="work-title">
            <a href="YOUR-LINK-HERE">Project or paper title</a>
          </h3>

          <p class="work-text">
            A short description of the project or paper.
          </p>
        </div>
      </li>
    </ol>
  </section>
  -->

  <section class="section" aria-labelledby="contact-heading">
    <h2 class="section-heading" id="contact-heading">
      <span class="slashes">//</span>
      Contact
    </h2>

    <div class="contact-links">
      <a href="mailto:gerrithourigan@gmail.com">Email</a>
      <span class="contact-separator">·</span>
      <a
        href="https://github.com/g-hourigan"
        target="_blank"
        rel="noopener noreferrer"
      >
        GitHub
      </a>
    </div>
  </section>

  <footer class="footer">
    © 2026 Gerrit Hourigan
  </footer>
</main>

<script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.9.4/p5.min.js"></script>

<script>
  let particles = [];

  let pointer = {
    x: 0,
    y: 0,
    active: false
  };

  const SETTINGS = {
    particleCountDesktop: 52,
    particleCountMobile: 30,
    maxNeighbors: 3,
    maxDistance: 150,
    mouseRadius: 210,
    mousePull: 0.05,
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

    if (
      window.matchMedia &&
      window.matchMedia("(prefers-reduced-motion: reduce)").matches
    ) {
      frameRate(20);
    }
  }

  function draw() {
    clear();

    for (const particle of particles) {
      particle.update();
    }

    blendMode(ADD);
    drawConnections();
    drawParticles();
    blendMode(BLEND);
  }

  function windowResized() {
    resizeCanvas(windowWidth, windowHeight);
    buildParticles();
  }

  function bindPointerEvents() {
    window.addEventListener("pointermove", (event) => {
      pointer.x = event.clientX;
      pointer.y = event.clientY;
      pointer.active = true;
    });

    window.addEventListener("pointerleave", () => {
      pointer.active = false;
    });
  }

  function buildParticles() {
    particles = [];

    const count =
      windowWidth < 760
        ? SETTINGS.particleCountMobile
        : SETTINGS.particleCountDesktop;

    for (let i = 0; i < count; i++) {
      particles.push(new Particle());
    }
  }

  function drawConnections() {
    for (let i = 0; i < particles.length; i++) {
      const particle = particles[i];
      const distances = [];

      for (let j = i + 1; j < particles.length; j++) {
        const other = particles[j];

        distances.push({
          index: j,
          distance: dist(particle.x, particle.y, other.x, other.y)
        });
      }

      distances.sort((a, b) => a.distance - b.distance);

      const neighborCount = Math.min(
        SETTINGS.maxNeighbors,
        distances.length
      );

      for (let k = 0; k < neighborCount; k++) {
        const entry = distances[k];

        if (entry.distance < SETTINGS.maxDistance) {
          const other = particles[entry.index];

          const alpha = map(
            entry.distance,
            0,
            SETTINGS.maxDistance,
            90,
            0
          );

          const weight = map(
            entry.distance,
            0,
            SETTINGS.maxDistance,
            1.05,
            0.18
          );

          stroke(0, 228, 244, alpha);
          strokeWeight(weight);
          line(particle.x, particle.y, other.x, other.y);
        }
      }
    }
  }

  function drawParticles() {
    noStroke();

    for (const particle of particles) {
      fill(255, 61, 169, 18);
      circle(particle.x, particle.y, particle.size * 3);

      fill(255, 61, 169, 165);
      circle(particle.x, particle.y, particle.size * 1.4);
    }
  }

  class Particle {
    constructor() {
      this.x = random(width);
      this.y = random(height);
      this.vx = random(-0.4, 0.4);
      this.vy = random(-0.4, 0.4);
      this.seed = random(10000);
      this.size = random(1.5, 3.1);
    }

    update() {
      const time = (frameCount + this.seed) * SETTINGS.flowSpeed;

      const angle =
        noise(
          this.x * SETTINGS.flowScale,
          this.y * SETTINGS.flowScale,
          time
        ) *
        TWO_PI *
        SETTINGS.flowTurns;

      this.vx = (this.vx + cos(angle) * 0.06) * 0.92;
      this.vy = (this.vy + sin(angle) * 0.06) * 0.92;

      this.x += this.vx;
      this.y += this.vy;

      if (pointer.active) {
        const distanceToPointer = dist(
          this.x,
          this.y,
          pointer.x,
          pointer.y
        );

        if (distanceToPointer < SETTINGS.mouseRadius) {
          const force = map(
            distanceToPointer,
            0,
            SETTINGS.mouseRadius,
            SETTINGS.mousePull,
            0
          );

          this.x = lerp(
            this.x,
            pointer.x + cos(this.seed) * 8,
            force
          );

          this.y = lerp(
            this.y,
            pointer.y + sin(this.seed) * 8,
            force
          );
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
