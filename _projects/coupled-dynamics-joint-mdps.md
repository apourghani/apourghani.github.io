---
layout: page
title: "Learning to Control Coupled-Dynamics Environments with Joint Markov Decision Processes"
description: >-
  Coupled-dynamics environments expose the one-step outcomes that would follow from several possible counterfactual actions under a common realization of exogenous randomness. The ordinary Markov decision process formalism allows one to reason about the marginal law of each action but discards dependence across these counterfactual outcomes. The Joint Markov decision process (JMDP) formalism preserves that dependence.
  Prior work established the formalism and solved the fixed-policy joint moment evaluation problem in JMDPs. This paper develops optimal-control methods. We define a nonparametric distributional Bellman optimality operator for JMDPs, and prove that when the induced marginal MDP has a unique optimal policy, its iterates converge in Wasserstein distance to the optimal joint return law.
  For the first two moments, we establish convergence under a weaker condition that permits several mean-optimal actions as long as their tie resolutions share a second-moment fixed point. We also derive sampled targets for neural approximation.
summary: >-
  We develop optimal-control methods for environments where different actions share the same randomness. Joint Markov decision processes preserve the dependence between these counterfactual outcomes, and we prove when Bellman updates recover their joint return distribution.
img: "https://arxiv.org/html/2608.22765v1/gridworld_moment_ground_truth.png"
img_alt: "Joint moment control and action correlations in a windy gridworld"
importance: 3
category: research
---

<figure>
  <img class="img-fluid" src="{{ page.img }}" alt="{{ page.img_alt | escape }}">
  <figcaption class="caption">Figure 3 · CC BY 4.0</figcaption>
</figure>

Ege C. Kaya, Aliasghar Pourghani, Mahsa Ghasemi, Vijay Gupta, and Abolfazl Hashemi

[arXiv](https://arxiv.org/abs/2608.22765v1) · [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
