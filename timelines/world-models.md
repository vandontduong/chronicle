---
layout: default
title: World models
permalink: /timelines/world-models/
---

# World models

<p class="meta">Predict the next state, then act in it. Video generators that claim to be simulators sit here. Chat agents that call tools sit on [agents]({{ '/timelines/agents/' | relative_url }}).</p>

Games-as-science also live on [DeepMind]({{ '/timelines/deepmind/' | relative_url }}). Sora as an OpenAI product beat is a pointer from [OpenAI]({{ '/timelines/openai/' | relative_url }}).

## 2018-03 — Ha and Schmidhuber

A VAE compresses the frame; an MDN-RNN predicts the next latent; a small controller trains *inside* the dream. The name “world model” for the current field starts here.

- Ha and Schmidhuber. *World Models*. [arXiv:1803.10122](https://arxiv.org/abs/1803.10122)

## 2019-11 / 2019-12 — MuZero and Dreamer

MuZero learns the dynamics it needs for search without being told the rules. Dreamer learns a latent dynamics model and backprops through imagined rollouts. Two labs, same bet: planning in a learned simulator.

- Schrittwieser et al. *Mastering Atari, Go, Chess and Shogi by Planning with a Learned Model*. [arXiv:1911.08265](https://arxiv.org/abs/1911.08265)
- Hafner et al. *Dream to Control*. [arXiv:1912.01603](https://arxiv.org/abs/1912.01603)

## 2023-01 — DreamerV3

One set of hyperparameters across discrete and continuous control. First published run to get a Minecraft diamond from scratch without human data. World-model RL as a general algorithm, not a domain trick.

- Hafner et al. *Mastering Diverse Domains through World Models*. [arXiv:2301.04104](https://arxiv.org/abs/2301.04104) · later [Nature](https://www.nature.com/articles/s41586-025-08744-2)

## 2023-09 — GAIA-1

Wayve: video + text + action tokens as a driving world model. The application is cars; the method is the same next-state bet.

- Hu et al. *GAIA-1: A Generative World Model for Autonomous Driving*. [arXiv:2309.17080](https://arxiv.org/abs/2309.17080)

## 2024-02 — Genie and Sora

Genie: interactive 2D worlds from unlabeled video, action-controllable. Sora: a diffusion transformer on spacetime patches; OpenAI frames it as a *world simulator* and does not release a recipe. Two different products, one claim — scale video, get physics. DeepMind moved the Genie-1 launch off `/discover/blog/`.

- Bruce et al. *Genie: Generative Interactive Environments*. [arXiv:2402.15391](https://arxiv.org/abs/2402.15391) · [DeepMind publication](https://deepmind.google/research/publications/60474/)
- [Video generation models as world simulators](https://openai.com/index/video-generation-models-as-world-simulators/)

## 2024-04 — V-JEPA

LeCun line: predict missing parts of a video representation, not pixels. A world model that is not a generator.

- Bardes et al. *Revisiting Feature Prediction for Learning Visual Representations from Video* (V-JEPA). [arXiv:2404.08471](https://arxiv.org/abs/2404.08471)

## 2024-12 / 2025-08 — Genie 2 and Genie 3

Genie 2: 3D, action-controllable, minutes of consistency from an image. Genie 3: real-time 720p interaction. The DeepMind claim is now a foundation *environment* for agents, not a demo reel.

- [Genie 2](https://deepmind.google/blog/genie-2-a-large-scale-foundation-world-model/)
- [Genie 3](https://deepmind.google/blog/genie-3-a-new-frontier-for-world-models/)

## What this page is not

A Veo / Runway / Kling product log. Text-to-video ships here only when the lab argues the model is a simulator (Sora, Genie). Robot policies that consume a world model belong on a robotics page when that page exists.
