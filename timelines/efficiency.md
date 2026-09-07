---
layout: default
title: Efficiency
permalink: /timelines/efficiency/
---

# Compute efficiency

<p class="meta">Capability per flop · every scaling shock has an efficiency twin</p>

Each beat is a ratio: loss per dollar, tokens per second, or a reasoner squeezed out of a cheaper base. Not a hardware catalog.

## 2020-01 / 2022-03 — How to spend the flops

Kaplan: loss is a power law in compute, data, and params — but the fit overweights params. Chinchilla: smaller model, more tokens, same compute, better loss. The training recipe for the next four years.

- Kaplan et al. *Scaling Laws for Neural Language Models*. [arXiv:2001.08361](https://arxiv.org/abs/2001.08361) · [alphaXiv](https://www.alphaxiv.org/abs/2001.08361)
- Hoffmann et al. *Training Compute-Optimal Large Language Models*. [arXiv:2203.15556](https://arxiv.org/abs/2203.15556) · [alphaXiv](https://www.alphaxiv.org/abs/2203.15556)

Also on: [capability stack]({{ '/timelines/capability-stack/' | relative_url }}), [DeepMind]({{ '/timelines/deepmind/' | relative_url }}).

## 2021-01 — Sparse compute (MoE)

Most weights idle on any one token. Switch Transformer makes MoE the standard way to grow params without growing FLOPs 1:1. Grok-1 later ships a 314B MoE open checkpoint.

- Fedus et al. *Switch Transformer*. [arXiv:2101.03961](https://arxiv.org/abs/2101.03961) · [alphaXiv](https://www.alphaxiv.org/abs/2101.03961)
- Lepikhin et al. *GShard*. [arXiv:2006.16668](https://arxiv.org/abs/2006.16668)
- [Grok-1 open release](https://x.ai/blog/grok-os)

## 2022-05 / 2023-07 — Attention tax

FlashAttention tiles the attention matmuls so HBM stops dominating. Same math, large wall-clock win. v2 / v3 keep shaving the kernel.

- Dao et al. *FlashAttention*. [arXiv:2205.14135](https://arxiv.org/abs/2205.14135) · [alphaXiv](https://www.alphaxiv.org/abs/2205.14135)
- Dao. *FlashAttention-2*. [arXiv:2307.08691](https://arxiv.org/abs/2307.08691)

## 2022–23 — Cheaper bits and speculative tokens

Quantization cuts memory and bandwidth. Speculative decoding uses a small draft model so the big model only verifies. Serving, not training.

- Frantar et al. *GPTQ*. [arXiv:2210.17323](https://arxiv.org/abs/2210.17323)
- Lin et al. *AWQ*. [arXiv:2306.00978](https://arxiv.org/abs/2306.00978)
- Leviathan et al. *Fast Inference from Transformers via Speculative Decoding*. [arXiv:2211.17192](https://arxiv.org/abs/2211.17192)

## 2024-08 / 2024-09 — Test-time as a budget

You can buy accuracy with decode tokens instead of pretrain FLOPs. Optimal allocation is its own scaling curve. o1 makes this a product; Snell et al. make it a paper.

- Snell et al. *Scaling LLM Test-Time Compute Optimally*. [arXiv:2408.03314](https://arxiv.org/abs/2408.03314) · [alphaXiv](https://www.alphaxiv.org/abs/2408.03314)
- [Learning to reason with LLMs](https://openai.com/index/learning-to-reason-with-llms/)
- OpenAI. *o1 System Card*. [arXiv:2412.16720](https://arxiv.org/abs/2412.16720)

## 2024-12 / 2025-01 — Training-cost shock

DeepSeek-V3 (MLA, MoE, cheap pretrain claims) then R1 (outcome RL → reasoner). The efficiency claim is as important as the benchmark claim: a reasoner from a mid-cost base.

- DeepSeek-AI. *DeepSeek-V3*. [arXiv:2412.19437](https://arxiv.org/abs/2412.19437) · [alphaXiv](https://www.alphaxiv.org/abs/2412.19437)
- DeepSeek-AI. *DeepSeek-R1*. [arXiv:2501.12948](https://arxiv.org/abs/2501.12948) · [alphaXiv](https://www.alphaxiv.org/abs/2501.12948)

Also on: [post-training]({{ '/timelines/post-training/' | relative_url }}), [capability stack]({{ '/timelines/capability-stack/' | relative_url }}).

## What this page is not

Cluster announcements and GPU SKUs. Those change the constant in front of the ratio; they are not the ratio.
