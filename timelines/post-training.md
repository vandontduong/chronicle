---
layout: default
title: Post-training
permalink: /timelines/post-training/
---

# Post-training

<p class="meta">How raw next-token models became usable — and then reasoners</p>

## 2022-03 — InstructGPT / RLHF

Human preferences as a reward model. A small aligned model beats a much larger base model in human evals. This is the ChatGPT stack.

- Paper: [Training language models to follow instructions with human feedback](https://arxiv.org/abs/2203.02155) · [alphaXiv](https://www.alphaxiv.org/abs/2203.02155)

## 2022-12 — Constitutional AI

Harmlessness from AI feedback plus a written constitution. Anthropic's alternative to pure RLHF labeling.

- Paper: [Constitutional AI](https://arxiv.org/abs/2212.08073) · [alphaXiv](https://www.alphaxiv.org/abs/2212.08073)

## 2023-05 — DPO

Skip the explicit reward model. The LM is already a reward model. Cheaper preference training; widely copied.

- Paper: [Direct Preference Optimization](https://arxiv.org/abs/2305.18290) · [alphaXiv](https://www.alphaxiv.org/abs/2305.18290)

## 2024–25 — RL for reasoning

Process rewards, outcome RL on math/code, long chain-of-thought. o1 / R1-class models. Post-training becomes a second training run, not a polish step.
