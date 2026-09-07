---
layout: default
title: Lab fission
permalink: /timelines/lab-fission/
---

# Lab fission

<p class="meta">Where people went, what thesis they took, and the work that proved it</p>

Read as **forks, not a calendar**. The 2025–26 Musk stack (X, SpaceX, Cursor, Colossus rents) is canonical on [SpaceX]({{ '/timelines/spacex/' | relative_url }}) and [clouds]({{ '/timelines/clouds/' | relative_url }}). This page keeps the *theses* and the papers.

## 2015-12 — OpenAI founded

Nonprofit research lab. Musk, Altman, Sutskever, Brockman and others. Charter: AGI that benefits humanity. Early work is RL + open tools; the scientific line that later becomes ChatGPT is already here.

**Advances**

- **PPO** (2017). Default policy-gradient algorithm for a decade of LLM post-training. [arXiv:1707.06347](https://arxiv.org/abs/1707.06347) · [OpenAI blog](https://openai.com/index/openai-baselines-ppo/)
- **Learning from human preferences** (2017, with DeepMind). Reward model from pairwise judgments — the RLHF primitive. [arXiv:1706.03741](https://arxiv.org/abs/1706.03741) · [OpenAI blog](https://openai.com/index/learning-from-human-preferences/)
- **GPT-1** (2018). Generative pre-training, then fine-tune. [PDF](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf) · [OpenAI](https://openai.com/index/language-unsupervised/)
- **GPT-2** (2019). Unsupervised multitask learner; staged release as a safety experiment. [PDF](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf) · [blog](https://openai.com/index/better-language-models/)
- **GPT-3** (2020). In-context learning at 175B. [arXiv:2005.14165](https://arxiv.org/abs/2005.14165)
- **InstructGPT** (2022). RLHF makes a smaller model beat a larger base model in human evals. [arXiv:2203.02155](https://arxiv.org/abs/2203.02155)
- **ChatGPT** (2022-11). Same stack, chat UI. [OpenAI post](https://openai.com/index/chatgpt/)
- **GPT-4** (2023). [arXiv:2303.08774](https://arxiv.org/abs/2303.08774)

People who later leave (Amodei, Sutskever, Schulman, Murati) are on these papers.

## 2018 — Musk leaves the OpenAI board

Control and direction fight. No new architecture drops with the exit. The scientific residue is the GPT/RLHF line above staying at OpenAI; Musk's later bet is a separate lab, not a paper.

## 2021-02 — Anthropic founded

Amodei cohort leaves OpenAI. Thesis: a frontier lab whose alignment method is part of the product, not a side team.

**Advances**

- **HHH / helpful-honest-harmless assistant** (2021–22). The lab's evaluation frame. [arXiv:2112.00861](https://arxiv.org/abs/2112.00861) · [arXiv:2204.05862](https://arxiv.org/abs/2204.05862)
- **Constitutional AI** (2022). Harmlessness from AI feedback plus a written constitution. [arXiv:2212.08073](https://arxiv.org/abs/2212.08073) · [Anthropic](https://www.anthropic.com/research/constitutional-ai-harmlessness-from-ai-feedback)
- **Claude's constitution** (2023, revised 2026). [Anthropic](https://www.anthropic.com/research/claudes-constitution)
- **Scaling monosemanticity** (2024). [Anthropic](https://www.anthropic.com/research/mapping-mind-language-model)

Also on: [post-training]({{ '/timelines/post-training/' | relative_url }}).

## 2023-03 — xAI founded

Musk. Thesis: a frontier model tied to X, shipped fast, less safety theater. Early science is model releases, not a new training paradigm.

- **Announcing Grok** (2023-11). [xAI](https://x.ai/blog/grok)
- **Grok-1 open weights** (2024-03). 314B MoE, Apache 2.0. [xAI](https://x.ai/blog/grok-os) · [github.com/xai-org/grok-1](https://github.com/xai-org/grok-1)

**2025–26 continuation** (X combination, SpaceX takeout, Cursor, Colossus rents, IPO, Starmind) is on [SpaceX]({{ '/timelines/spacex/' | relative_url }}). Landlord economics on [clouds]({{ '/timelines/clouds/' | relative_url }}).

## 2023-11 — OpenAI board crisis

Altman fired and restored in days. Not a methods paper. The scientific shadow is who walks:

- **Superalignment** framing (Sutskever & Leike, 2023). [OpenAI](https://openai.com/index/introducing-superalignment/)
- Leike → Anthropic. Sutskever → SSI. Schulman → Anthropic briefly → Thinking Machines.

The capability work (GPT-4 class, then o-series) stays at OpenAI. See [capability stack]({{ '/timelines/capability-stack/' | relative_url }}) and [post-training]({{ '/timelines/post-training/' | relative_url }}).

## 2024-06 — Safe Superintelligence (SSI)

Sutskever, Gross, Levy. Thesis: one product, safe superintelligence; no side products, no public research cadence. By design there is almost nothing to cite except the founding note and later compute deals.

- Founding statement, 19 Jun 2024. [ssi.inc](https://ssi.inc) · [X thread](https://x.com/ssi/status/1803472825476587910)
- Sutskever takes CEO after Gross exits (2025). [TechCrunch](https://techcrunch.com/2025/07/03/ilya-sutskever-will-lead-safe-superintelligence-following-his-ceos-exit/)
- Nvidia partnership / scale-up (2026). [TechCrunch](https://techcrunch.com/2026/07/27/ilya-sutskevers-safe-superintelligence-partners-with-nvidia-to-scale-its-ai-research/)

Intellectual prior: [Superalignment](https://openai.com/index/introducing-superalignment/).

## 2024-09 / 2025-02 — Thinking Machines Lab

Murati leaves OpenAI; Zoph, Weng, then Schulman as chief scientist. Thesis opposite SSI: ship infrastructure and open weights so other people can do post-training.

- **Tinker** (2025-10). [thinkingmachines.ai/tinker](https://thinkingmachines.ai/tinker/) · [tinker-cookbook](https://github.com/thinking-machines-lab/tinker-cookbook)
- **Inkling** (2026-07). [WIRED](https://www.wired.com/story/thinking-machines-lab-releases-its-first-model-inkling/)
- **Inkling-Small** (2026-07). [lab post](https://thinkingmachines.ai/news/inkling-small/)

Schulman's earlier scientific payload is still PPO + InstructGPT (see OpenAI section).

## 2024–26 — Second wave

The field is no longer three labs and a long tail. Most of these are product or world-model bets, not a new transformer paper.

- **Reflection AI** (Laskin, Antonoglou, ex-DeepMind). Agents / code systems (Asimov).
- **World Labs** (Fei-Fei Li). Spatial / world models. Prior: ImageNet + *NeuroAI* [arXiv:2210.08340](https://arxiv.org/abs/2210.08340).
- **AMI Labs** (LeCun, 2025). JEPA / world-model thesis. Prior: [arXiv:2301.08243](https://arxiv.org/abs/2301.08243).
- **Discovery Loop** (2026). Treat as a beat until they publish.
- **Meta Superintelligence Labs** (2025). Science still sits in the Llama reports until a real paper lands.

Cross-links: [DeepMind]({{ '/timelines/deepmind/' | relative_url }}), [SpaceX]({{ '/timelines/spacex/' | relative_url }}), [capability stack]({{ '/timelines/capability-stack/' | relative_url }}), [post-training]({{ '/timelines/post-training/' | relative_url }}), [agents]({{ '/timelines/agents/' | relative_url }}).
