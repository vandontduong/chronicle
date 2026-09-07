---
layout: default
title: Agents
permalink: /timelines/agents/
---

# Agents

<p class="meta">From tool calls to systems that do work</p>

## 2022-10 — ReAct

Interleave reasoning traces with environment actions. The unit stops being a single completion.

- Yao et al. *ReAct: Synergizing Reasoning and Acting in Language Models*. [arXiv:2210.03629](https://arxiv.org/abs/2210.03629) · [alphaXiv](https://www.alphaxiv.org/abs/2210.03629)

## 2023-02 — Toolformer

The model learns *when* to call tools (calculator, search, calendar) from self-supervised traces. Tools become part of pretraining, not just prompting.

- Schick et al. *Toolformer*. [arXiv:2302.04761](https://arxiv.org/abs/2302.04761) · [alphaXiv](https://www.alphaxiv.org/abs/2302.04761)

## 2023 — Loops and hype

AutoGPT / BabyAGI: an LLM in a while-loop with memory. Fragile. Shows demand; does not show reliability.

- [AutoGPT](https://github.com/Significant-Gravitas/AutoGPT)
- Shinn et al. *Reflexion*. [arXiv:2303.11366](https://arxiv.org/abs/2303.11366)
- Yao et al. *Tree of Thoughts*. [arXiv:2305.10601](https://arxiv.org/abs/2305.10601)
- Wang et al. *Voyager* (Minecraft lifelong learning). [arXiv:2305.16291](https://arxiv.org/abs/2305.16291)

## 2023-05 — Tool APIs as a research object

Calling real APIs correctly, not toy tools.

- Patil et al. *Gorilla: Large Language Model Connected with Massive APIs*. [arXiv:2305.15334](https://arxiv.org/abs/2305.15334)

## 2024 — Software-engineering agents

SWE-bench becomes the scoreboard. Agents that edit repos and pass tests — first agent product people pay for.

- Jimenez et al. *SWE-bench*. [arXiv:2310.06770](https://arxiv.org/abs/2310.06770)
- Yang et al. *SWE-agent*. [arXiv:2405.15793](https://arxiv.org/abs/2405.15793) · [alphaXiv](https://www.alphaxiv.org/abs/2405.15793)
- Cognition *Devin* (product, 2024). No flagship paper; the demo set the market.
- Anthropic *Claude Code* / OpenAI *Codex* — productized versions of the same loop.

## 2024-10 / 2025 — Computer use

Models operate browsers and desktops. Capability is uneven; the question is long-horizon reliability, not screenshots.

- Anthropic. [Introducing computer use](https://www.anthropic.com/news/3-5-models-and-computer-use) (Oct 2024)
- OpenAI. Operator / computer-use in the o/GPT line — product posts, thin papers.
- DeepMind Gato as an earlier generalist-agent bet: [arXiv:2205.06175](https://arxiv.org/abs/2205.06175)

Also on: [capability stack]({{ '/timelines/capability-stack/' | relative_url }}), [DeepMind]({{ '/timelines/deepmind/' | relative_url }}).
