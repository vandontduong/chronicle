---
layout: default
title: Post-training
permalink: /timelines/post-training/
---

# Post-training

<p class="meta">How raw next-token models became usable — and then reasoners</p>

Three regimes, in order: **imitate** (SFT), **prefer** (RLHF / DPO / constitutions), **search** (process rewards, then RL-for-reasoning). Pretraining lives on [capability stack]({{ '/timelines/capability-stack/' | relative_url }}). Who left with which recipe lives on [lab fission]({{ '/timelines/lab-fission/' | relative_url }}).

## 2017 — Preferences as a reward

Learn a reward from pairwise human judgments, then RL. Joint OpenAI / DeepMind. PPO is the optimizer that survives into the LLM era. InstructGPT is this paper plus a language model.

- Christiano et al. *Deep reinforcement learning from human preferences*. [arXiv:1706.03741](https://arxiv.org/abs/1706.03741) · [OpenAI](https://openai.com/index/learning-from-human-preferences/)
- Schulman et al. *Proximal Policy Optimization Algorithms*. [arXiv:1707.06347](https://arxiv.org/abs/1707.06347)

## 2021-06 — Cheap adaptation

LoRA: freeze the base, train low-rank adapters. The reason open SFT is a weekend job instead of a second pretrain. Not a new alignment method; the substrate under every later preference run that is not full-weight.

- Hu et al. *LoRA: Low-Rank Adaptation of Large Language Models*. [arXiv:2106.09685](https://arxiv.org/abs/2106.09685)

## 2022-03 — InstructGPT / RLHF

SFT on demonstrations, reward model on rankings, PPO against that reward. A 1.3B aligned model beats 175B GPT-3 in human evals. ChatGPT (Nov) is the same stack with a chat UI — the event that puts every other lab on a product clock.

- Ouyang et al. *Training language models to follow instructions with human feedback*. [arXiv:2203.02155](https://arxiv.org/abs/2203.02155)
- [ChatGPT](https://openai.com/index/chatgpt/)

## 2022-03 / 2022-12 — Bootstrap, then a constitution

STaR: the model generates rationales, keeps the ones that reach the right answer, fine-tunes on those. Self-Instruct: the model writes its own SFT set. Then Anthropic: harmlessness from *AI* feedback plus a written constitution.

- Zelikman et al. *STaR: Bootstrapping Reasoning With Reasoning*. [arXiv:2203.14465](https://arxiv.org/abs/2203.14465)
- Wang et al. *Self-Instruct*. [arXiv:2212.10560](https://arxiv.org/abs/2212.10560)
- Bai et al. *Training a Helpful and Harmless Assistant with RLHF*. [arXiv:2204.05862](https://arxiv.org/abs/2204.05862)
- Bai et al. *Constitutional AI*. [arXiv:2212.08073](https://arxiv.org/abs/2212.08073) · [Anthropic](https://www.anthropic.com/research/constitutional-ai-harmlessness-from-ai-feedback)
- [Claude's constitution](https://www.anthropic.com/research/claudes-constitution)

## 2023-05 — DPO

Skip the explicit reward model and the PPO loop. Treat the LM as already a reward model; train on preference pairs. Cheaper, stabler, the default in open post-training (Zephyr, Tülu, and the copies).

- Rafailov et al. *Direct Preference Optimization*. [arXiv:2305.18290](https://arxiv.org/abs/2305.18290)

## 2023-05 — Process rewards

Grade the *steps*, not just the final answer. Lightman et al. show process supervision beats outcome supervision on MATH. A bridge to o1-class training: you can RL against a process, not only a yes/no.

- Lightman et al. *Let's Verify Step by Step*. [arXiv:2305.13763](https://arxiv.org/abs/2305.13763)

## 2024–25 — RL for reasoning

Post-training becomes a second training run, sometimes larger than SFT. OpenAI publishes evals (o1), not the recipe. DeepSeekMath introduces GRPO; R1 publishes the outcome-RL path to a reasoner. After R1, "base ⇒ reasoner" is assumed to be cheap — that claim is also an [efficiency]({{ '/timelines/efficiency/' | relative_url }}) beat.

- [Learning to reason with LLMs](https://openai.com/index/learning-to-reason-with-llms/)
- OpenAI. *o1 System Card*. [arXiv:2412.16720](https://arxiv.org/abs/2412.16720)
- Shao et al. *DeepSeekMath* (GRPO). [arXiv:2402.03300](https://arxiv.org/abs/2402.03300)
- DeepSeek-AI. *DeepSeek-R1*. [arXiv:2501.12948](https://arxiv.org/abs/2501.12948)

## 2025-10 — Post-training as a service

Thinking Machines' Tinker is an API: you send the job, they run the cluster. The thesis of that lab (opposite SSI) is that *other people* should be able to do this section. [lab fission]({{ '/timelines/lab-fission/' | relative_url }}).

- [Tinker](https://thinkingmachines.ai/tinker/)

## What this page is not

Pretrain architecture and scale: [capability stack]({{ '/timelines/capability-stack/' | relative_url }}). Agent loops that *use* a post-trained model: [agents]({{ '/timelines/agents/' | relative_url }}). Outer loops that rewrite prompts or code: [RSI]({{ '/timelines/rsi/' | relative_url }}).
