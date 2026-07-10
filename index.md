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

  * {
    box-sizing: border-box;
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
    background: rgba(255, 78, 205, 0.22);
    color: #ffffff;
  }

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

  .site-shell {
    position: relative;
    z-index: 1;
    width: min(100% - 2rem, 900px);
    margin: 0 auto;
    padding: clamp(4rem, 10vw, 7rem) 0 3rem;
  }

  .topbar {
    display: flex;
    align-items: baseline;
    justify-content: space-between;
    gap: 2rem;
    padding-bottom: 1.15rem;
    border-bottom: 1px solid rgba(255, 255, 255, 0.10);
  }

  .name {
    margin: 0;
    font-size: clamp(2.15rem, 5vw, 3.4rem);
    line-height: 1;
    letter-spacing: -0.045em;
    font-weight: 720;
    color: #f4f7fa;
  }

  .nav {
    display: flex;
    flex-wrap: wrap;
    gap: 1.1rem;
    font-size: 0.93rem;
  }

  .nav a,
  .update-title a {
    color: #aebdca !important;
    text-decoration: none !important;
    transition: color 0.18s ease;
  }

  .nav a:hover,
  .update-title a:hover {
    color: #ffffff !important;
  }

  .intro {
    max-width: 660px;
    padding: clamp(2.3rem, 6vw, 4.5rem) 0;
  }

  .intro p {
    margin: 0;
    font-size: clamp(1.15rem, 2.4vw, 1.45rem);
    line-height: 1.65;
    letter-spacing: -0.015em;
    color: #aebdca;
  }

  .intro strong {
    color: #edf3f7;
    font-weight: 600;
  }

  .updates {
    max-width: 760px;
    padding-top: 1.15rem;
    border-top: 1px solid rgba(255, 255, 255, 0.10);
  }

  .section-heading {
    margin: 0 0 0.65rem;
    font-size: 0.8rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: #738196;
  }

  .empty-state {
    margin: 0;
    padding: 1rem 0 1.5rem;
    color: #8998aa;
    line-height: 1.65;
  }

  .update-list {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .update-item {
    display: grid;
    grid-template-columns: 7rem 1fr;
    gap: 1.5rem;
    padding: 1.2rem 0;
    border-bottom: 1px solid rgba(255, 255, 255, 0.08);
  }

  .update-date {
    color: #738196;
    font-size: 0.9rem;
  }

  .update-title {
    margin: 0;
    font-size: 1rem;
    font-weight: 600;
    color: #e6edf2;
  }

  .update-text {
    margin: 0.3rem 0 0;
    color: #91a0b1;
    line-height: 1.6;
  }

  .footer {
    margin-top: 5rem;
    padding-top: 1.1rem;
    border-top: 1px solid rgba(255, 255, 255, 0.08);
    color: #647286;
    font-size: 0.88rem;
  }

  @media (max-width: 620px) {
    .site-shell {
      width: min(100% - 1.4rem, 900px);
      padding-top: 2.8rem;
    }

    .topbar {
      align-items: flex-start;
      flex-direction: column;
      gap: 1.1rem;
    }

    .intro {
      padding: 2.6rem 0 3.5rem;
    }

    .update-item {
      grid-template-columns: 1fr;
      gap: 0.35rem;
    }
  }
</style>

<div id="p5-network-bg" aria-hidden="true"></div>

<main class="site-shell">
  <header class="topbar">
    <h1 class="name">Gerrit Hourigan</h1>

    <nav class="nav" aria-label="Primary navigation">
      <a href="/cv/">CV</a>
      <a href="mailto:gerrithourigan@gmail.com">Email</a>
      <a href="https://github.com/g-hourigan" target="_blank" rel="noopener noreferrer">GitHub</a>
    </nav>
  </header>

  <section class="intro" aria-label="About">
    <p>
      I am a psychology researcher interested in <strong>cognition, individual differences,
      and quantitative methods</strong>. I use this site to share papers and occasional updates.
    </p>
  </section>

  <!-- Add this section when you have something to post.
  <section class="updates" aria-labelledby="updates-heading">
    <h2 class="section-heading" id="updates-heading">Recent</h2>

    <ol class="update-list">
      <li class="update-item">
        <time class="update-date" datetime="2026-08">August 2026</time>
        <div>
          <h3 class="update-title">
            <a href="YOUR-LINK-HERE">Title of paper or update</a>
          </h3>
          <p class="update-text">One brief sentence about it.</p>
        </div>
      </li>
    </ol>
  </section>
  -->

  <footer class="footer">© 2026 Gerrit Hourigan</footer>
</main>

<script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.9.4/p5.min.js"></script>
<script>
  let particles = [];
  let pointer = { x: 0, y: 0, active: false };

  const SETTINGS = {
    particleCountDesktop: 52,
    particleCountMobile: 32,
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
    const count = windowWidth < 760
      ? SETTINGS.particleCountMobile
      : SETTINGS.particleCountDesktop;

    for (let index = 0; index < count; index++) {
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

      for (let k = 0; k < Math.min(SETTINGS.maxNeighbors, distances.length); k++) {
        const entry = distances[k];

        if (entry.distance < SETTINGS.maxDistance) {
          const other = particles[entry.index];
          const alpha = map(entry.distance, 0, SETTINGS.maxDistance, 100, 0);
          const weight = map(entry.distance, 0, SETTINGS.maxDistance, 1.2, 0.2);

          stroke(0, 240, 255, alpha);
          strokeWeight(weight);
          line(particle.x, particle.y, other.x, other.y);
        }
      }
    }
  }

  function drawParticles() {
    noStroke();

    for (const particle of particles) {
      fill(255, 61, 171, 22);
      circle(particle.x, particle.y, particle.size * 3);

      fill(255, 61, 171, 175);
      circle(particle.x, particle.y, particle.size * 1.45);
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
      const angle = noise(
        this.x * SETTINGS.flowScale,
        this.y * SETTINGS.flowScale,
        time
      ) * TWO_PI * SETTINGS.flowTurns;

      this.vx = (this.vx + cos(angle) * 0.06) * 0.92;
      this.vy = (this.vy + sin(angle) * 0.06) * 0.92;
      this.x += this.vx;
      this.y += this.vy;

      if (pointer.active) {
        const distanceToPointer = dist(this.x, this.y, pointer.x, pointer.y);

        if (distanceToPointer < SETTINGS.mouseRadius) {
          const force = map(
            distanceToPointer,
            0,
            SETTINGS.mouseRadius,
            SETTINGS.mousePull,
            0
          );

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
