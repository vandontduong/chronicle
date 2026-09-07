---
layout: default
title: Efficiency
permalink: /timelines/efficiency/
---

# Compute efficiency

<p class="meta">Capability per flop. Every scaling shock has an efficiency twin.</p>

Each beat is a **ratio**: loss per dollar, tokens per second, or a reasoner squeezed out of a cheaper base. Hardware SKUs change the constant in front of the ratio; they live on [Nvidia]({{ '/timelines/nvidia/' | relative_url }}) and [Cerebras]({{ '/timelines/cerebras/' | relative_url }}). Who *pays* for the flops lives on [clouds]({{ '/timelines/clouds/' | relative_url }}). Prefill/decode *split across machines* lives on [disaggregated compute]({{ '/timelines/disaggregated-compute/' | relative_url }}). A longer window without more HBM lives on [memory]({{ '/timelines/memory/' | relative_url }}). How you *train* the student lives on [post-training]({{ '/timelines/post-training/' | relative_url }}). The DeepSeek cost shock also lives on [China labs]({{ '/timelines/china-labs/' | relative_url }}).

## 2015-03 / 2019-10 — Distill the teacher

Hinton, Vinyals, Dean: train a small net to match a large net's *soft* labels. Same task, fewer parameters. DistilBERT is the LM-era product — a 40% smaller BERT that keeps most of the GLUE score. The object is the ratio, not a new architecture.

- Hinton, Vinyals, Dean. *Distilling the Knowledge in a Neural Network*. [arXiv:1503.02531](https://arxiv.org/abs/1503.02531)
- Sanh et al. *DistilBERT*. [arXiv:1910.01108](https://arxiv.org/abs/1910.01108)

## 2020-01 / 2022-03 — How to spend the flops

Kaplan: loss is a power law in compute, data, and params — but the fit overweights params. Chinchilla: smaller model, more tokens, same compute, better loss. The training recipe for the next four years.

- Kaplan et al. *Scaling Laws for Neural Language Models*. [arXiv:2001.08361](https://arxiv.org/abs/2001.08361)
- Hoffmann et al. *Training Compute-Optimal Large Language Models*. [arXiv:2203.15556](https://arxiv.org/abs/2203.15556)

Also on: [capability stack]({{ '/timelines/capability-stack/' | relative_url }}), [data]({{ '/timelines/data/' | relative_url }}), [DeepMind]({{ '/timelines/deepmind/' | relative_url }}).

## 2021-01 — Sparse compute (MoE)

Most weights idle on any one token. Switch Transformer makes MoE the standard way to grow params without growing FLOPs 1:1. Grok-1 later ships a 314B MoE open checkpoint.

- Fedus et al. *Switch Transformer*. [arXiv:2101.03961](https://arxiv.org/abs/2101.03961)
- Lepikhin et al. *GShard*. [arXiv:2006.16668](https://arxiv.org/abs/2006.16668)
- [Grok-1 open release](https://x.ai/blog/grok-os)

## 2022-05 / 2023-07 / 2024-07 — Attention tax

FlashAttention tiles the attention matmuls so HBM stops dominating. Same math, large wall-clock win. v2 / v3 keep shaving the kernel. GQA cuts KV heads so decode bandwidth stops scaling with query heads.

- Dao et al. *FlashAttention*. [arXiv:2205.14135](https://arxiv.org/abs/2205.14135)
- Dao. *FlashAttention-2*. [arXiv:2307.08691](https://arxiv.org/abs/2307.08691)
- Shah et al. *FlashAttention-3*. [arXiv:2407.08608](https://arxiv.org/abs/2407.08608)
- Ainslie et al. *GQA: Training Generalized Multi-Query Transformer Models from Multi-Head Checkpoints*. [arXiv:2305.13245](https://arxiv.org/abs/2305.13245)

## 2022–23 — Cheaper bits, speculative tokens, paged KV

Quantization cuts memory and bandwidth. Speculative decoding uses a small draft model so the big model only verifies. PagedAttention treats the KV cache like virtual memory so a serving process stops wasting HBM on reserved slots.

- Frantar et al. *GPTQ*. [arXiv:2210.17323](https://arxiv.org/abs/2210.17323)
- Lin et al. *AWQ*. [arXiv:2306.00978](https://arxiv.org/abs/2306.00978)
- Leviathan et al. *Fast Inference from Transformers via Speculative Decoding*. [arXiv:2211.17192](https://arxiv.org/abs/2211.17192)
- Kwon et al. *Efficient Memory Management for Large Language Model Serving with PagedAttention*. [arXiv:2309.06180](https://arxiv.org/abs/2309.06180)

## 2024-08 / 2024-09 — Test-time as a budget

You can buy accuracy with decode tokens instead of pretrain FLOPs. Optimal allocation is its own scaling curve. o1 makes this a product; Snell et al. make it a paper.

- Snell et al. *Scaling LLM Test-Time Compute Optimally*. [arXiv:2408.03314](https://arxiv.org/abs/2408.03314)
- [Learning to reason with LLMs](https://openai.com/index/learning-to-reason-with-llms/)
- OpenAI. *o1 System Card*. [arXiv:2412.16720](https://arxiv.org/abs/2412.16720)

## 2024-12 / 2025-01 — Training-cost shock, then the student

DeepSeek-V3 (MLA, MoE, cheap pretrain claims) then R1 (outcome RL → reasoner). The second half of the paper is the 2015 move at frontier scale: distill R1 into Qwen and Llama *dense* nets so a 32B/70B student carries the reasoning. After this, “mid-cost base ⇒ open reasoner” is assumed. Recipe: [post-training]({{ '/timelines/post-training/' | relative_url }}). Who shipped the students: [China labs]({{ '/timelines/china-labs/' | relative_url }}).

- DeepSeek-AI. *DeepSeek-V3*. [arXiv:2412.19437](https://arxiv.org/abs/2412.19437)
- DeepSeek-AI. *DeepSeek-R1*. [arXiv:2501.12948](https://arxiv.org/abs/2501.12948)

## What this page is not

Cluster announcements and GPU SKUs. Those change the constant in front of the ratio; they are not the ratio. Splitting prefill and decode onto different machines is [disaggregated compute]({{ '/timelines/disaggregated-compute/' | relative_url }}). Infini-attention and Titans are [memory]({{ '/timelines/memory/' | relative_url }}). Synthetic *corpora* (Phi, TinyStories) are [data]({{ '/timelines/data/' | relative_url }}) — generated text, not a teacher-student pair.
