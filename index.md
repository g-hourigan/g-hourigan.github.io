---
layout: default
title: Home
---

<style>
  .masthead,
  .masthead__inner-wrap,
  .greedy-nav,
  .page__footer {
    display: none !important;
  }

  .initial-content {
    margin-top: 0 !important;
  }

  ::selection {
    background: rgba(155, 122, 229, 0.35);
    color: #111;
  }

  ::-moz-selection {
    background: rgba(155, 122, 229, 0.35);
    color: #111;
  }

  body {
    background: #f7f7f7;
  }

  .gh-hero {
    max-width: 1080px;
    margin: 0 auto;
    padding: 1rem 1.5rem 0.8rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 1.5rem;
    border-bottom: 1px solid #e5e5e5;
  }

  .gh-hero h1 {
    font-size: clamp(1.9rem, 4vw, 2.5rem);
    margin: 0;
    font-weight: 800;
    letter-spacing: -0.04em;
    color: #111;
    line-height: 1;
  }

  .gh-subtitle {
    font-size: 0.95rem;
    color: #666;
    margin: 0.35rem 0 0;
  }

  .gh-nav {
    display: flex;
    gap: 1rem;
    align-items: center;
    flex-wrap: wrap;
  }

  .gh-nav a {
    color: #9b7ae5 !important;
    font-size: 0.95rem;
    font-weight: 700;
    text-decoration: none;
  }

  .gh-nav a:hover {
    text-decoration: underline;
  }

  .gh-page {
    max-width: 1080px;
    margin: 0 auto;
    padding: 1rem 1.5rem 1.5rem;
  }

  .home-grid {
    display: grid;
    grid-template-columns: 1.05fr 0.95fr;
    gap: 1rem;
    align-items: start;
  }

  .intro-card,
  .project-card,
  .mini-card {
    border: 1px solid #e5e5e5;
    border-radius: 18px;
    padding: 1.15rem;
    background: #fff;
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.04);
  }

  .intro-card h2,
  .project-card h2,
  .mini-card h3 {
    margin-top: 0;
    margin-bottom: 0.55rem;
    color: #111;
  }

  .intro-card h2 {
    font-size: 1.45rem;
  }

  .project-card h2 {
    font-size: 1.35rem;
  }

  .mini-card h3 {
    font-size: 1rem;
  }

  .intro-card p,
  .project-card p,
  .mini-card p {
    line-height: 1.48;
    margin: 0 0 0.75rem;
    color: #566;
    font-size: 0.98rem;
  }

  .intro-card p:last-child,
  .project-card p:last-child,
  .mini-card p:last-child {
    margin-bottom: 0;
  }

  .intro-card a,
  .project-link {
    color: #9b7ae5 !important;
    font-weight: 700;
    text-decoration: none;
  }

  .intro-card a:hover,
  .project-link:hover {
    text-decoration: underline;
  }

  .project-label {
    font-size: 0.72rem;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    color: #777;
    font-weight: 700;
    margin-bottom: 0.5rem;
  }

  .project-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
    margin: 0.75rem 0 0.8rem;
  }

  .project-tags span {
    border: 1px solid #ddd;
    border-radius: 999px;
    padding: 0.2rem 0.55rem;
    font-size: 0.78rem;
    background: #fafafa;
    color: #555;
  }

  .mini-grid {
    grid-column: 1 / -1;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1rem;
  }

  .mini-card p {
    font-size: 0.92rem;
  }

  @media (max-width: 850px) {
    .gh-hero {
      flex-direction: column;
      align-items: flex-start;
      gap: 0.7rem;
    }

    .home-grid,
    .mini-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<header class="gh-hero">
  <div>
    <h1>Gerrit Hourigan</h1>
    <p class="gh-subtitle">Psychology · Behavioral Data Science · Cognitive Science</p>
  </div>

  <nav class="gh-nav">
    <a href="/cv/">CV</a>
    <a href="mailto:gerrithourigan@gmail.com">Email</a>
    <a href="https://github.com/g-hourigan" target="_blank" rel="noopener noreferrer">GitHub</a>
  </nav>
</header>

<main class="gh-page">
  <section class="home-grid">

    <div class="intro-card">
      <h2>Hi, I’m Gerrit.</h2>

      <p>
        I’m an incoming Psychology M.Sc. student interested in using statistics,
        machine learning, and behavioral data to understand cognition,
        decision-making, and performance.
      </p>

      <p>
        I completed my Bachelor’s degree at Leuphana University Lüneburg and am
        currently a research assistant at
        <a href="https://www.uni-ulm.de/in/psy-pers/" target="_blank" rel="noopener noreferrer">
          Mattis Geiger's Personality Psychology Lab
        </a>.
      </p>

      <p>
        Outside academics, I’m a competitive chess player around 2300 Elo and FM,
        working toward the International Master title.
      </p>
    </div>

    <div class="project-card">
      <div class="project-label">Featured Project</div>

      <h2>Life Events and Climate Action Readiness</h2>

      <p>
        Tested whether life events measured at T3 predicted latent change in
        readiness for climate action from T0 to T3 using latent difference score
        modeling in R.
      </p>

      <div class="project-tags">
        <span>R</span>
        <span>lavaan</span>
        <span>Longitudinal Modeling</span>
        <span>Latent Variables</span>
        <span>Survey Data</span>
      </div>

      <a class="project-link" href="/projects/life-events-rca/">
        Read case study →
      </a>
    </div>

    <div class="mini-grid">
      <div class="mini-card">
        <h3>Focus</h3>
        <p>Behavioral data science, quantitative UX research, cognition, decision-making, and performance.</p>
      </div>

      <div class="mini-card">
        <h3>Methods</h3>
        <p>Statistical modeling, longitudinal survey analysis, latent variables, R, and reproducible reporting.</p>
      </div>

      <div class="mini-card">
        <h3>Background</h3>
        <p>Psychology B.Sc., data science internship experience, research assistant work, and competitive chess.</p>
      </div>
    </div>

  </section>
</main>
