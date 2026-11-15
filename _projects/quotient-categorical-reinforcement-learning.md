---
layout: page
title: "Quotient-Categorical Representations for Bellman-Compatible Average-Reward Distributional Reinforcement Learning"
description: >-
  Average-reward reinforcement learning requires estimating the gain and a state-dependent bias, which solves the Poisson equation only up to an additive constant. Distributional analogues of the bias inherit this same ambiguity. We introduce a quotient-space formulation in which state-indexed laws are identified up to a common translation, together with a categorical parameterization that respects this symmetry.
  On this space, we define a projected average-reward distributional operator and show that it is well-defined, non-expansive in a coordinate Cramér metric, and admits fixed points. We interpret the projected fixed points through geometrically-stopped differential returns, whose categorical operators are contractive and whose fixed points converge in the Abel sense to a canonical fixed point of the projected undiscounted operator.
  We show that the means of the projected fixed points match the scalar bias up to an error caused by endpoint clipping of the categorical projections, and we bound this error. Finally, we establish almost-sure convergence and finite-iteration residual bounds for temporal-difference recursions with gain-centered rewards under i.i.d. and Markovian sampling.
  When the gain is unknown, we couple the recursion with an online gain estimator and prove the same guarantees under Markovian sampling, with a bound on the gain error.
summary: >-
  We use a quotient-categorical representation to model differential returns in average-reward reinforcement learning. It respects the common-shift ambiguity of the bias, and we prove convergence of the resulting temporal-difference updates even when the average reward is estimated online.
img: "https://arxiv.org/html/2605.11289v2/fig2_convergence.svg"
img_alt: "Convergence of categorical temporal-difference learning in a five-state Markov decision process"
importance: 2
category: research
---

<figure>
  <img class="img-fluid" src="{{ page.img }}" alt="{{ page.img_alt | escape }}">
  <figcaption class="caption">Figure 2 · CC BY 4.0</figcaption>
</figure>

Ege C. Kaya, Aliasghar Pourghani, Vijay Gupta, and Abolfazl Hashemi

NeurIPS 2026 · [arXiv](https://arxiv.org/abs/2605.11289v2) · [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
