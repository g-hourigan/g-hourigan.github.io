---
layout: default
title: Home
permalink: /
---

<style>
  /* --------------------------------------------------
     Remove theme elements
  -------------------------------------------------- */

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

  html {
    background: #030711;
  }

  body {
    margin: 0;
    overflow-x: hidden;
    background:
      radial-gradient(circle at 15% 18%, rgba(0, 220, 255, 0.045), transparent 28%),
      radial-gradient(circle at 85% 14%, rgba(255, 61, 169, 0.04), transparent 25%),
      radial-gradient(circle at 70% 82%, rgba(0, 220, 255, 0.025), transparent 28%),
      #030711;
    color: #dce5ec;
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
    background: rgba(255, 61, 169, 0.22);
    color: #ffffff;
  }

  a {
    -webkit-tap-highlight-color: transparent;
  }

  /* --------------------------------------------------
     Network background
  -------------------------------------------------- */

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

  /* --------------------------------------------------
     Main panel
  -------------------------------------------------- */

  .site-panel {
    position: relative;
    z-index: 1;
    width: min(100% - 2rem, 760px);
    min-height: 100vh;
    margin: 0 auto;
    padding:
      clamp(3.6rem, 8vw, 5.8rem)
      clamp(1.5rem, 4.8vw, 3.2rem)
      2.2rem;
    display: flex;
    flex-direction: column;
    background: rgba(3, 7, 17, 0.78);
    border-left: 1px solid rgba(255, 255, 255, 0.025);
    border-right: 1px solid rgba(255, 255, 255, 0.025);
    box-shadow: 0 0 52px rgba(0, 0, 0, 0.18);
    backdrop-filter: blur(2px);
    -webkit-backdrop-filter: blur(2px);
  }

  /* --------------------------------------------------
     Hero
  -------------------------------------------------- */

  .hero {
    display: grid;
    grid-template-columns: 2px 1fr;
    gap: 1.25rem;
    align-items: start;
    margin-bottom: clamp(3.6rem, 8vw, 5.2rem);
  }

  .hero-accent {
    width: 2px;
    min-height: 8.5rem;
    border-radius: 999px;
    background: #ff3da9;
    box-shadow: 0 0 12px rgba(255, 61, 169, 0.15);
  }

  .hero-copy {
    max-width: 560px;
  }

  .name {
    margin: 0;
    color: #f3f7fa;
    font-size: clamp(2.2rem, 5vw, 3.45rem);
    font-weight: 700;
    line-height: 0.98;
    letter-spacing: -0.05em;
  }

  .meta {
    margin-top: 1rem;
    color: #8b99ab;
    font-size: clamp(0.98rem, 1.9vw, 1.08rem);
    line-height: 1.7;
  }

  .meta strong {
    color: #aab7c5;
    font-weight: 500;
  }

  /* --------------------------------------------------
     Sections
  -------------------------------------------------- */

  .section {
    margin-top: 2.8rem;
  }

  .section:first-of-type {
    margin-top: 0;
  }

  .section-heading {
    display: flex;
    align-items: center;
    gap: 0.8rem;
    margin: 0 0 1.15rem;
    color: #768598;
    font-size: 0.74rem;
    font-weight: 700;
    letter-spacing: 0.16em;
    text-transform: uppercase;
  }

  .section-heading::after {
    content: "";
    flex: 1;
    height: 1px;
    background: rgba(255, 255, 255, 0.055);
  }

  .slashes {
    color: #00ddec;
    letter-spacing: 0;
  }

  /* --------------------------------------------------
     Code-like profile block
  -------------------------------------------------- */

  .code-block {
    margin: 0;
    padding: 1.15rem 1.2rem;
    border: 1px solid rgba(255, 255, 255, 0.06);
    border-radius: 12px;
    background: rgba(255, 255, 255, 0.02);
    box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.02);
    overflow-x: auto;
  }

  .code-block code {
    display: block;
    margin: 0;
    white-space: pre-wrap;
    word-break: break-word;
    color: #b8c5d1;
    font-family:
      ui-monospace,
      SFMono-Regular,
      Menlo,
      Monaco,
      Consolas,
      "Liberation Mono",
      "Courier New",
      monospace;
    font-size: 0.95rem;
    line-height: 1.85;
  }

  .token-comment {
    color: #6f8094;
  }

  .token-key {
    color: #00ddec;
  }

  .token-string {
    color: #e7eef5;
  }

  .token-accent {
    color: #ff57b0;
  }

  /* --------------------------------------------------
     Contact
  -------------------------------------------------- */

  .contact-links {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 0.8rem;
    font-family:
      ui-monospace,
      SFMono-Regular,
      Menlo,
      Monaco,
      Consolas,
      "Liberation Mono",
      "Courier New",
      monospace;
    font-size: 0.92rem;
  }

  .contact-links a {
    color: #a7b5c3 !important;
    text-decoration: none !important;
    transition: color 0.16s ease;
  }

  .contact-links a:hover,
  .contact-links a:focus-visible {
    color: #00ddec !important;
  }

  .contact-prefix {
    color: #6f8094;
  }

  .contact-separator {
    color: #465463;
    user-select: none;
  }

  /* --------------------------------------------------
     Future work section
  -------------------------------------------------- */

  .work-list {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .work-item {
    display: grid;
    grid-template-columns: 4.4rem 1fr;
    gap: 1.2rem;
    padding: 1.05rem 0;
    border-bottom: 1px solid rgba(255, 255, 255, 0.055);
  }

  .work-item:first-child {
    border-top: 1px solid rgba(255, 255, 255, 0.055);
  }

  .work-date {
    color: #617080;
    font-size: 0.84rem;
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
    transition: color 0.16s ease;
  }

  .work-title a:hover,
  .work-title a:focus-visible {
    color: #00ddec !important;
  }

  .work-text {
    margin: 0.28rem 0 0;
    color: #8998a8;
    line-height: 1.6;
  }

  /* --------------------------------------------------
     Footer
  -------------------------------------------------- */

  .footer {
    margin-top: auto;
    padding-top: 4.6rem;
    color: #4e5c6c;
    font-size: 0.78rem;
  }

  /* --------------------------------------------------
     Mobile
  -------------------------------------------------- */

  @media (max-width: 620px) {
    .site-panel {
      width: 100%;
      padding: 3rem 1.2rem 1.8rem;
      border-left: none;
      border-right: none;
      background: rgba(3, 7, 17, 0.79);
    }

    .hero {
      grid-template-columns: 2px 1fr;
      gap: 0.9rem;
      margin-bottom: 3.2rem;
    }

    .hero-accent {
      min-height: 7.6rem;
    }

    .name {
      font-size: clamp(2.1rem, 11vw, 3rem);
    }

    .meta {
      margin-top: 0.8rem;
    }

    .section {
      margin-top: 2.5rem;
    }

    .code-block {
      padding: 1rem;
      border-radius: 10px;
    }

    .work-item {
      grid-template-columns: 1fr;
      gap: 0.2rem;
    }

    .footer {
      padding-top: 4rem;
    }
  }

  /* --------------------------------------------------
     Reduced motion
  -------------------------------------------------- */

  @media (prefers-reduced-motion: reduce) {
    #p5-network-bg {
      opacity: 0.55;
    }
  }
