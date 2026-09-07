---
layout: default
title: Agents
permalink: /timelines/agents/
---

# Agents

<p class="meta">From tool calls to systems that do work.</p>

An agent is a model plus a loop that is allowed to touch the world more than once. This page is that loop. The weights that sit inside it live on [capability stack]({{ '/timelines/capability-stack/' | relative_url }}). The scoreboard (SWE-bench, LiveCodeBench) lives on [evals]({{ '/timelines/evals/' | relative_url }}). Search over agent *designs* lives on [RSI]({{ '/timelines/rsi/' | relative_url }}). Learned simulators live on [world models]({{ '/timelines/world-models/' | relative_url }}).

Reliability, not a new architecture, is the scarce object after 2024.

## 2022-10 — ReAct

Interleave a reasoning trace with an environment action. The unit stops being a single completion. Everything later (tools, SWE-bench, computer use) is this pattern with a better environment.

- Yao et al. *ReAct: Synergizing Reasoning and Acting in Language Models*. [arXiv:2210.03629](https://arxiv.org/abs/2210.03629)

## 2023-02 — Toolformer

The model learns *when* to call tools from self-supervised traces. Tools become part of training, not just a system prompt.

- Schick et al. *Toolformer*. [arXiv:2302.04761](https://arxiv.org/abs/2302.04761)

## 2023 — Loops, then a scoreboard for tools

AutoGPT / BabyAGI put an LLM in a while-loop. Fragile. Demand signal, not a method. Reflexion and Tree of Thoughts add self-critique and search over thoughts. Voyager shows a skill library in Minecraft. Gorilla is the unglamorous beat: call *real* APIs without hallucinating the schema.

- [AutoGPT](https://github.com/Significant-Gravitas/AutoGPT)
- Shinn et al. *Reflexion*. [arXiv:2303.11366](https://arxiv.org/abs/2303.11366)
- Yao et al. *Tree of Thoughts*. [arXiv:2305.10601](https://arxiv.org/abs/2305.10601)
- Wang et al. *Voyager*. [arXiv:2305.16291](https://arxiv.org/abs/2305.16291)
- Patil et al. *Gorilla*. [arXiv:2305.15334](https://arxiv.org/abs/2305.15334)

## 2024 — Software-engineering agents

SWE-bench turns GitHub issues into an eval. SWE-agent is the academic loop (edit, run tests, repeat). Devin is the demo that created a market. Claude Code and Codex are the products people actually pay for. Cursor is the distribution that SpaceX later bought — see [SpaceX]({{ '/timelines/spacex/' | relative_url }}).

- Jimenez et al. *SWE-bench*. [arXiv:2310.06770](https://arxiv.org/abs/2310.06770)
- Yang et al. *SWE-agent*. [arXiv:2405.15793](https://arxiv.org/abs/2405.15793)

The scoreboard moved faster than the papers. Treat leaderboard jumps as product beats unless a method paper lands.

## 2024-10 / 2025 — Computer use

The environment is a desktop. Anthropic ships computer use with Claude 3.5; OpenAI ships Operator-class products. Capability is bursty. The question is hours of reliable work, not a screenshot demo.

- Anthropic. [Introducing computer use](https://www.anthropic.com/news/3-5-models-and-computer-use) (Oct 2024)
- Earlier generalist bet: Reed et al. *Gato*. [arXiv:2205.06175](https://arxiv.org/abs/2205.06175) — also on [DeepMind]({{ '/timelines/deepmind/' | relative_url }})

## 2024-11 — A socket, not a better net

Anthropic's Model Context Protocol is an interface standard for tools and data. Unsexy. It is how agents stop being one-off harnesses.

- [Model Context Protocol](https://www.anthropic.com/news/model-context-protocol)

## 2026-08 — Grok Bot

SpaceXAI ships agents on the Cursor + Grok bundle after the acquisition closes. Product surface of a lab merger, not a new paper.

- [The Next Web](https://thenextweb.com/news/spacexai-grok-bot-ai-agents-cursor)
- Company object: [SpaceX]({{ '/timelines/spacex/' | relative_url }})

## What this page is not

Reasoning models (o1, R1) are [post-training]({{ '/timelines/post-training/' | relative_url }}). Agents that rewrite their own code are [RSI]({{ '/timelines/rsi/' | relative_url }}). Genie / Sora as environments are [world models]({{ '/timelines/world-models/' | relative_url }}).
