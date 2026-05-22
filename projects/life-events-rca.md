---
layout: default
title: Life Events and Climate Action Readiness
permalink: /projects/life-events-rca/
---

<style>
  .masthead,
  .masthead__inner-wrap,
  .site-title,
  .greedy-nav,
  .page__footer,
  .page__footer-follow,
  .page__footer-copyright,
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

  .bottom-line {
    border-color: rgba(0, 212, 255, 0.24);
    background: linear-gradient(
      180deg,
      rgba(0, 212, 255, 0.07),
      rgba(9, 15, 26, 0.92)
    );
  }

  .math-box {
    margin: 0.9rem 0;
    padding: 0.85rem 1rem;
    border: 1px solid rgba(0, 212, 255, 0.18);
    border-radius: 14px;
    background: rgba(0, 212, 255, 0.045);
    color: #dffaff;
    font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;
    font-size: 1rem;
    line-height: 1.6;
    overflow-x: auto;
  }

  .result-table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 0.9rem;
    font-size: 0.92rem;
    color: #aebdca;
  }

  .result-table th,
  .result-table td {
    border-bottom: 1px solid rgba(255, 255, 255, 0.08);
    padding: 0.65rem 0.5rem;
    text-align: left;
    vertical-align: top;
  }

  .result-table th {
    color: #f2f7fb;
    font-weight: 700;
    font-size: 0.78rem;
    letter-spacing: 0.08em;
    text-transform: uppercase;
  }

  .result-table code {
    color: #dffaff;
  }

  .model-note {
    margin-top: 0.8rem;
    color: #8c99ad !important;
    font-size: 0.94rem;
  }

  .project-figure {
    overflow: hidden;
  }

  .project-figure img {
    display: block;
    width: 100%;
    height: auto;
  }

  .project-figure-placeholder {
    padding: 4rem 1rem;
    text-align: center;
    color: #8c99ad;
    font-size: 0.95rem;
  }

  .project-figure-placeholder code {
    color: #dffaff;
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

  .reference-list {
    font-size: 0.9rem;
    color: #9fb0c2;
    line-height: 1.6;
  }

  .reference-list p + p {
    margin-top: 0.65rem;
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

    .result-table {
      font-size: 0.84rem;
    }

    .result-table th,
    .result-table td {
      padding: 0.55rem 0.35rem;
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
          I asked a simple question with a fairly technical model: when people go through
          important life events, does their readiness to support and engage in climate action
          change over time?
        </p>

        <div class="project-meta">
          <span>R</span>
          <span>lavaan</span>
          <span>SEM</span>
          <span>Latent Variables</span>
          <span>Measurement Invariance</span>
          <span>Latent Change Models</span>
          <span>Survey Data</span>
        </div>
      </section>

      <div class="project-grid">

        <section class="project-card bottom-line">
          <h2>Bottom line</h2>
          <p>
            I tested whether broad life-event exposure predicts longitudinal change in
            Readiness to Act. Some life-event domains showed meaningful structure, but the
            final latent change models did not provide evidence that the broad life-events
            factor predicted change in general readiness or its domain-specific components.
          </p>
        </section>

        <section class="project-card">
          <h2>My role</h2>
          <p>
            I prepared the data, structured the life-event item pool, ran the exploratory
            structure analyses, compared confirmatory factor models, estimated the latent
            change models, and interpreted the results in R using <code>lavaan</code>.
          </p>
        </section>

        <section class="project-card">
          <h2>The outcome, briefly</h2>
          <p>
            The outcome in this project is <strong>Readiness to Act</strong>: a broad
            climate-action construct that combines individual behavior, policy acceptance,
            and political participation.
          </p>
          <p>
            I use it because climate action is not just about private lifestyle choices.
            It also includes whether people support climate policy and whether they engage
            politically. Prior work suggests that this broader construct predicts actual
            climate-relevant behavior better than several narrower environmental constructs.
          </p>
        </section>

        <section class="project-figure">
          <img src="/assets/img/rta-framework.jpg" alt="Conceptual framework of Readiness to Act">
          <div class="project-figure-caption">
            <strong>Conceptual framework.</strong> Readiness to Act is positioned as a broad
            climate-action construct linking upstream predictors to downstream forms of action.
          </div>
        </section>

        <section class="project-card">
          <h2>What I wanted to know</h2>
          <p>
            The question was whether life events help explain change in climate-action
            readiness. In plain language: do experiences such as financial strain, health
            problems, work changes, family events, or environmental disruptions move people
            toward or away from being ready to act on climate change?
          </p>
          <p>
            The key word is <strong>change</strong>. I was not only interested in whether life
            events and readiness were related at one point in time. I wanted to know whether
            life events explain who changes more or less over time.
          </p>
        </section>

        <section class="project-card">
          <h2>The data in plain language</h2>
          <p>
            The data came from a longitudinal survey. Participants answered questions about
            their climate-action readiness at multiple time points, and they also reported
            whether they had experienced different life events.
          </p>
          <p>
            The readiness outcome was built from three kinds of climate-action indicators:
            individual climate-related behavior, support for climate policies, and political
            participation for climate protection.
          </p>
          <p>
            The life-event variables were broad and concrete. They included environmental
            experiences such as heat, drought, storms, flooding, smoke or air pollution,
            pollen, and ticks; financial strain such as welfare, late rent, dunning fees,
            negative account balance, use of food banks, or losing housing; and health-related
            events such as illness, surgery, caregiving, or psychotherapy.
          </p>
          <p>
            The wider item pool also included work, legal, family, partnership, and transition
            events, such as job changes, dismissal, moving, pregnancy, birth, separation,
            bereavement, friendship endings, legal problems, and other major life changes.
          </p>
        </section>

        <section class="project-card">
          <h2>How I studied it</h2>
          <p>
            I started by organizing binary life-event indicators into theory-guided domains:
            environmental burden, financial burden, health, work, and family or partnership.
            I then checked whether those domains actually held together empirically.
          </p>
          <p>
            After that, I explored the broader structure across all life-event items, compared
            reduced confirmatory factor models on a more coherent core of items, and finally
            tested whether a broad exploratory life-events factor predicted later change in
            Readiness to Act.
          </p>
        </section>

        <section class="project-figure">
          <div class="project-figure-placeholder">
            Domain heatmap goes here later<br>
            <code>/assets/img/domain-heatmap.png</code>
          </div>
          <div class="project-figure-caption">
            <strong>Figure 1.</strong> Within-domain associations for theory-guided life-event
            domains.
          </div>
        </section>

        <section class="project-card">
          <h2>What a latent variable is</h2>
          <p>
            A latent variable is something we care about but cannot observe directly.
            Readiness to Act is like that: there is no single perfect question that measures it.
            Instead, we infer it from several observed indicators.
          </p>

          <div class="math-box">
            observed response = latent construct + measurement error
          </div>

          <p>
            This matters because a latent model separates the underlying construct from noise
            in individual survey items. So instead of treating readiness as a simple sum score,
            the model estimates the common factor behind multiple imperfect indicators.
          </p>
        </section>

        <section class="project-card">
          <h2>Why measurement invariance matters</h2>
          <p>
            Before modeling change, we need to make sure that the construct is measured in the
            same way at both time points. Otherwise, an apparent change could simply mean that
            the measurement worked differently at T0 and T3.
          </p>
          <p>
            In simple terms: if we want to compare readiness over time, we need to use the same
            ruler twice.
          </p>

          <div class="math-box">
            λ<sub>j,T0</sub> = λ<sub>j,T3</sub><br>
            τ<sub>j,T0</sub> = τ<sub>j,T3</sub>
          </div>

          <p>
            Equal loadings <code>λ</code> mean that each indicator relates to the latent
            construct in the same way over time. Equal intercepts <code>τ</code> mean that the
            baseline level of each indicator is comparable across waves. With this in place,
            change in the latent factor is more interpretable as real change rather than a
            measurement artifact.
          </p>
        </section>

        <section class="project-card">
          <h2>The final model</h2>
          <p>
            The final model was a longitudinal latent change model. It asks: after accounting
            for people’s earlier readiness level, does the life-events factor explain who
            changed more or less over time?
          </p>

          <div class="math-box">
            g<sub>life events</sub> → latent change in RTA
          </div>

          <p>
            More technically, readiness is estimated as a latent variable at both time points:
          </p>

          <div class="math-box">
            y<sub>j,t</sub> = τ<sub>j</sub> + λ<sub>j</sub> · RTA<sub>t</sub> + ε<sub>j,t</sub>
          </div>

          <p>
            Then the model estimates change directly:
          </p>

          <div class="math-box">
            RTA<sub>T3</sub> = RTA<sub>T0</sub> + ΔRTA
          </div>

          <p>
            Finally, the life-events factor is used to predict that change:
          </p>

          <div class="math-box">
            ΔRTA = α + β · g<sub>life events</sub> + ζ
          </div>

          <p>
            The key parameter is <code>β</code>. If it were clearly positive or negative, that
            would suggest that life events explain change in Readiness to Act. In the final
            models, this was not the case.
          </p>
        </section>

        <section class="project-figure">
          <div class="project-figure-placeholder">
            CFA comparison figure goes here later<br>
            <code>/assets/img/cfa-comparison.png</code>
          </div>
          <div class="project-figure-caption">
            <strong>Figure 2.</strong> Reduced CFA comparing a broad general-factor
            representation with a more interpretable multi-factor structure.
          </div>
        </section>

        <section class="project-card">
          <h2>Going one level deeper</h2>
          <p>
            The model did not only test change in the general readiness factor. Because the
            measurement model was a bifactor model, it also separated the general
            Readiness-to-Act component from domain-specific residual components: individual
            behavior, policy acceptance, and political participation.
          </p>

          <div class="math-box">
            climate-action indicators → general RTA + domain-specific residual factors
          </div>

          <p>
            These specific factors are orthogonal to the general readiness factor. That means
            they capture what is unique to each domain after removing what all climate-action
            indicators have in common.
          </p>

          <div class="math-box">
            g<sub>life events</sub> → ΔRTA, ΔIB<sub>specific</sub>, ΔPA<sub>specific</sub>, ΔPP<sub>specific</sub>
          </div>

          <p>
            This distinction matters. A life event might not change someone’s general
            climate-action readiness, but it could still shift one specific channel. For
            example, it might affect the policy-acceptance-specific component, over and above
            the person’s general readiness to act.
          </p>
        </section>

        <section class="project-card">
          <h2>What I found</h2>
          <ul>
            <li>
              Some life-event domains showed meaningful local structure, especially
              environmental burden and financial burden.
            </li>
            <li>
              The full set of life events did not form one clean, simple global structure.
            </li>
            <li>
              In the final latent change models, the broad life-events factor did not clearly
              predict later change in general readiness or in the domain-specific residual
              components.
            </li>
          </ul>

          <table class="result-table">
            <thead>
              <tr>
                <th>Outcome predicted by life-events factor</th>
                <th>Interpretation</th>
                <th>Std. β</th>
                <th>p</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td><code>ΔRTA</code></td>
                <td>Change in general readiness</td>
                <td>.033</td>
                <td>.441</td>
              </tr>
              <tr>
                <td><code>ΔPA-specific</code></td>
                <td>Change in policy-acceptance-specific residual factor</td>
                <td>.018</td>
                <td>.636</td>
              </tr>
              <tr>
                <td><code>ΔPP-specific</code></td>
                <td>Change in political-participation-specific residual factor</td>
                <td>−.044</td>
                <td>.168</td>
              </tr>
              <tr>
                <td><code>ΔIB-specific</code></td>
                <td>Change in individual-behavior-specific residual factor</td>
                <td>−.015</td>
                <td>.598</td>
              </tr>
            </tbody>
          </table>

          <p class="model-note">
            All four estimates are close to zero and statistically unclear. So the result is
            not “life events strongly matter, but only somewhere hidden.” The pattern is more
            simply: this broad life-events factor did not explain longitudinal change in the
            broad readiness construct or in its domain-specific residual components.
          </p>
        </section>

        <section class="project-figure">
          <img src="/assets/img/cluster-structure.png" alt="Exploratory structure across the full life-event item set">
          <div class="project-figure-caption">
            <strong>Figure 3.</strong> Exploratory structure across the full life-event item set.
            This figure helps show why a simple global life-events factor is a fairly strong
            simplification of a heterogeneous event pool.
          </div>
        </section>

        <section class="project-figure">
          <div class="project-figure-placeholder">
            Final change-model figure goes here later<br>
            <code>/assets/img/change-models.png</code>
          </div>
          <div class="project-figure-caption">
            <strong>Figure 4.</strong> Final latent change models for Readiness to Act.
          </div>
        </section>

        <section class="project-card">
          <h2>How I interpret the null result</h2>
          <p>
            I do not see the null result as a failure. It is theoretically plausible.
            Readiness to Act is a broad, partly trait-like construct. Broad psychological
            dispositions are usually not expected to change strongly just because someone
            experienced more life events.
          </p>
          <p>
            This fits a broader pattern from personality psychology. Life events can be
            related to personality change, but the effects are usually relatively small,
            specific, and not always consistent. If even broad personality traits tend to show
            only modest event-related change, it would be surprising if one broad life-events
            score strongly predicted change in a broad climate-action readiness factor.
          </p>
          <p>
            My takeaway is that “life events in general” may be too blunt as a predictor.
            More specific mechanisms may matter more: financial strain, health threats,
            perceived vulnerability, environmentally relevant disruptions, or changes in
            perceived control.
          </p>
          <p>
            In other words, the result does not mean life events are irrelevant. It suggests
            that the mechanism is probably not captured well by one broad aggregate factor.
          </p>
        </section>

        <section class="project-links">
          <h2>Materials</h2>
          <p>
            <a href="/assets/files/life-events-full-analysis.html">Full analysis (HTML)</a><br>
            <a href="https://github.com/g-hourigan" target="_blank" rel="noopener noreferrer">Code / GitHub</a>
          </p>
        </section>

        <section class="project-card">
          <h2>References</h2>
          <div class="reference-list">
            <p>
              Betsch, C., Geiger, M., Lehrer, L., Sprengholz, P., Temme, H., Tiede, K.,
              & Jenny, M. (2025). <em>Psychological foundations of climate action</em>.
              Center for Open Science. https://doi.org/10.31219/osf.io/enkwy_v2
            </p>
            <p>
              Bühler, J. L., Orth, U., Bleidorn, W., Weber, E., Kretzschmar, A., Scheling,
              L., & Hopwood, C. J. (2024). <em>Life events and personality change:
              A systematic review and meta-analysis</em>. European Journal of Personality,
              38(3), 544–568. https://doi.org/10.1177/08902070231190219
            </p>
          </div>
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
