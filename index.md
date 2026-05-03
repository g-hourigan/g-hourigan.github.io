---
layout: default
title: Home
---

<style>
  .masthead,
.greedy-nav {
  display: none !important;
}

.initial-content {
  margin-top: 0 !important;
}
  /* Remove blue footer strip */
.page__footer {
  display: none !important;
}

/* Make text-selection highlight violet instead of black/blue */
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
    padding: 3rem 1rem 2.5rem;
    border-bottom: 1px solid #e5e5e5;
  }

  .gh-hero h1 {
    font-size: 3.2rem;
    margin: 0 0 0.4rem;
    font-weight: 800;
    color: #111;
  }

  .gh-subtitle {
    font-size: 1.35rem;
    color: #666;
    margin: 0.5rem 0;
  }

  .gh-pronouns {
    color: #999;
    margin: 0.5rem 0;
  }

  .gh-top-link {
    color: #9b7ae5;
    font-weight: 700;
    text-decoration: none;
    font-size: 1.1rem;
  }

  .gh-page {
    max-width: 1120px;
    margin: 0 auto;
    padding: 3rem 1.5rem;
    display: grid;
    grid-template-columns: 1.6fr 0.8fr;
    gap: 4rem;
    align-items: start;
  }

  .gh-intro {
    font-size: 1.15rem;
    line-height: 1.75;
    color: #5f6a6a;
  }

  .gh-intro p {
    margin-bottom: 1.6rem;
  }

  .gh-intro strong {
    color: #333;
  }

  .gh-profile {
    text-align: center;
  }

  .gh-profile img {
    width: 100%;
    max-width: 330px;
    border-radius: 10px;
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.08);
  }

  .gh-links {
    margin-top: 1.2rem;
    display: flex;
    justify-content: center;
    gap: 1rem;
    flex-wrap: wrap;
  }

  .gh-links a {
    color: #9b7ae5;
    font-size: 0.9rem;
    font-weight: 600;
    text-decoration: none;
  }

  .gh-links a:hover,
  .gh-top-link:hover {
    text-decoration: underline;
  }

  @media (max-width: 800px) {
    .gh-hero h1 {
      font-size: 2.4rem;
    }

    .gh-page {
      grid-template-columns: 1fr;
      gap: 2rem;
    }

    .gh-profile {
      order: -1;
    }
  }
</style>

<section class="gh-hero">
  <h1>Gerrit Hourigan</h1>
  <p class="gh-subtitle">Psychology M.Sc. student · Data science focus</p>
  <p class="gh-pronouns">chess · cognition · statistics · machine learning</p>
  <a class="gh-top-link" href="/cv/">CV</a>
</section>

<section class="gh-page">
  <div class="gh-intro">
    <p>
      <strong>Hi!</strong> I’m Gerrit, an incoming Psychology M.Sc. student with a data science focus.
      I’m interested in using statistics, machine learning, and behavioral data to understand cognition,
      decision-making, and performance.
    </p>


    <p>
      Apart from academics, I’m a competitive chess player, I enjoy travelling, running, and lifting,
      and I’m always up for a challenge.
    </p>
  </div>

  <aside class="gh-profile">

    <div class="gh-links">
      <a href="mailto:YOUR_EMAIL">Email</a>
      <a href="https://github.com/g-hourigan">GitHub</a>
      <a href="/projects/">Projects</a>
      <a href="/about/">About</a>
    </div>
  </aside>
</section>
