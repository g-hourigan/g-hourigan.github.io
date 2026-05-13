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
    text-align: center;
    padding: 1rem 1rem 0.85rem;
    border-bottom: 1px solid #e5e5e5;
  }

  .gh-hero h1 {
    font-size: clamp(2.1rem, 5vw, 3rem);
    margin: 0 0 0.25rem;
    font-weight: 800;
    letter-spacing: -0.04em;
    color: #111;
    line-height: 1.05;
  }

  .gh-subtitle {
    font-size: 1rem;
    color: #666;
    margin: 0.2rem 0;
  }

  .gh-pronouns {
    color: #999;
    margin: 0.1rem 0 0.4rem;
    font-size: 0.9rem;
  }

  .gh-links {
    display: flex;
    justify-content: center;
    gap: 1.2rem;
    flex-wrap: wrap;
    margin-top: 0.35rem;
  }

  .gh-links a {
    color: #9b7ae5 !important;
    font-size: 0.95rem;
    font-weight: 700;
    text-decoration: none;
  }

  .gh-links a:hover {
    text-decoration: underline;
  }

  .gh-page {
    max-width: 900px;
    margin: 0 auto;
    padding: 1.2rem 1.5rem 1.5rem;
  }

  .intro-card,
  .project-card {
    border: 1px solid #e5e5e5;
    border-radius: 18px;
    background: #fff;
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.04);
  }

  .intro-card {
    padding: 1.25rem 1.35rem;
    margin-bottom: 0.95rem;
  }

  .project-card {
    padding: 1rem 1.15rem;
  }

  .intro-card p,
  .project-card p {
    line-height: 1.5;
    color: #566;
    margin: 0 0 0.8rem;
  }

  .intro-card p {
    font-size: 1rem;
  }

  .project-card p {
    font-size: 0.94rem;
    line-height: 1.45;
  }

  .intro-card p:last-child,
  .project-card p:last-child {
    margin-bottom: 0;
  }

  .intro-card strong {
    color: #333;
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

  .projects-section h2 {
    font-size: 1.15rem;
    margin: 0 0 0.55rem;
    color: #111;
  }

  .project-card h3 {
    margin: 0 0 0.45rem;
    font-size: 1.18rem;
    color: #111;
  }

  .project-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.35rem;
    margin: 0.65rem 0 0.7rem;
  }

  .project-tags span {
    border: 1px solid #ddd;
    border-radius: 999px;
    padding: 0.16rem 0.48rem;
    font-size: 0.72rem;
    background: #fafafa;
    color: #555;
  }

  .project-link {
    display: inline-block;
    font-size: 0.9rem;
    font-weight: 700;
  }

  @media (max-width: 800px) {
    .gh-hero h1 {
      font-size: 2.25rem;
    }

    .gh-page {
      padding: 1rem 1rem 1.4rem;
    }

    .intro-card {
      padding: 1.1rem;
    }

    .project-card {
      padding: 0.95rem;
    }
  }
</style>

<section class="gh-hero">
  <h1>Gerrit Hourigan</h1>

  <p class="gh-subtitle">
    Psychology M.Sc. student 
  </p>

  <p class="gh-pronouns">(he/him)</p>

  <div class="gh-links">
    <a href="/cv/">CV</a>
    <a href="mailto:gerrithourigan@gmail.com">Email</a>
  </div>
</section>

<section class="gh-page">

  <div class="intro-card">
    <p>
      <strong>Hi!</strong> I’m Gerrit, an incoming Psychology M.Sc. student with a focus on
      data science, cognitive science, and behavioral data. I’m interested in using
      statistics, machine learning, and psychological theory to understand cognition,
      decision-making, and performance.
    </p>

    <p>
      I completed my Bachelor’s degree at Leuphana University Lüneburg and am currently
      a research assistant at
      <a href="https://www.uni-ulm.de/in/psy-pers/" target="_blank" rel="noopener noreferrer">
        Mattis Geiger's Personality Psychology Lab
      </a>.
    </p>

    <p>
      Outside academics, I’m a competitive chess player around 2300 Elo and FM,
      working toward the International Master title.
    </p>
  </div>

  <section class="projects-section">
    <h2>Selected Project</h2>

    <div class="project-card">
      <h3>Life Events and Climate Action Readiness</h3>

      <p>
        I tested whether life events measured at T3 predicted latent change in
        readiness for climate action from T1 to T3. The project combines survey data
        preparation, measurement invariance, SEM, and latent
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
        Read project →
      </a>
    </div>
  </section>

</section>
