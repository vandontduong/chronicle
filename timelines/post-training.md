---
layout: default
title: Post-training
permalink: /timelines/post-training/
---

# Post-training

<p class="meta">How raw next-token models became usable — and then reasoners</p>

## 2017 — Preferences as a reward

Before InstructGPT: learn a reward from pairwise human judgments, then RL. Joint OpenAI / DeepMind result. This is the primitive RLHF still uses.

- Christiano et al. *Deep reinforcement learning from human preferences*. [arXiv:1706.03741](https://arxiv.org/abs/1706.03741) · [alphaXiv](https://www.alphaxiv.org/abs/1706.03741) · [OpenAI](https://openai.com/index/learning-from-human-preferences/)
- Schulman et al. *Proximal Policy Optimization Algorithms*. [arXiv:1707.06347](https://arxiv.org/abs/1707.06347) · [alphaXiv](https://www.alphaxiv.org/abs/1707.06347)

## 2022-03 — InstructGPT / RLHF

SFT on demonstrations, reward model on rankings, PPO against that reward. A 1.3B aligned model beats 175B GPT-3 in human evals. This is the ChatGPT stack.

- Ouyang et al. *Training language models to follow instructions with human feedback*. [arXiv:2203.02155](https://arxiv.org/abs/2203.02155) · [alphaXiv](https://www.alphaxiv.org/abs/2203.02155)
- [ChatGPT](https://openai.com/index/chatgpt/)

## 2022-04 / 2022-12 — HHH and Constitutional AI

Anthropic's frame: helpful, honest, harmless. Then harmlessness from *AI* feedback plus a written constitution — less labeling, more inspectable rules.

- Bai et al. *Training a Helpful and Harmless Assistant with RLHF*. [arXiv:2204.05862](https://arxiv.org/abs/2204.05862) · [alphaXiv](https://www.alphaxiv.org/abs/2204.05862)
- Bai et al. *Constitutional AI: Harmlessness from AI Feedback*. [arXiv:2212.08073](https://arxiv.org/abs/2212.08073) · [alphaXiv](https://www.alphaxiv.org/abs/2212.08073) · [Anthropic](https://www.anthropic.com/research/constitutional-ai-harmlessness-from-ai-feedback)
- [Claude's constitution](https://www.anthropic.com/research/claudes-constitution)

## 2023-05 — DPO

Skip the explicit reward model and the PPO loop. Treat the LM as already a reward model; train on preference pairs. Cheaper, stabler, widely copied.

- Rafailov et al. *Direct Preference Optimization*. [arXiv:2305.18290](https://arxiv.org/abs/2305.18290) · [alphaXiv](https://www.alphaxiv.org/abs/2305.18290)

## 2023-05 — Process rewards

Grade the *steps*, not just the final answer. Lightman et al. show process supervision beats outcome supervision on MATH. A bridge to o1-class training.

- Lightman et al. *Let's Verify Step by Step*. [arXiv:2305.13763](https://arxiv.org/abs/2305.13763) · [alphaXiv](https://www.alphaxiv.org/abs/2305.13763)

## 2024–25 — RL for reasoning

Post-training becomes a second training run. OpenAI publishes evals (o1), not the recipe. DeepSeek publishes the recipe (GRPO, outcome RL).

- [Learning to reason with LLMs](https://openai.com/index/learning-to-reason-with-llms/)
- OpenAI. *o1 System Card*. [arXiv:2412.16720](https://arxiv.org/abs/2412.16720) · [alphaXiv](https://www.alphaxiv.org/abs/2412.16720)
- Shao et al. *DeepSeekMath* (introduces GRPO). [arXiv:2402.03300](https://arxiv.org/abs/2402.03300)
- DeepSeek-AI. *DeepSeek-R1*. [arXiv:2501.12948](https://arxiv.org/abs/2501.12948) · [alphaXiv](https://www.alphaxiv.org/abs/2501.12948)

Also on: [capability stack]({{ '/timelines/capability-stack/' | relative_url }}), [lab fission]({{ '/timelines/lab-fission/' | relative_url }}).
