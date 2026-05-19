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
      radial-gradient(circle at 20% 20%, rgba(0, 212, 255, 0.08), transparent 28%),
      radial-gradient(circle at 80% 15%, rgba(255, 78, 205, 0.08), transparent 24%),
      radial-gradient(circle at 50% 80%, rgba(0, 212, 255, 0.05), transparent 30%),
      #050914;
    color: #dbe7ef;
    font-family: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    overflow-x: hidden;
  }

  ::selection {
    background: rgba(255, 78, 205, 0.25);
    color: #ffffff;
  }

  ::-moz-selection {
    background: rgba(255, 78, 205, 0.25);
    color: #ffffff;
  }

  #network-bg {
    position: fixed;
    inset: 0;
    width: 100%;
    height: 100%;
    z-index: 0;
    pointer-events: none;
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
      rgba(8, 13, 24, 0.88) 0%,
      rgba(6, 10, 18, 0.94) 100%
    );
    box-shadow:
      0 0 0 1px rgba(255, 255, 255, 0.02) inset,
      0 30px 80px rgba(0, 0, 0, 0.35),
      0 0 80px rgba(0, 212, 255, 0.06);
    backdrop-filter: blur(12px);
    -webkit-backdrop-filter: blur(12px);
    padding: 2rem 2rem 1.6rem;
  }

  .site-panel::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
      linear-gradient(90deg, rgba(0, 212, 255, 0.06), transparent 18%, transparent 82%, rgba(255, 78, 205, 0.05)),
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

  .identity-line {
    position: relative;
    z-index: 1;
    margin: 0 0 0.45rem;
    font-size: 0.96rem;
    font-weight: 700;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: #00d4ff;
  }

  .hero-title {
    position: relative;
    z-index: 1;
    margin: 0;
    max-width: 950px;
    font-size: clamp(2.2rem, 5vw, 4rem);
    line-height: 1.08;
    letter-spacing: -0.045em;
    font-weight: 800;
    color: #f4f8fb;
  }

  .hero-title .accent {
    color: #b8f7ff;
    text-decoration: underline;
    text-decoration-thickness: 2px;
    text-decoration-color: rgba(255, 78, 205, 0.75);
    text-underline-offset: 0.16em;
  }

  .hero-subtitle {
    position: relative;
    z-index: 1;
    max-width: 840px;
    margin: 1rem 0 0;
    font-size: 1.08rem;
    line-height: 1.7;
    color: #aebdca;
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
    line-height: 1.7;
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

<canvas id="network-bg" aria-hidden="true"></canvas>

<section class="site-shell">
  <div class="site-panel">
    <p class="section-label">// HOME</p>
    <p class="identity-line">Gerrit Hourigan</p>

    <h1 class="hero-title">
      I work at the intersection of
      <span class="accent">psychology</span>,
      <span class="accent">statistics</span>, and
      <span class="accent">machine learning</span>.
    </h1>

    <p class="hero-subtitle">
      I build and analyze research and data projects grounded in behavioral science,
      with a focus on cognition, decision-making, performance, and real-world data.
    </p>

    <div class="hero-links">
      <a href="/cv/">CV</a>
      <a href="mailto:gerrithourigan@gmail.com">Email</a>
      <a href="https://github.com/g-hourigan" target="_blank" rel="noopener noreferrer">GitHub</a>
    </div>

    <div class="welcome-card">
      <p>
        Welcome. This site is intentionally minimal: you can find ways to contact me,
        browse selected work, and get a quick sense of the questions I like to work on.
      </p>
      <p>
        I completed my B.Sc. in Psychology at Leuphana University Lüneburg and am now
        continuing into the M.Sc. while working on research and data analysis projects.
        My interests sit where behavioral theory meets empirical modeling.
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
          Measurement, latent variables, longitudinal data, individual differences,
          and behavioral outcomes that matter outside the lab.
        </p>
      </div>

      <div class="info-card">
        <p class="card-title">Tools</p>
        <p>
          R, SEM, survey data workflows, reproducible analysis, and increasingly
          machine learning methods for behavioral and cognitive data.
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
        BUILD: PSYCHOLOGY × DATA × ML
      </div>
    </div>

    <p class="meta-note">
      Interface: GitHub Pages / Jekyll / custom canvas network background.
    </p>
  </div>
</section>

<script>
  (function () {
    const canvas = document.getElementById("network-bg");
    if (!canvas) return;

    const ctx = canvas.getContext("2d");
    if (!ctx) return;

    const prefersReducedMotion = window.matchMedia("(prefers-reduced-motion: reduce)").matches;

    let width = 0;
    let height = 0;
    let nodes = [];
    let animationFrameId;

    function resizeCanvas() {
      width = window.innerWidth;
      height = window.innerHeight;
      canvas.width = width * window.devicePixelRatio;
      canvas.height = height * window.devicePixelRatio;
      canvas.style.width = width + "px";
      canvas.style.height = height + "px";
      ctx.setTransform(window.devicePixelRatio, 0, 0, window.devicePixelRatio, 0, 0);
      createNodes();
    }

    function createNodes() {
      const mobile = width < 700;
      const count = mobile ? 28 : 52;
      nodes = [];

      for (let i = 0; i < count; i++) {
        const isAccent = Math.random() > 0.72;

        nodes.push({
          x: Math.random() * width,
          y: Math.random() * height,
          vx: prefersReducedMotion ? 0 : (Math.random() - 0.5) * 0.35,
          vy: prefersReducedMotion ? 0 : (Math.random() - 0.5) * 0.35,
          r: isAccent ? 2.6 : 1.8,
          color: isAccent
            ? (Math.random() > 0.5 ? "255,78,205" : "0,212,255")
            : "180,205,230"
        });
      }
    }

    function updateNodes() {
      for (const node of nodes) {
        node.x += node.vx;
        node.y += node.vy;

        if (node.x <= 0 || node.x >= width) node.vx *= -1;
        if (node.y <= 0 || node.y >= height) node.vy *= -1;
      }
    }

    function drawBackgroundGlow() {
      const gradient = ctx.createRadialGradient(
        width * 0.52,
        height * 0.42,
        0,
        width * 0.52,
        height * 0.42,
        Math.max(width, height) * 0.55
      );
      gradient.addColorStop(0, "rgba(0, 212, 255, 0.035)");
      gradient.addColorStop(0.45, "rgba(255, 78, 205, 0.02)");
      gradient.addColorStop(1, "rgba(0, 0, 0, 0)");
      ctx.fillStyle = gradient;
      ctx.fillRect(0, 0, width, height);
    }

    function drawConnections() {
      const maxDistance = width < 700 ? 120 : 155;

      for (let i = 0; i < nodes.length; i++) {
        for (let j = i + 1; j < nodes.length; j++) {
          const a = nodes[i];
          const b = nodes[j];
          const dx = a.x - b.x;
          const dy = a.y - b.y;
          const distance = Math.sqrt(dx * dx + dy * dy);

          if (distance < maxDistance) {
            const alpha = 1 - distance / maxDistance;
            ctx.beginPath();
            ctx.moveTo(a.x, a.y);
            ctx.lineTo(b.x, b.y);
            ctx.strokeStyle = `rgba(70, 150, 210, ${alpha * 0.18})`;
            ctx.lineWidth = 1;
            ctx.stroke();
          }
        }
      }
    }

    function drawNodes() {
      for (const node of nodes) {
        ctx.beginPath();
        ctx.arc(node.x, node.y, node.r, 0, Math.PI * 2);
        ctx.fillStyle = `rgba(${node.color}, 0.95)`;
        ctx.fill();
      }
    }

    function render() {
      ctx.clearRect(0, 0, width, height);
      drawBackgroundGlow();
      if (!prefersReducedMotion) updateNodes();
      drawConnections();
      drawNodes();
      animationFrameId = window.requestAnimationFrame(render);
    }

    resizeCanvas();
    render();

    window.addEventListener("resize", function () {
      window.cancelAnimationFrame(animationFrameId);
      resizeCanvas();
      render();
    });
  })();
</script>
