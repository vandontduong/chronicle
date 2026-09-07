---
layout: default
title: Data
permalink: /timelines/data/
---

# Data

<p class="meta">The stack assumes tokens. This page is where the tokens came from, how they were cleaned, and how they got poisoned.</p>

Scale laws and architectures: [capability stack]({{ '/timelines/capability-stack/' | relative_url }}). Distillation as an efficiency move: [efficiency]({{ '/timelines/efficiency/' | relative_url }}). Backdoors as a safety regime: [safety]({{ '/timelines/safety/' | relative_url }}).

## 2008– — Common Crawl

A nonprofit snapshot of the public web. Every later “web mix” is a filter on this firehose.

- [Common Crawl](https://commoncrawl.org/)

## 2019-10 — C4

Raffel et al. take a crawl snapshot, throw away what fails a language and blocklist filter, and call it Colossal Clean Crawled Corpus. T5 trains on it. Dodge later documents what the cleaning hid.

- Raffel et al. *Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer*. [arXiv:1910.10683](https://arxiv.org/abs/1910.10683)
- Dodge et al. *Documenting Large Webtext Corpora*. [arXiv:2104.08758](https://arxiv.org/abs/2104.08758)

## 2020-12 — The Pile

Twenty-two sources, 800 GB, academic and code weighted on purpose. The open mix that later Llama-class recipes are compared against.

- Gao et al. *The Pile: An 800GB Dataset of Diverse Text for Language Modeling*. [arXiv:2101.00027](https://arxiv.org/abs/2101.00027)

## 2021-07 — Dedup

Lee et al.: exact and near-duplicate spans are a large fraction of C4 and The Pile; models copy them back. Dedup becomes a training step, not a nicety.

- Lee et al. *Deduplicating Training Data Makes Language Models Better*. [arXiv:2107.06499](https://arxiv.org/abs/2107.06499)

## 2022-03 — Tokens, not just parameters

Hoffmann et al. (Chinchilla): compute-optimal means more data per parameter than GPT-3 used. Data collection, not just cluster size, is now the constraint.

- Hoffmann et al. *Training Compute-Optimal Large Language Models*. [arXiv:2203.15556](https://arxiv.org/abs/2203.15556)

## 2023-02 — Poisoning the crawl is cheap

Carlini et al.: split-view and frontrun attacks on URL lists. Tens of dollars to touch a slice of LAION or a Wikipedia snapshot. The web is not a trusted corpus.

- Carlini et al. *Poisoning Web-Scale Training Datasets is Practical*. [arXiv:2302.10149](https://arxiv.org/abs/2302.10149)

## 2023-05 / 2023-06 — Synthetic text that works

TinyStories: models well under a billion parameters learn coherent English from a generated children’s corpus. *Textbooks Are All You Need* (Phi-1): a curated plus synthetic code mix beats a crawl of the same size. Data *quality* is now a method.

- Eldan and Li. *TinyStories*. [arXiv:2305.07759](https://arxiv.org/abs/2305.07759)
- Gunasekar et al. *Textbooks Are All You Need*. [arXiv:2306.11644](https://arxiv.org/abs/2306.11644)

## 2023-06 / 2024-06 — Filter as the recipe

RefinedWeb: aggressive filtering of Common Crawl beats a curated multi-source mix at the same token count (Falcon). FineWeb: Hugging Face publishes the 2024 open default — traces, ablations, a reproducible filter stack. After this, “which crawl snapshot” is a less interesting question than “which filters.”

- Penedo et al. *The RefinedWeb Dataset for Falcon LLM*. [arXiv:2306.01116](https://arxiv.org/abs/2306.01116)
- Penedo et al. *The FineWeb Datasets*. [arXiv:2406.17557](https://arxiv.org/abs/2406.17557)

## 2025-10 — A few hundred docs

Anthropic / UK AISI / Turing: ~250 poisoned documents backdoor models from 600M to 13B. Count, not fraction of the mix. Pretrain hygiene is a security problem.

- [A small number of samples can poison LLMs of any size](https://www.anthropic.com/research/small-samples-poison)

## What this page is not

A catalogue of every SlimPajama / RedPajama / Dolma release. New mixes land here only if they change the recipe (open license, synthetic, a new filter stack, or a new attack).
