---
layout: default
title: Life Events and Climate Action Readiness
permalink: /projects/life-events-rca/
---

<section class="case-study">

<p class="eyebrow">Behavioral Data Science · Quantitative Research</p>

# Life Events and Climate Action Readiness

<p class="lead">
I analyzed whether life events measured at T3 predicted individual change in
readiness for climate action between T0 and T3. The analysis used longitudinal
survey data and latent difference score modeling to study behavioral change while
accounting for measurement structure.
</p>

<div class="case-meta">
  <div>
    <strong>Role</strong>
    <p>Data preparation, statistical modeling, interpretation, reporting</p>
  </div>
  <div>
    <strong>Tools</strong>
    <p>R, R Markdown, lavaan, dplyr, ggplot2, psych</p>
  </div>
  <div>
    <strong>Methods</strong>
    <p>EFA/CFA, factor-score construction, latent difference score modeling</p>
  </div>
</div>

## Research question

Do life events measured at T3 explain latent change in readiness for climate
action from T0 to T3?

## Why this mattered

Simple observed difference scores can be noisy, especially when the construct of
interest is measured through multiple survey items. I therefore modeled readiness
for climate action as a latent construct over time and tested whether life events
predicted latent change rather than only raw score differences.

## Analysis pipeline

<div class="pipeline">
  <div>Raw T3 life-event items</div>
  <span>↓</span>
  <div>Binary recoding and missing-data checks</div>
  <span>↓</span>
  <div>Exploratory measurement checks</div>
  <span>↓</span>
  <div>CFA-based factor-score construction</div>
  <span>↓</span>
  <div>Latent difference score model</div>
  <span>↓</span>
  <div>Test: life events → change in climate action readiness</div>
</div>

## Technical approach

The life-event items were dichotomous indicators of whether a person had
experienced a specific event. I recoded the items, inspected their frequency
distributions, and examined their correlation structure. I then evaluated a
pragmatic general life-event factor for downstream modeling.

Readiness for climate action was modeled longitudinally using a latent difference
score model. This allowed the analysis to estimate change at the latent level and
test whether the life-event factor predicted individual differences in that
change.

## Main result

The broad life-event factor did not show convincing evidence of predicting latent
change in climate action readiness. This suggests that a global life-event score
may be too coarse and that future analyses should test more targeted hypotheses
around specific event domains, such as financial strain, health events, or
climate-related experiences.

## What this project demonstrates

- Building a reproducible end-to-end R analysis workflow
- Working with messy longitudinal behavioral survey data
- Preparing and validating psychological/behavioral indicators
- Using latent variable models instead of naive observed change scores
- Interpreting null results without overclaiming
- Translating complex statistical output into a clear research conclusion

## Data availability

The raw data are not publicly available because they contain sensitive survey
responses. The public version of this project focuses on the research question,
analysis strategy, model logic, and selected outputs.

</section>
