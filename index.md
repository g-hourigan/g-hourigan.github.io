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

  .gh-hero {
    text-align: center;
    padding: 1.25rem 1rem 1.15rem;
    border-bottom: 1px solid #e5e5e5;
  }

  .gh-hero h1 {
    font-size: 2.85rem;
    margin: 0 0 0.2rem;
    font-weight: 800;
    color: #111;
  }

  .gh-subtitle {
    font-size: 1.05rem;
    color: #666;
    margin: 0.2rem 0;
  }

  .gh-pronouns {
    color: #999;
    margin: 0.15rem 0 0.35rem;
    font-size: 0.9rem;
  }

  .gh-top-link {
    color: #9b7ae5 !important;
    font-weight: 700;
    text-decoration: none;
    font-size: 1rem;
  }

  .gh-page {
    max-width: 980px;
    margin: 0 auto;
    padding: 1.45rem 1.5rem 0.5rem;
  }

  .gh-intro {
    font-size: 1rem;
    line-height: 1.45;
    color: #5f6a6a;
  }

  .gh-intro p {
    margin-bottom: 0.9rem;
  }

  .gh-intro strong {
    color: #333;
  }

  .gh-intro a {
    color: #9b7ae5 !important;
    font-weight: 700;
    text-decoration: none;
  }

  .gh-intro a:hover {
    text-decoration: underline;
  }

  .gh-links {
    margin-top: 0.7rem;
    display: flex;
    gap: 1.2rem;
  }

  .gh-links a {
    color: #9b7ae5 !important;
    font-size: 0.95rem;
    font-weight: 700;
    text-decoration: none;
  }

  .gh-links a:hover,
  .gh-top-link:hover {
    text-decoration: underline;
  }

  @media (max-width: 800px) {
    .gh-hero h1 {
      font-size: 2.3rem;
    }

    .gh-subtitle {
      font-size: 0.95rem;
    }

    .gh-page {
      padding-top: 1.2rem;
    }

    .gh-intro {
      font-size: 0.98rem;
    }
  }
</style>

<section class="gh-hero">
  <h1>Gerrit Hourigan</h1>
  <p class="gh-subtitle">Psychology M.Sc. student · Data science &amp; cognitive science</p>
  <p class="gh-pronouns">(he/him)</p>
  <a class="gh-top-link" href="/cv/">CV</a>
</section>

<section class="gh-page">
  <div class="gh-intro">
    <p>
      <strong>Hi!</strong> I’m Gerrit, an incoming Psychology M.Sc. student with a data science
      and cognitive science focus. I’m interested in using statistics, machine learning,
      and behavioral data to understand cognition, decision-making, and performance.
    </p>

    <p>
      I completed my Bachelor’s degree at Leuphana University Lüneburg and will start my Master's degree this October.
      I am currently a research assistant at
      <a href="https://www.uni-ulm.de/in/psy-pers/" target="_blank" rel="noopener noreferrer">
        Mattis Geiger's Personality Psychology Lab
      </a>.
    </p>

    <p>
      Apart from academics, I’m a competitive chess player, currently around 2300 Elo and FM,
      and I am working towards earning the International Master title. I enjoy being active,
      hiking, travelling, and I’m always up for an adventure.
    </p>
    <p>
      In the future, I am planing to present some of my analyses and results here.
    </p>


  </div>

  <section class="projects-section">

<h2>Selected Projects</h2>

<div class="project-card">
  <div class="project-label">Behavioral Data Science · Quantitative Research</div>

  <h3>Life Events and Climate Action Readiness</h3>

  <p>
    I tested whether life events measured at T3 predicted latent change in
    readiness for climate action from T0 to T3. The project combines survey data
    preparation, measurement checks, factor-score construction, and latent
    difference score modeling in R.
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

</section>

  <div class="gh-links">
    <a href="mailto:gerrithourigan@gmail.com">Email</a>
    <a href="https://github.com/g-hourigan">GitHub</a>
  </div>
</section>