</style>

<div id="p5-network-bg" aria-hidden="true"></div>

<main class="site-panel">
  <header class="hero">
    <div class="hero-accent" aria-hidden="true"></div>

    <div class="hero-copy">
      <h1 class="name">Gerrit Hourigan</h1>

      <div class="meta">
        <div><strong>M.Sc. Psychology</strong> · Ulm University</div>
        <div>Data Science &amp; Applied Cognitive Science</div>
      </div>
    </div>
  </header>

  <section class="section" aria-labelledby="profile-heading">
    <h2 class="section-heading" id="profile-heading">
      <span class="slashes">//</span>
      Profile
    </h2>

    <pre class="code-block"><code><span class="token-comment"># current focus</span>
<span class="token-key">degree</span>    = <span class="token-string">"M.Sc. Psychology, Ulm University"</span>
<span class="token-key">track</span>     = [<span class="token-string">"Data Science"</span>, <span class="token-string">"Applied Cognitive Science"</span>]
<span class="token-key">interest</span>  = <span class="token-string">"statistical and computational approaches"</span>
            + <span class="token-string">" to studying human behavior"</span>

<span class="token-comment"># orientation</span>
<span class="token-key">keywords</span>  = [<span class="token-string">"statistics"</span>, <span class="token-string">"computational methods"</span>, <span class="token-string">"psychology"</span>]
<span class="token-key">status</span>    = <span class="token-accent">"student"</span></code></pre>
  </section>

  <section class="section" aria-labelledby="contact-heading">
    <h2 class="section-heading" id="contact-heading">
      <span class="slashes">//</span>
      Contact
    </h2>

    <div class="contact-links">
      <span class="contact-prefix">links =</span>

      <a href="mailto:gerrithourigan@gmail.com">"email"</a>

      <span class="contact-separator">·</span>

      <a
        href="https://github.com/g-hourigan"
        target="_blank"
        rel="noopener noreferrer"
      >
        "github"
      </a>
    </div>
  </section>

  <!--
    Uncomment this once you have something
    you genuinely want to feature.

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

  let animationPaused = false;

  const SETTINGS = {
    particleCountDesktop: 46,
    particleCountMobile: 26,
    maxNeighbors: 3,
    maxDistance: 155,
    mouseRadius: 200,
    mousePull: 0.045,
    flowScale: 0.002,
    flowSpeed: 0.002,
    flowTurns: 2.0
  };

  function setup() {
    const parent = document.getElementById("p5-network-bg");
    const canvas = createCanvas(windowWidth, windowHeight);

    canvas.parent(parent);

    pixelDensity(
      Math.min(
        window.devicePixelRatio || 1,
        2
      )
    );

    buildParticles();
    bindPointerEvents();
    bindVisibilityEvents();

    if (
      window.matchMedia &&
      window.matchMedia("(prefers-reduced-motion: reduce)").matches
    ) {
      frameRate(18);
    }
  }

  function draw() {
    if (animationPaused) {
      return;
    }

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

  function bindVisibilityEvents() {
    document.addEventListener("visibilitychange", () => {
      animationPaused = document.hidden;
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
            78,
            0
          );

          const weight = map(
            entry.distance,
            0,
            SETTINGS.maxDistance,
            1,
            0.18
          );

          stroke(0, 226, 241, alpha);
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
      fill(255, 61, 169, 17);
      circle(
        particle.x,
        particle.y,
        particle.size * 3
      );

      fill(255, 61, 169, 150);
      circle(
        particle.x,
        particle.y,
        particle.size * 1.35
      );
    }
  }

  class Particle {
    constructor() {
      this.x = random(width);
      this.y = random(height);
      this.vx = random(-0.38, 0.38);
      this.vy = random(-0.38, 0.38);
      this.seed = random(10000);
      this.size = random(1.4, 3);
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

      this.vx = (this.vx + cos(angle) * 0.055) * 0.92;
      this.vy = (this.vy + sin(angle) * 0.055) * 0.92;

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
