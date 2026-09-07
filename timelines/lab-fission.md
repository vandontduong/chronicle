---
layout: default
title: Lab fission
permalink: /timelines/lab-fission/
---

# Lab fission

<p class="meta">Where people went, what thesis they took, and the work that proved it.</p>

Read as **forks, not a calendar**. The OpenAI and Anthropic *firms* (charter, landlords, product cadence) live on [OpenAI]({{ '/timelines/openai/' | relative_url }}) and [Anthropic]({{ '/timelines/anthropic/' | relative_url }}). The 2025–26 Musk stack is canonical on [SpaceX]({{ '/timelines/spacex/' | relative_url }}) and [clouds]({{ '/timelines/clouds/' | relative_url }}). This page keeps the theses and the papers that justified leaving.

## 2015-12 — OpenAI founded

Nonprofit research lab. Musk, Altman, Sutskever, Brockman and others. Charter: AGI that benefits humanity. Early work is RL plus open tools; the scientific line that later becomes ChatGPT is already here.

The papers that matter for the *forks*:

- **PPO** (2017). Default policy-gradient algorithm for a decade of LLM post-training. [arXiv:1707.06347](https://arxiv.org/abs/1707.06347)
- **Learning from human preferences** (2017, with DeepMind). Reward model from pairwise judgments — the RLHF primitive. [arXiv:1706.03741](https://arxiv.org/abs/1706.03741)
- **InstructGPT** (2022). RLHF makes a smaller model beat a larger base in human evals. [arXiv:2203.02155](https://arxiv.org/abs/2203.02155)

GPT-1 through GPT-4 and the Microsoft / Amazon deals sit on [OpenAI]({{ '/timelines/openai/' | relative_url }}). Architecture and scale sit on [capability stack]({{ '/timelines/capability-stack/' | relative_url }}).

People who later leave (Amodei, Sutskever, Schulman, Murati) are on those three papers.

## 2018 — Musk leaves the OpenAI board

Control and direction fight. No new architecture drops with the exit. The scientific residue is the GPT / RLHF line staying at OpenAI. Musk's later bet is a separate lab, not a paper — see 2023 xAI, then [SpaceX]({{ '/timelines/spacex/' | relative_url }}).

## 2021-02 — Anthropic founded

Amodei cohort leaves OpenAI. Thesis: a frontier lab whose alignment method is part of the product, not a side team.

- **HHH** (2021–22). Helpful, honest, harmless as the evaluation frame. [arXiv:2112.00861](https://arxiv.org/abs/2112.00861) · [arXiv:2204.05862](https://arxiv.org/abs/2204.05862)
- **Constitutional AI** (2022). Harmlessness from AI feedback plus a written constitution. [arXiv:2212.08073](https://arxiv.org/abs/2212.08073) · [Anthropic](https://www.anthropic.com/research/constitutional-ai-harmlessness-from-ai-feedback)
- **Scaling monosemanticity** (2024). Dictionary learning on a production model. [Anthropic](https://www.anthropic.com/research/mapping-mind-language-model)

Landlords, Claude cadence, MCP, computer use: [Anthropic]({{ '/timelines/anthropic/' | relative_url }}). Methods also on [post-training]({{ '/timelines/post-training/' | relative_url }}) and [safety]({{ '/timelines/safety/' | relative_url }}).

## 2023-03 — xAI founded

Musk. Thesis: a frontier model tied to X, shipped fast, less safety theater. Early science is model releases, not a new training paradigm.

- [Announcing Grok](https://x.ai/blog/grok) (2023-11)
- [Grok-1 open weights](https://x.ai/blog/grok-os) (2024-03). 314B MoE, Apache 2.0.

**2025–26 continuation** (X combination, SpaceX takeout, Cursor, Colossus rents, IPO, Starmind) is on [SpaceX]({{ '/timelines/spacex/' | relative_url }}). Landlord economics on [clouds]({{ '/timelines/clouds/' | relative_url }}).

## 2023-11 — OpenAI board crisis

Altman fired and restored in days. Not a methods paper. The scientific shadow is who walks:

- [Superalignment](https://openai.com/index/introducing-superalignment/) (Sutskever and Leike, 2023)
- Leike → Anthropic. Sutskever → SSI. Schulman → Anthropic briefly → Thinking Machines.

The capability work (GPT-4 class, then o-series) stays at OpenAI. See [OpenAI]({{ '/timelines/openai/' | relative_url }}) and [post-training]({{ '/timelines/post-training/' | relative_url }}).

## 2024-06 — Safe Superintelligence (SSI)

Sutskever, Gross, Levy. Thesis: one product, safe superintelligence; no side products, no public research cadence. By design there is almost nothing to cite except the founding note and later compute deals.

- Founding statement, 19 Jun 2024. [ssi.inc](https://ssi.inc)
- Sutskever takes CEO after Gross exits (2025). [TechCrunch](https://techcrunch.com/2025/07/03/ilya-sutskever-will-lead-safe-superintelligence-following-his-ceos-exit/)
- Nvidia partnership (2026). [TechCrunch](https://techcrunch.com/2026/07/27/ilya-sutskevers-safe-superintelligence-partners-with-nvidia-to-scale-its-ai-research/)

Intellectual prior: [Superalignment](https://openai.com/index/introducing-superalignment/). Missing paper is the point. Also on [RSI]({{ '/timelines/rsi/' | relative_url }}).

## 2024-09 / 2025-02 — Thinking Machines Lab

Murati leaves OpenAI; Zoph, Weng, then Schulman as chief scientist. Thesis opposite SSI: ship infrastructure and open weights so other people can do post-training.

- [Tinker](https://thinkingmachines.ai/tinker/) (2025-10)
- [Inkling](https://thinkingmachines.ai/news/inkling-small/) (2026-07)

Schulman's earlier scientific payload is still PPO + InstructGPT.

## 2024–26 — Second wave

The field is no longer three labs and a long tail. Most of these are product or world-model bets, not a new transformer paper.

- **Reflection AI** (Laskin, Antonoglou, ex-DeepMind). Agents / code systems.
- **World Labs** (Fei-Fei Li). Spatial / world models. Prior: ImageNet + *NeuroAI* [arXiv:2210.08340](https://arxiv.org/abs/2210.08340). Also [world models]({{ '/timelines/world-models/' | relative_url }}).
- **AMI Labs** (LeCun, 2025). JEPA thesis. Prior: [arXiv:2301.08243](https://arxiv.org/abs/2301.08243).
- **Discovery Loop** (2026). Treat as a beat until they publish.
- **Meta Superintelligence Labs** (2025). Science still sits in the Llama reports until a real paper lands.

## What this page is not

A cap table. A launch calendar. Company pages exist so this page can stay a list of *arguments that left*.
