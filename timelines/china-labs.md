---
layout: default
title: China labs
permalink: /timelines/china-labs/
---

# China labs

<p class="meta">Open weights as the export. Cheap reasoners as the shock. Listings as the cash-out.</p>

Not one actor. Platform labs (Alibaba Qwen, ByteDance Seed, Tencent Hunyuan, Baidu ERNIE) sit on a cloud or an app. Pure-plays (DeepSeek, Moonshot, Zhipu/Z.ai, MiniMax) sell weights, APIs, and a listing story. Methods that changed the global stack live also on [capability stack]({{ '/timelines/capability-stack/' | relative_url }}), [post-training]({{ '/timelines/post-training/' | relative_url }}), and [efficiency]({{ '/timelines/efficiency/' | relative_url }}).

## 2022-10 / 2023-09 — The bilingual open line

Before the R1 year, two families already ship weights: Tsinghua-spinout GLM and Alibaba's Qwen. The thesis is bilingual, open, and good enough to be a default base — not a ChatGPT clone with a press release.

- Zeng et al. *GLM-130B*. [arXiv:2210.02414](https://arxiv.org/abs/2210.02414)
- GLM team. *ChatGLM: A Family of Large Language Models from GLM-130B to GLM-4 All Tools*. [arXiv:2406.12793](https://arxiv.org/abs/2406.12793)
- Qwen team. *Qwen Technical Report*. [arXiv:2309.16609](https://arxiv.org/abs/2309.16609)

## 2024-05 — DeepSeek-V2 (MLA + sparse MoE)

Hangzhou quant shop High-Flyer. V2 is the architecture beat: Multi-head Latent Attention shrinks the KV cache; DeepSeekMoE keeps most weights idle. Training cost and decode cost both drop. Everything later (V3, R1) sits on this skeleton.

- DeepSeek-AI. *DeepSeek-V2*. [arXiv:2405.04434](https://arxiv.org/abs/2405.04434)
- Also on: [efficiency]({{ '/timelines/efficiency/' | relative_url }})

## 2024-09 / 2024-12 — Qwen2.5 as the download spine

Alibaba ships a size ladder, not one flagship. 0.5B through 72B, then hosted MoE. By 2026 Qwen is the most-downloaded open family — the Llama role, played from Hangzhou. The paper is a catalog as much as a result.

- Qwen team. *Qwen2.5 Technical Report*. [arXiv:2412.15115](https://arxiv.org/abs/2412.15115)
- Qwen2. [arXiv:2407.10671](https://arxiv.org/abs/2407.10671)

## 2024-12 — DeepSeek-V3

671B MoE, 37B active. Claimed mid-single-digit millions of dollars to train on H800-class parts. The cost number is the beat as much as the evals. Open weights, permissive license.

- DeepSeek-AI. *DeepSeek-V3*. [arXiv:2412.19437](https://arxiv.org/abs/2412.19437)

## 2025-01 — R1, and Moonshot's twin

DeepSeek publishes the reasoner recipe the West had kept as a system card: outcome RL (GRPO from DeepSeekMath), then distill into Qwen and Llama dense nets. Same month Moonshot's k1.5 shows long-context RL matching o1-class scores without a process-reward zoo.

After this, "a mid-cost Chinese base ⇒ a reasoner" is assumed. That is the efficiency and post-training shock, not a regional footnote.

- DeepSeek-AI. *DeepSeek-R1*. [arXiv:2501.12948](https://arxiv.org/abs/2501.12948)
- Shao et al. *DeepSeekMath* (GRPO). [arXiv:2402.03300](https://arxiv.org/abs/2402.03300)
- Kimi team. *Kimi k1.5: Scaling Reinforcement Learning with LLMs*. [arXiv:2501.12599](https://arxiv.org/abs/2501.12599)

## 2025-04 / 2025-05 — Platform labs publish recipes too

ByteDance Seed ships a thinking model with an RL paper, not only a Doubao product post. Alibaba's Qwen3 is a full family with a thinking/non-thinking switch and 119 languages. The platforms stop treating research as a side blog.

- ByteDance Seed. *Seed1.5-Thinking*. [arXiv:2504.13914](https://arxiv.org/abs/2504.13914)
- Qwen team. *Qwen3 Technical Report*. [arXiv:2505.09388](https://arxiv.org/abs/2505.09388)

## 2025-07 / 2025-08 — Agents and coding as the open scoreboard

Moonshot K2 (1T / 32B active) is sold as agentic intelligence — SWE-bench, tool use — not a chat lmsys slice. Zhipu GLM-4.5 is an open MoE aimed at the same jobs. The contest moves from MMLU to repos that pass tests.

- Kimi team. *Kimi K2: Open Agentic Intelligence*. [arXiv:2507.20534](https://arxiv.org/abs/2507.20534)
- GLM team. *GLM-4.5: An Open Mixture-of-Experts LLM*. [arXiv:2508.06471](https://arxiv.org/abs/2508.06471)

## 2025-12 — DeepSeek-V3.2

Efficiency plus agent scores on the V3 line. Cadence, not a new paradigm. [arXiv:2512.02556](https://arxiv.org/abs/2512.02556)

## 2026-01 — The tigers list

Z.ai (Zhipu, Tsinghua spinout, ticker 2513.HK) prices in Hong Kong on 8 Jan. MiniMax (0100.HK) prices the same week and doubles on debut. First time the China pure-plays have a public mark instead of a cap-table rumor. DeepSeek stays private; Moonshot prepares a later HK filing.

- [Reuters on the Zhipu debut week](https://www.reuters.com/world/asia-pacific/chinese-tech-companies-led-by-zhipu-ai-climb-hong-kong-debut-2026-01-08/)
- [Reuters: MiniMax doubles](https://www.reuters.com/world/asia-pacific/china-ai-firm-minimax-set-surge-hong-kong-debut-2026-01-09/)
- [WSJ on Zhipu's first day](https://www.wsj.com/tech/ai/chinese-ai-firm-zhipu-makes-lukewarm-trading-debut-1daf328a)

## 2026 — Capex and the closed twin

ByteDance discusses tens of billions in data-center and chip spend — a hyperscaler move, not a startup round. Doubao / Seed stays mostly closed; the open artifacts (UI-TARS, research papers) are the leak. Qwen keeps publishing a Max-tier checkpoint under a custom license. Treat later V4 / K2.6 / GLM-5.x version numbers as product cadence unless a methods paper lands.

Also on: [clouds]({{ '/timelines/clouds/' | relative_url }}) for who pays for the GPUs.

## What this page is not

A leaderboard. Chip-export rules and Huawei Ascend claims belong with silicon, not here, until a lab publishes a full training recipe on that stack. 01.AI / Yi and Baichuan were early open names; they are not the 2025–26 frontier.
