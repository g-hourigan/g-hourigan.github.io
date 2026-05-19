---
layout: default
title: Life Events and Climate Action Readiness
permalink: /projects/life-events-rca/
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
    margin: 1.4rem 0 1.2rem;
    background: linear-gradient(
      90deg,
      rgba(255, 255, 255, 0.08),
      rgba(255, 255, 255, 0.02)
    );
  }

  .project-shell {
    position: relative;
    z-index: 1;
    max-width: 940px;
  }

  .project-hero,
  .project-card,
  .project-figure,
  .project-links {
    border: 1px solid rgba(114, 134, 170, 0.16);
    border-radius: 18px;
    background: linear-gradient(
      180deg,
      rgba(14, 21, 35, 0.92),
      rgba(9, 15, 26, 0.92)
    );
    box-shadow: 0 12px 30px rgba(0, 0, 0, 0.16);
  }

  .project-hero,
  .project-card,
  .project-links {
    padding: 1.25rem 1.3rem;
  }

  .project-hero {
    margin-bottom: 1rem;
  }

  .top-nav {
    position: relative;
    z-index: 1;
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem;
    margin-bottom: 1rem;
  }

  .top-nav a {
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
    text-decoration: none !important;
    transition: color 0.2s ease, border-color 0.2s ease, transform 0.2s ease;
  }

  .top-nav a:hover,
  .project-links a:hover {
    color: #ff71d6 !important;
    border-color: rgba(255, 113, 214, 0.32);
    transform: translateY(-1px);
  }

  .project-kicker {
    margin: 0 0 0.55rem;
    font-size: 0.82rem;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: #8c99ad;
    font-weight: 700;
  }

  .project-hero h1 {
    margin: 0;
    font-size: clamp(2rem, 4vw, 3rem);
    line-height: 1.05;
    letter-spacing: -0.04em;
    color: #f4f8fb;
  }

  .project-subtitle {
    margin: 0.85rem 0 0;
    max-width: 760px;
    font-size: 1.03rem;
    line-height: 1.7;
    color: #aebdca;
  }

  .project-meta {
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
    margin-top: 1rem;
  }

  .project-meta span {
    display: inline-flex;
    align-items: center;
    padding: 0.28rem 0.62rem;
    border-radius: 999px;
    border: 1px solid rgba(170, 187, 211, 0.14);
    background: rgba(255, 255, 255, 0.03);
    color: #a9b6c4;
    font-size: 0.74rem;
    font-weight: 700;
  }

  .project-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1rem;
  }

  .project-card h2,
  .project-links h2 {
    margin: 0 0 0.8rem;
    font-size: 0.95rem;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: #f2f7fb;
  }

  .project-card p,
  .project-links p {
    margin: 0;
    color: #aebdca;
    line-height: 1.72;
  }

  .project-card p + p,
  .project-card ul,
  .project-links p + p {
    margin-top: 0.8rem;
  }

  .project-card ul {
    padding-left: 1.1rem;
    color: #aebdca;
    line-height: 1.7;
  }

  .project-card li + li {
    margin-top: 0.45rem;
  }

  .project-figure {
    overflow: hidden;
  }

  .project-figure img {
    display: block;
    width: 100%;
    height: auto;
  }

  .project-figure-caption {
    padding: 0.9rem 1rem 1rem;
    border-top: 1px solid rgba(255, 255, 255, 0.06);
    color: #9fb0c2;
    line-height: 1.6;
    font-size: 0.95rem;
  }

  .project-links a {
    color: #00d4ff !important;
    text-decoration: none !important;
    font-weight: 700;
  }

  .footer-row {
    position: relative;
    z-index: 1;
    display: grid;
    grid-template-columns: 1fr auto;
    gap: 1rem;
    align-items: start;
    margin-top: 1.4rem;
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

    .footer-row {
      grid-template-columns: 1fr;
    }

    .system-meta {
      text-align: left;
    }

    .project-subtitle {
      font-size: 1rem;
    }
  }

  @media (max-width: 640px) {
    .top-nav {
      gap: 0.6rem;
    }

    .top-nav a {
      width: 100%;
      justify-content: center;
    }
  }
</style>

<div id="p5-network-bg" aria-hidden="true"></div>

