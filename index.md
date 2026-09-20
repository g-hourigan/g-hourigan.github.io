---
layout: default
title: Home
permalink: /
---

<style>
  /* Hide theme elements */
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
      radial-gradient(
        circle at 18% 20%,
        rgba(0, 212, 255, 0.055),
        transparent 28%
      ),
      radial-gradient(
        circle at 82% 18%,
        rgba(255, 78, 205, 0.045),
        transparent 24%
      ),
      radial-gradient(
        circle at 50% 82%,
        rgba(0, 212, 255, 0.035),
        transparent 30%
      ),
      #050914;

    color: #dbe7ef;

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
    background: rgba(255, 78, 205, 0.22);
    color: #ffffff;
  }

  /* Animated background */

  #p5-network-bg {
    position: fixed;
    inset: 0;
    z-index: 0;
    pointer-events: none;
    opacity: 0.78;
  }

  #p5-network-bg canvas {
    display: block;
    width: 100% !important;
    height: 100% !important;
  }

  /* Main layout */

  .site-shell {
    position: relative;
    z-index: 1;

    width: min(100% - 2rem, 900px);
    min-height: 100vh;

    margin: 0 auto;
    padding: clamp(4rem, 10vw, 7rem) 0 2.5rem;

    display: flex;
    flex-direction: column;
  }

  /* Header */

  .topbar {
    padding-bottom: 1.2rem;
    border-bottom: 1px solid rgba(255, 255, 255, 0.10);
  }

  .name {
    margin: 0;

    color: #f4f7fa;

    font-size: clamp(2.25rem, 5vw, 3.45rem);
    font-weight: 700;
    line-height: 1;
    letter-spacing: -0.045em;
  }

  /* Intro */

  .intro {
    max-width: 720px;
    padding: clamp(2.6rem, 7vw, 5rem) 0;
  }

  .intro p {
    margin: 0;

    color: #aebdca;

    font-size: clamp(1.15rem, 2.4vw, 1.45rem);
    line-height: 1.65;
    letter-spacing: -0.015em;
  }

  .intro strong {
    color: #edf3f7;
    font-weight: 600;
  }

  /* Optional work section */

  .work {
    max-width: 760px;

    padding-top: 1.2rem;

    border-top: 1px solid rgba(255, 255, 255, 0.10);
  }

  .section-heading {
    margin: 0 0 0.7rem;

    color: #738196;

    font-size: 0.78rem;
    font-weight: 700;

    letter-spacing: 0.13em;
    text-transform: uppercase;
  }

  .work-list {
    margin: 0;
    padding: 0;

    list-style: none;
  }

  .work-item {
    display: grid;
    grid-template-columns: 6rem 1fr;
    gap: 1.5rem;

    padding: 1.25rem 0;

    border-bottom: 1px solid rgba(255, 255, 255, 0.075);
  }

  .work-date {
    color: #738196;
    font-size: 0.9rem;
  }

  .work-title {
    margin: 0;

    color: #e6edf2;

    font-size: 1rem;
    font-weight: 600;
  }

  .work-title a {
    color: inherit !important;
    text-decoration: none !important;

    transition: color 0.18s ease;
  }

  .work-title a:hover {
    color: #ffffff !important;
  }

  .work-text {
    margin: 0.3rem 0 0;

    color: #91a0b1;

    line-height: 1.6;
  }

  /* Footer */

  .footer {
    margin-top: auto;
    padding-top: 1.15rem;

    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 1rem;

    border-top: 1px solid rgba(255, 255, 255, 0.08);

    color: #647286;

    font-size: 0.86rem;
  }

  .footer-links {
    display: flex;
    align-items: center;
    gap: 0.55rem;
  }

  .footer a {
    color: #8998aa !important;
    text-decoration: none !important;

    transition: color 0.18s ease;
  }

  .footer a:hover {
    color: #ffffff !important;
  }

  /* Mobile */

  @media (max-width: 620px) {
    .site-shell {
      width: min(100% - 1.5rem, 900px);
      padding-top: 3rem;
      padding-bottom: 2rem;
    }

    .intro {
      padding: 2.75rem 0 4rem;
    }

    .work-item {
      grid-template-columns: 1fr;
      gap: 0.35rem;
    }

    .footer {
      align-items: flex-start;
      flex-direction: column;
      gap: 0.55rem;
    }
  }

  @media (prefers-reduced-motion: reduce) {
    #p5-network-bg {
      opacity: 0.55;
    }
  }
