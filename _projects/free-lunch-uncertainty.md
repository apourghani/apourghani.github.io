---
layout: page
title: "Free Lunch Uncertainty: Sequence-Level Rényi Entropy from Particle Decoding for Adaptive LLM Reasoning"
description: >-
  Quantifying uncertainty over an entire LLM completion is critical for selective prediction and adaptive compute. Zero-cost signals such as mean token entropy and log-probability are local to tokens or to one completion, and self-consistency needs many extra completions.
  We show that Sequential Monte Carlo (SMC) decoding for power sampling already estimates the normalizing constant of the power distribution, which gives the sequence-level Rényi entropy (SRE) of the model’s completion distribution at zero marginal cost, with a guarantee at every particle budget. A Rényi chain rule extends this readout to a family of stepwise entropies of any order.
  We prove that orders above one are tied to the most likely token of each step, which explains why they track log-probability, while the order-1/2 member accumulates the log of per-step search effort. This member is the best zero-cost selective-prediction signal in 10 of 13 settings. On MATH500 its AUROC is 0.022 to 0.044 above log-probability with all four models and within length quartiles, and the same order is selected when each setting is held out.
  An 8-particle probe identifies the problems that benefit from more particles, and a two-pass policy matches 64-particle accuracy on MATH500 with 34.2% fewer particles over three seeds.
summary: >-
  We estimate uncertainty over an entire LLM answer from statistics already computed during particle decoding. Using sequence-level Rényi entropy to decide when to allocate more particles matched the 64-particle baseline’s accuracy on MATH500 while using 34.2% fewer particles.
img: "https://arxiv.org/html/2611.13414v1/overview-2.png"
img_alt: "Adaptive particle allocation using sequence-level Rényi entropy"
importance: 1
category: research
---

<figure>
  <img class="img-fluid" src="{{ page.img }}" alt="{{ page.img_alt | escape }}">
  <figcaption class="caption">Figure 1 · CC BY 4.0</figcaption>
</figure>

Erfan Baghaei Potraghloo, Milad Heidari Sorkhehdizaj, Shahab Rahimirad, Aliasghar Pourghani, Seyedarmin Azizi, Souvik Kundu, Abolfazl Hashemi, Joseph Campbell, and Vijay Gupta

[arXiv](https://arxiv.org/abs/2611.13414v1) · [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