<section class="site-shell">
  <div class="site-panel">
    <p class="section-label">// PROJECT</p>

    <div class="project-shell">
      <nav class="top-nav">
        <a href="/">Home</a>
        <a href="/cv/">CV</a>
        <a href="https://github.com/g-hourigan" target="_blank" rel="noopener noreferrer">GitHub</a>
      </nav>

      <section class="project-hero">
        <p class="project-kicker">Life Events × Climate Action</p>
        <h1>Life Events and Climate Action Readiness</h1>
        <p class="project-subtitle">
          Do recent life events help explain change in readiness for climate action over time?
          This project combines theory-guided domain building, exploratory structure analysis,
          reduced CFA, and latent change modeling in R.
        </p>

        <div class="project-meta">
          <span>R</span>
          <span>lavaan</span>
          <span>SEM</span>
          <span>Latent Change Models</span>
          <span>Survey Data</span>
          <span>Life Events</span>
        </div>
      </section>

      <div class="project-grid">

        <section class="project-card">
          <h2>Overview</h2>
          <p>
            This project examined whether life events measured at T3 were associated with
            subsequent change in readiness for climate action. The analysis moved from
            theory-guided life-event domains to exploratory structure analysis, then to a
            reduced confirmatory factor model and finally to latent change models.
          </p>
        </section>

        <section class="project-card">
          <h2>Conceptual background</h2>
          <p>
            Readiness to Act is the broader conceptual framework behind the outcome studied
            here. It can be understood as a latent readiness construct shaped by factors
            such as knowledge, trust, perceived risks, self-efficacy, social norms, and
            perceived policy effectiveness, and expressed in outcomes such as policy
            acceptance, political participation, and individual behavior.
          </p>
          <p>
            Including this framework helps clarify what kind of construct this project is
            trying to explain over time before moving into the life-event analyses.
          </p>
        </section>

        <section class="project-figure">
          <img src="/assets/img/rta-framework.jpg" alt="Conceptual framework of Readiness to Act showing predictors and indicators">
          <div class="project-figure-caption">
            <strong>Conceptual framework.</strong> Readiness to Act can be understood as a
            latent readiness construct positioned between upstream predictors and downstream
            forms of action-related response. In this project, the longitudinal analyses
            focus on change in this broader readiness construct over time.
          </div>
        </section>

        <section class="project-card">
          <h2>Approach</h2>
          <ul>
            <li>Recoded and prepared binary life-event indicators.</li>
            <li>Grouped items into theory-guided domains such as environmental burden, financial burden, health, work, and family/partnership.</li>
            <li>Inspected within-domain coherence using phi correlations.</li>
            <li>Explored the overall structure of all life-event items using clustering and exploratory factor analysis.</li>
            <li>Compared a reduced general-factor CFA against a reduced multi-factor CFA on a coherent core of items.</li>
            <li>Built an exploratory life-event general factor score and tested it in latent change models for readiness for climate action.</li>
          </ul>
        </section>

        <section class="project-card">
          <h2>Key findings</h2>
          <ul>
            <li>
              Some local structure was visible in the theory-guided domains, especially for
              environmental burden and financial burden, where within-domain associations
              looked more coherent than in several other parts of the item set.
            </li>
            <li>
              The full life-event pool did not support one simple, clean global structure,
              which is why the confirmatory step focused on a reduced and more interpretable
              subset of items rather than the complete item set.
            </li>
            <li>
              For the longitudinal models, an exploratory life-event general factor score
              was used as a pragmatic summary indicator.
            </li>
            <li>
              Across the latent change models, there was no convincing evidence that this
              broad life-event summary factor predicted later change in readiness for climate action.
            </li>
          </ul>
        </section>

        <section class="project-figure">
          <img src="/assets/img/domain-heatmap.png" alt="Heatmap of within-domain phi correlations for theory-guided life-event domains">
          <div class="project-figure-caption">
            <strong>Figure 1.</strong> Within-domain phi correlations for theory-guided life-event
            domains. This view is useful for showing that some domains are more internally
            coherent than others.
          </div>
        </section>

        <section class="project-figure">
          <img src="/assets/img/cluster-structure.png" alt="Exploratory cluster structure of all life-event items">
          <div class="project-figure-caption">
            <strong>Figure 2.</strong> Exploratory structure across the full life-event item set.
            This figure is there to communicate that the overall system does not collapse
            neatly into one simple global factor.
          </div>
        </section>

        <section class="project-figure">
          <img src="/assets/img/cfa-comparison.png" alt="Reduced CFA comparison of general-factor and multi-factor models">
          <div class="project-figure-caption">
            <strong>Figure 3.</strong> Reduced CFA on a coherent core of items. The goal here is
            not to present every parameter estimate, but to show how the reduced confirmatory
            step was used to compare a general-factor representation against a more interpretable
            multi-factor structure.
          </div>
        </section>

        <section class="project-figure">
          <img src="/assets/img/change-models.png" alt="Summary of latent change models predicting readiness for climate action">
          <div class="project-figure-caption">
            <strong>Figure 4.</strong> Latent change models for readiness for climate action.
            The substantive takeaway is that the exploratory broad life-events factor did not
            provide convincing evidence of explaining later change.
          </div>
        </section>

        <section class="project-card">
          <h2>Interpretation</h2>
          <p>
            The analysis suggests that life events are not best understood here as a single
            highly coherent global construct. Some thematic groupings are visible, but once
            the analysis is pushed into longitudinal change models, the broad exploratory
            summary factor does not appear to explain meaningful variation in later readiness
            for climate action.
          </p>
          <p>
            In practical terms, that means a simple “more life events leads to more change in
            climate action readiness” story is not supported in these models. A more promising
            route may be to focus on narrower event classes or better theoretically targeted
            event mechanisms instead of relying on one broad aggregate score.
          </p>
        </section>

        <section class="project-links">
          <h2>Materials</h2>
          <p>
            <a href="/assets/files/life-events-full-analysis.html">Full analysis (HTML)</a><br>
            <a href="https://github.com/g-hourigan" target="_blank" rel="noopener noreferrer">Code / GitHub</a>
          </p>
        </section>

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