</style>

<div id="p5-network-bg" aria-hidden="true"></div>

<main class="site-shell">

  <header class="topbar">
    <h1 class="name">Gerrit Hourigan</h1>
  </header>

  <section class="intro" aria-label="About">
    <p>
      I am a psychology student interested in
      <strong>statistical and computational approaches to studying human behavior.</strong>
    </p>
  </section>

  <!--
  Add papers or projects here when you have something you want to feature.

  Example:

  <section class="work" aria-labelledby="work-heading">

    <h2 class="section-heading" id="work-heading">
      Selected work
    </h2>

    <ol class="work-list">

      <li class="work-item">

        <time class="work-date" datetime="2026">
          2026
        </time>

        <div>
          <h3 class="work-title">
            <a href="YOUR-LINK-HERE">
              Project or paper title
            </a>
          </h3>

          <p class="work-text">
            A short description of the project or paper.
          </p>
        </div>

      </li>

    </ol>

  </section>
  -->

  <footer class="footer">

    <div class="footer-links">
      <a href="mailto:gerrithourigan@gmail.com">
        Email
      </a>

      <span aria-hidden="true">·</span>

      <a
        href="https://github.com/g-hourigan"
        target="_blank"
        rel="noopener noreferrer"
      >
        GitHub
      </a>
    </div>

    <div>© 2026 Gerrit Hourigan</div>

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

    pixelDensity(
      Math.min(window.devicePixelRatio || 1, 2)
    );

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
          distance: dist(
            particle.x,
            particle.y,
            other.x,
            other.y
          )
        });
      }

      distances.sort(
        (a, b) => a.distance - b.distance
      );

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
            100,
            0
          );

          const weight = map(
            entry.distance,
            0,
            SETTINGS.maxDistance,
            1.2,
            0.2
          );

          stroke(0, 240, 255, alpha);
          strokeWeight(weight);

          line(
            particle.x,
            particle.y,
            other.x,
            other.y
          );
        }
      }
    }
  }

  function drawParticles() {
    noStroke();

    for (const particle of particles) {
      fill(255, 61, 171, 22);

      circle(
        particle.x,
        particle.y,
        particle.size * 3
      );

      fill(255, 61, 171, 175);

      circle(
        particle.x,
        particle.y,
        particle.size * 1.45
      );
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
      const time =
        (frameCount + this.seed) *
        SETTINGS.flowSpeed;

      const angle =
        noise(
          this.x * SETTINGS.flowScale,
          this.y * SETTINGS.flowScale,
          time
        ) *
        TWO_PI *
        SETTINGS.flowTurns;

      this.vx =
        (this.vx + cos(angle) * 0.06) *
        0.92;

      this.vy =
        (this.vy + sin(angle) * 0.06) *
        0.92;

      this.x += this.vx;
      this.y += this.vy;

      if (pointer.active) {
        const distanceToPointer = dist(
          this.x,
          this.y,
          pointer.x,
          pointer.y
        );

        if (
          distanceToPointer <
          SETTINGS.mouseRadius
        ) {
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

      if (this.x < -margin) {
        this.x = width + margin;
      }

      if (this.x > width + margin) {
        this.x = -margin;
      }

      if (this.y < -margin) {
        this.y = height + margin;
      }

      if (this.y > height + margin) {
        this.y = -margin;
      }
    }
  }
</script>
