---
layout: default
title: Robotics
permalink: /timelines/robotics/
---

# Robotics

<p class="meta">The loop leaves the desktop. A policy that outputs joint commands, not tokens in a browser.</p>

Desktop agents stay on [agents]({{ '/timelines/agents/' | relative_url }}). Learned simulators stay on [world models]({{ '/timelines/world-models/' | relative_url }}). Games-as-science stay on [DeepMind]({{ '/timelines/deepmind/' | relative_url }}). This page is the vision-language-action line: internet semantics in, motor tokens out.

## 2018-06 — QT-Opt

Kalashnikov et al.: a single Q-function, seven real robots, hundreds of thousands of grasp attempts. Scaled off-policy RL on hardware. Not a foundation model. Proof that *more real data* beats a cleverer sim.

- Kalashnikov et al. *QT-Opt*. [arXiv:1806.10293](https://arxiv.org/abs/1806.10293)

## 2022-12 — RT-1

A transformer trained on 130k real episodes, language in, discretized actions out. One policy, many kitchen tasks, on the same Google robot. The architecture is small (~35M). The claim is *scale of robot data*.

- Brohan et al. *RT-1: Robotics Transformer for Real-World Control at Scale*. [arXiv:2212.06817](https://arxiv.org/abs/2212.06817)

## 2023-04 — ALOHA

Zhao et al.: two low-cost arms, action chunking, imitation that can zip a bag and slot a battery. The hardware is cheap enough to copy. Later π0 demos run on this platform.

- Zhao et al. *Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware*. [arXiv:2304.13705](https://arxiv.org/abs/2304.13705)

## 2023-07 — RT-2

Fine-tune a web VLM (PaLI-X class) so action tokens sit in the same vocabulary as words. “Pick up the object that puts out a fire” works because the web already taught “extinguisher.” VLA becomes the name.

- Brohan et al. *RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control*. [arXiv:2307.15818](https://arxiv.org/abs/2307.15818)

## 2023-10 — Open X-Embodiment

Many labs, many arms, one pool (~1M trajectories). RT-1-X and RT-2-X trained across embodiments beat the single-robot baseline. The scarce object is a *shared* robot corpus, not another architecture.

- Open X-Embodiment Collaboration. *Open X-Embodiment*. [arXiv:2310.08864](https://arxiv.org/abs/2310.08864)

## 2024-06 / 2024-10 — Open twin, then flow

OpenVLA: a 7B open VLA you can fine-tune. π0 (Physical Intelligence): flow matching on a smaller VLM backbone, bimanual dexterity (fold laundry, clear a table), inference on a 4090-class box. Closed API plus later open checkpoints. The lab is a fork of the RT line, not a new transformer.

- Kim et al. *OpenVLA*. [arXiv:2406.09246](https://arxiv.org/abs/2406.09246)
- Black et al. *π0: A Vision-Language-Action Flow Model for General Robot Control*. [arXiv:2410.24164](https://arxiv.org/abs/2410.24164) · [Physical Intelligence](https://www.physicalintelligence.company/blog/pi0)

## What this page is not

A humanoid cap table (Figure, Optimus, Boston Dynamics) unless a paper or a shipped policy changes the stack. Cosmos as a *simulator SKU* stays on [world models]({{ '/timelines/world-models/' | relative_url }}). Gato as a generalist agent stays on [DeepMind]({{ '/timelines/deepmind/' | relative_url }}).
