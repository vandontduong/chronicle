---
layout: default
title: Memory
permalink: /timelines/memory/
---

# Memory

<p class="meta">The context window became an asset class. This page is how the net holds state past a few thousand tokens.</p>

Architecture and scale live on [capability stack]({{ '/timelines/capability-stack/' | relative_url }}). RoPE and GQA as *ratios* live on [efficiency]({{ '/timelines/efficiency/' | relative_url }}). KV paging across machines lives on [disaggregated compute]({{ '/timelines/disaggregated-compute/' | relative_url }}). Bytes on rust and NAND live on [storage]({{ '/timelines/storage/' | relative_url }}). The DRAM cube next to the GPU lives on [HBM]({{ '/timelines/hbm/' | relative_url }}). This page is the window itself — recurrence, retrieval, compression, then a million-token product.

## 2019-01 — Segment recurrence

Transformer-XL reuses hidden states from the previous segment instead of wiping the cache at every chunk. Context is no longer one training cut.

- Dai et al. *Transformer-XL: Attentive Language Models Beyond a Fixed-Length Context*. [arXiv:1901.02860](https://arxiv.org/abs/1901.02860)

## 2019-11 — Compress the past

Compressive Transformer keeps a second cache of *compressed* old activations. The window grows without keeping every key.

- Rae et al. *Compressive Transformers for Long-Range Sequence Modelling*. [arXiv:1911.05507](https://arxiv.org/abs/1911.05507)

## 2022-03 — A kNN over old keys

Memorizing Transformers: approximate nearest-neighbor lookup into a non-differentiable store of recent (key, value) pairs. Perplexity keeps falling as the store grows to hundreds of thousands of tokens. Memory as an index, not a longer softmax.

- Wu et al. *Memorizing Transformers*. [arXiv:2203.08913](https://arxiv.org/abs/2203.08913)

## 2023-10 — Context parallel

Ring Attention shards the sequence across devices so the *effective* window is the cluster, not the chip. Serving trick that made million-token demos cheap enough to ship. Also on [disaggregated compute]({{ '/timelines/disaggregated-compute/' | relative_url }}).

- Liu, Zaharia, Abbeel. *Ring Attention with Blockwise Transformers*. [arXiv:2310.01889](https://arxiv.org/abs/2310.01889)

## 2024-02 — A million tokens as a product

Gemini 1.5 reports a 1M-token window that actually retrieves. The window is now a SKU labs quote next to parameter count. Recipe unpublished; the eval is the claim.

- *Gemini 1.5*. [arXiv:2403.05530](https://arxiv.org/abs/2403.05530)

## 2024-04 — Bounded memory, unbounded stream

Infini-attention: local softmax plus a compressive linear memory in the same block. Passkey retrieval at 1M with a fixed state. The opposite bet from “just buy more HBM.”

- Munkhdalai, Faruqui, Gopal. *Leave No Context Behind*. [arXiv:2404.07143](https://arxiv.org/abs/2404.07143)

## 2025-01 — Memorize at test time

Titans: a neural long-term memory that updates while the model runs, plus attention over the current window. Needle tasks past 2M. Test-time memorization, not a bigger KV cache.

- Behrouz, Zhong, Mirrokni. *Titans: Learning to Memorize at Test Time*. [arXiv:2501.00663](https://arxiv.org/abs/2501.00663)

## What this page is not

A list of every long-context eval (Needle, RULER). Those land on [evals]({{ '/timelines/evals/' | relative_url }}) only if labs train against them. Linear RNNs and Mamba as *architecture alternatives* stay a pointer from [capability stack]({{ '/timelines/capability-stack/' | relative_url }}) until they change what ships. Exos / Ultrastar SKUs are [storage]({{ '/timelines/storage/' | relative_url }}). HBM stacks and vendor quals are [HBM]({{ '/timelines/hbm/' | relative_url }}).
