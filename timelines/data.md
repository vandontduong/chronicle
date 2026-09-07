---
layout: default
title: Data
permalink: /timelines/data/
---

# Data

<p class="meta">Where the tokens came from, how they were cleaned, and how they got poisoned.</p>

This page is the **text firehose** and the two public mixes that escaped it: permissively licensed **code**, and CLIP-filtered **image–text pairs**. A modality earns a beat when labs started training on it as a first-class mix, not when a dataset exists.

Robot trajectories: [robotics]({{ '/timelines/robotics/' | relative_url }}). Protein sequences and structures: [techbio]({{ '/timelines/techbio/' | relative_url }}). Preference pairs and distill traces: [post-training]({{ '/timelines/post-training/' | relative_url }}). Scale laws: [capability stack]({{ '/timelines/capability-stack/' | relative_url }}). Backdoors as a release regime: [safety]({{ '/timelines/safety/' | relative_url }}). Project Panama the firm: [Anthropic]({{ '/timelines/anthropic/' | relative_url }}).

## 2008– — Common Crawl

A nonprofit snapshot of the public web. Every later “web mix” is a filter on this firehose.

- [Common Crawl](https://commoncrawl.org/)

## 2019-10 — C4

Raffel et al. take a crawl snapshot, throw away what fails a language and blocklist filter, and call it Colossal Clean Crawled Corpus. T5 trains on it. Dodge later documents what the cleaning hid.

- Raffel et al. *Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer*. [arXiv:1910.10683](https://arxiv.org/abs/1910.10683)
- Dodge et al. *Documenting Large Webtext Corpora*. [arXiv:2104.08758](https://arxiv.org/abs/2104.08758)

## 2020-12 — The Pile

Twenty-two sources, 800 GB. Academic prose and code weighted on purpose. The open mix later Llama-class recipes are compared against. Code here is still a *slice of a text mix*, not its own corpus.

- Gao et al. *The Pile: An 800GB Dataset of Diverse Text for Language Modeling*. [arXiv:2101.00027](https://arxiv.org/abs/2101.00027)

## 2021-07 — Dedup

Lee et al.: exact and near-duplicate spans are a large fraction of C4 and The Pile; models copy them back. Dedup becomes a training step, not a nicety.

- Lee et al. *Deduplicating Training Data Makes Language Models Better*. [arXiv:2107.06499](https://arxiv.org/abs/2107.06499)

## 2021–24 — Books, two pipelines

Long-form text that is not a web snapshot. Claude's lab used two acquisition methods; a court later split them.

**Pirate libraries.** 2021: ~5 million files from Library Genesis. 2022: ~2 million more from Pirate Library Mirror. Judge Alsup (*Bartz v. Anthropic*, 24-cv-05417): downloading and keeping those copies was not fair use.

**Print, then a mill.** 2024 Project Panama — internal line: “destructively scan all the books in the world.” Tom Turvey (ex-Google Books) buys used print in bulk. Vendors cut the spines, scan the pages, discard the paper. Alsup: *that* pipeline is fair use. Anthropic says less-common / reference copies, not antiquarian collectibles. Headlines said “rare books.” The record says millions of print copies destroyed to make a searchable library kept “forever.”

- Alsup, Order on Fair Use, 23 Jun 2025. [Washington Post filing PDF](https://www.washingtonpost.com/documents/cf8f6674-7b14-4b7d-ab6f-bbd9ad45963f.pdf)
- [Washington Post on Panama](https://www.washingtonpost.com/technology/2026/01/27/anthropic-ai-scan-destroy-books/)
- [Snopes on “rare” vs less-common](https://www.snopes.com/fact-check/ai-companies-destroying-rare-books/)

## 2022-03 — Tokens, not just parameters

Hoffmann et al. (Chinchilla): compute-optimal means more data per parameter than GPT-3 used. Collecting tokens, not just buying a cluster, is now the constraint.

- Hoffmann et al. *Training Compute-Optimal Large Language Models*. [arXiv:2203.15556](https://arxiv.org/abs/2203.15556)

## 2022-10 / 2022-11 — Two public mixes that are not prose

**Image–text.** LAION-5B: 5.85 billion CLIP-filtered pairs scraped from the web. Open enough to train a Stable Diffusion. The crawl problem now has pixels attached. Carlini later poisons this class of URL list.

**Code.** The Stack: 3.1 TB of *permissively licensed* source in 30 languages, with an opt-out. StarCoder (2023) is the model that proved the mix; Stack v2 (2024) pulls Software Heritage. License and governance are the recipe change, not “more GitHub.”

- Schuhmann et al. *LAION-5B*. [arXiv:2210.08402](https://arxiv.org/abs/2210.08402)
- Kocetkov et al. *The Stack*. [arXiv:2211.15533](https://arxiv.org/abs/2211.15533)
- Li et al. *StarCoder*. [arXiv:2305.06161](https://arxiv.org/abs/2305.06161)
- Lozhkov et al. *StarCoder 2 and The Stack v2*. [arXiv:2402.19173](https://arxiv.org/abs/2402.19173)

## 2023-02 — Poisoning the crawl is cheap

Carlini et al.: split-view and frontrun attacks on URL lists. Tens of dollars to touch a slice of LAION or a Wikipedia snapshot. The web is not a trusted corpus.

- Carlini et al. *Poisoning Web-Scale Training Datasets is Practical*. [arXiv:2302.10149](https://arxiv.org/abs/2302.10149)

## 2023-05 / 2023-06 — Synthetic text that works

TinyStories: models well under a billion parameters learn coherent English from a generated children’s corpus. *Textbooks Are All You Need* (Phi-1): a curated plus synthetic *code* mix beats a crawl of the same size. Quality of the mix is now a method. Teacher-student distillation is a different object — [efficiency]({{ '/timelines/efficiency/' | relative_url }}) / [post-training]({{ '/timelines/post-training/' | relative_url }}).

- Eldan and Li. *TinyStories*. [arXiv:2305.07759](https://arxiv.org/abs/2305.07759)
- Gunasekar et al. *Textbooks Are All You Need*. [arXiv:2306.11644](https://arxiv.org/abs/2306.11644)

## 2023-06 / 2024-06 — Filter as the recipe

RefinedWeb: aggressive filtering of Common Crawl beats a curated multi-source mix at the same token count (Falcon). FineWeb: Hugging Face publishes the 2024 open default — traces, ablations, a reproducible filter stack. After this, “which crawl snapshot” matters less than “which filters.”

- Penedo et al. *The RefinedWeb Dataset for Falcon LLM*. [arXiv:2306.01116](https://arxiv.org/abs/2306.01116)
- Penedo et al. *The FineWeb Datasets*. [arXiv:2406.17557](https://arxiv.org/abs/2406.17557)

## 2025-09 / 2026-07 — The invoice for the pirate copies

*Bartz* settles for **$1.5B** (~$3k per listed work, ~482k books). Final approval July 2026. The money and the order to destroy LibGen / PiLiMi files are about the *torrent* pipeline. The destructive scans stayed fair use. Largest US copyright class recovery to date. Outputs and future training are not released.

- [NYT on the September 2025 deal](https://www.nytimes.com/2025/09/05/technology/anthropic-settlement-copyright-ai.html)
- [AP on final approval](https://apnews.com/article/ai-anthropic-copyright-settlement-claude-books-bartz-74b140444023898aeba8579b6e9f0d63)
- Firm page: [Anthropic]({{ '/timelines/anthropic/' | relative_url }})

## 2025-10 — A few hundred docs

Anthropic / UK AISI / Turing: ~250 poisoned documents backdoor models from 600M to 13B. Count, not fraction of the mix. Pretrain hygiene is a security problem.

- [A small number of samples can poison LLMs of any size](https://www.anthropic.com/research/small-samples-poison)

## What this page is not

A catalogue of SlimPajama / RedPajama / Dolma. ImageNet and MMLU items are [evals]({{ '/timelines/evals/' | relative_url }}). Open X-Embodiment is [robotics]({{ '/timelines/robotics/' | relative_url }}). UniRef, PDB, AlphaFold DB are [techbio]({{ '/timelines/techbio/' | relative_url }}). HH-RLHF and other preference sets are [post-training]({{ '/timelines/post-training/' | relative_url }}). Whisper-scale speech and Sora-scale video stay off until a lab publishes the mix, not just the model.
