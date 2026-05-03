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
  padding: 2.2rem 1rem 2rem;
  border-bottom: 1px solid #e5e5e5;
}

.gh-hero h1 {
  font-size: 3.2rem;
  margin: 0 0 0.4rem;
  font-weight: 800;
  color: #111;
}

.gh-subtitle {
  font-size: 1.25rem;
  color: #666;
  margin: 0.35rem 0;
}

.gh-pronouns {
  color: #999;
  margin: 0.35rem 0 0.6rem;
  font-size: 1rem;
}

.gh-top-link {
  color: #9b7ae5;
  font-weight: 700;
  text-decoration: none;
  font-size: 1.1rem;
}

.gh-page {
  max-width: 850px;
  margin: 0 auto;
  padding: 3rem 1.5rem 1rem;
}

.gh-intro {
  font-size: 1.18rem;
  line-height: 1.7;
  color: #5f6a6a;
}

.gh-intro p {
  margin-bottom: 1.5rem;
}

.gh-intro strong {
  color: #333;
}

.gh-links {
  margin-top: 1.5rem;
  display: flex;
  gap: 1.2rem;
}

.gh-links a {
  color: #9b7ae5;
  font-size: 1rem;
  font-weight: 700;
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

  .gh-subtitle {
    font-size: 1.05rem;
  }

  .gh-page {
    padding-top: 2rem;
  }

  .gh-intro {
    font-size: 1.05rem;
  }
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

<section class="gh-page">
  <div class="gh-intro">
    <p>
      <strong>Hi!</strong> I’m Gerrit, an incoming Psychology M.Sc. student with a data science
      and cognitive science focus. I’m interested in using statistics, machine learning,
      and behavioral data to understand cognition, decision-making, and performance.
    </p>

    <p>
      Apart from academics, I’m a competitive chess player. I enjoy being active,
      hiking, travelling, and I’m always up for an adventure.
    </p>
  </div>

  <div class="gh-links">
    <a href="mailto:gerrithourigan@gmail.com">Email</a>
    <a href="https://github.com/g-hourigan">GitHub</a>
  </div>
</section>
