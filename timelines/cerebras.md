---
layout: default
title: Cerebras
permalink: /timelines/cerebras/
---

# Cerebras

<p class="meta">One wafer, on-chip SRAM · the bet that decode speed is the product</p>

Nvidia sells FLOPs and fabric. Cerebras sells *tokens per second per user* by refusing the reticle limit. Few papers; blogs and S-1s are the primary sources. Cerebras does not buy companies. Other people try to buy Cerebras and fail.

## 2016 — Founded

Andrew Feldman, Sean Lie, Lauterbach, Fricker, James. After SeaMicro → AMD. Thesis: cut the wafer into one chip instead of hundreds of GPUs that then need a network.

- Company: [cerebras.ai](https://www.cerebras.ai/)

## 2017 — OpenAI / Tesla look at a purchase

Sutskever emails (later exhibits in Musk v. OpenAI) talk diligence and “negotiate merger terms with Cerebras.” He argues *not* to buy it through Tesla — shareholder duty vs OpenAI’s charter. Nothing closes. Eight years later OpenAI buys *capacity and warrants*, not the company.

- [TechCrunch on the 2017 emails](https://techcrunch.com/2024/11/15/openai-at-one-point-considered-acquiring-ai-chip-startup-cerebras/)

## 2019 — WSE-1

First commercial wafer-scale processor. The architectural claim is set: SRAM next to every core, no off-chip HBM hop for weights that fit.

- Early system writeups and ISSCC/Hot Chips talks from this generation; later numbers live on the WSE-3 pages.

## 2021 — WSE-2 / CS-2

Bigger SRAM, more cores. Still mostly a training/HPC story (national labs, pharma). The market has not yet priced *decode latency*.

## 2024-03 / 2024-08 — WSE-3, CS-3, Inference API

Third wafer on TSMC N5: ~900k cores, 44 GB on-chip SRAM, claimed ~21 PB/s on-chip bandwidth. MemoryX (weight streaming) + SwarmX (cluster fabric) so models larger than one wafer still run. Then the product flip: **Cerebras Inference** as an API, Llama 3.1 8B/70B posted at thousands of tok/s vs GPU clouds.

- [Cerebras AI Day / CS-3 architecture](https://www.youtube.com/watch?v=re4QqXPmfgs)
- [Introducing Cerebras Inference](https://cerebras.ai/blog/introducing-cerebras-inference-ai-at-instant-speed/) (27 Aug 2024)
- Zhang et al. *Benchmarking LLMs on the Cerebras WSE*. [arXiv:2409.00287](https://arxiv.org/abs/2409.00287)

## 2024 — G42 concentration, first S-1 pulled

Abu Dhabi's G42 is ~85–87% of 2024 revenue and an investor. CFIUS reviews the stake. S-1 goes stale; IPO waits. The scientific work continues; the company risk is geopolitical, not architectural. This is a minority investment, not an acquisition of Cerebras.

- [NYT on the later filing](https://www.nytimes.com/2026/04/17/technology/cerebras-public-offering-ai.html)
- [S-1 customer-mix recap](https://thestartupproject.io/blog/cerebras-s1-breakdown)

## 2025-01 — Fast reasoning

DeepSeek-R1 distill (Llama-70B) on the inference API. The pitch becomes: long CoT is only usable if decode is cheap and fast. Ties this page to [post-training]({{ '/timelines/post-training/' | relative_url }}) and [efficiency]({{ '/timelines/efficiency/' | relative_url }}).

- [Cerebras: DeepSeek R1 Llama-70B inference](https://www.cerebras.ai/blog/cerebras-launches-worlds-fastest-deepseek-r1-llama-70b-inference)

## 2025-12 / 2026-01 — OpenAI inference offtake (buy the tokens, not the firm)

Master relationship agreement: OpenAI commits to **750 MW** of Cerebras inference, valued by Cerebras at **>$20B**, option for another 1.25 GW through 2030. OpenAI advances ~$1B working capital with **warrants** on tens of millions of shares — a path to a stake without owning the wafer. That is the 2017 idea, inverted.

Numbers in press wander between “$10B+” (Jan announcement) and “>$20B” (S-1 / earnings). Use the S-1 figure.

- [NYT, 14 Jan 2026](https://www.nytimes.com/2026/01/14/technology/openai-cerebras-chips-deal.html)
- [VentureBeat IPO + $20B deal](https://venturebeat.com/technology/cerebras-stock-nearly-doubles-on-day-one-as-ai-chipmaker-hits-100-billion-what-it-means-for-ai-infrastructure)
- [Motley Fool on the $25.4B backlog](https://www.fool.com/investing/2026/09/05/cerebras-has-a-usd25-4-billion-backlog-and-one-openai-agreement-is-behind-much-of-it/)
- Warrants / loan: [TechCrunch IPO preview](https://techcrunch.com/2026/05/04/openais-cozy-partner-cerebras-is-on-track-for-a-blockbuster-ipo/)

## 2025–26 — Nvidia asks; Cerebras says no

Reuters: as OpenAI shops SRAM inference, Nvidia approaches Cerebras and Groq about a purchase. Cerebras declines and takes the OpenAI offtake. Groq later becomes Nvidia’s license + hire (see [Nvidia]({{ '/timelines/nvidia/' | relative_url }})).

- [Reuters, 4 Feb 2026](https://www.reuters.com/business/ai-chip-maker-cerebras-systems-raises-1-billion-late-stage-funding-2026-02-04/)

## 2026-03 — AWS: prefill on Trainium, decode on CS-3

Disaggregated inference as a cloud product. Amazon Bedrock path. Cerebras's blog frames this as the GPU being “split in half.”

- [The GPU Is Being Split in Half](https://www.cerebras.ai/blog/disaggregated-inference)

## 2026-04 / 2026-05 — Arm / SoftBank approach, then IPO

Bloomberg: Arm and SoftBank make a pre-IPO approach. Rebuffed. Cerebras prices instead. Day-one pop; concentration risk now split between UAE (G42 + MBZUAI still most of *historical* revenue) and OpenAI (most of *backlog*).

- [Bloomberg Law](https://news.bloomberglaw.com/mergers-and-acquisitions/arm-softbank-said-to-have-tried-to-buy-cerebras-before-ipo-1)
- [NYT filing story](https://www.nytimes.com/2026/04/17/technology/cerebras-public-offering-ai.html)
- [VentureBeat day one](https://venturebeat.com/technology/cerebras-stock-nearly-doubles-on-day-one-as-ai-chipmaker-hits-100-billion-what-it-means-for-ai-infrastructure)

## 2026-08 — CS-4 / WSE-3 Turbo, rack scale

Clocked-up wafer plus a three-wafer rack that wants to be one scale-up domain. Hot Chips 2026. Frontier decode (GPT-5.6 Sol class) as the demo, not training.

- [Introducing Cerebras CS-4](https://www.cerebras.ai/blog) (18 Aug 2026)
- [ServeTheHome, Hot Chips 2026](https://www.servethehome.com/cerebras-talks-going-rack-scale-with-their-wses-at-hot-chips-2026/)

## Software / papers worth keeping

- He et al. *WaferLLM* (OSDI 2025) — wafer-scale inference system, not a Cerebras paper but the independent systems result. [USENIX](https://www.usenix.org/conference/osdi25/presentation/he)
- Cerebras MoE-on-wafer notes: [MoE at Scale](https://www.cerebras.ai/blog/moe-guide-scale)
- Weight streaming is the training trick when params exceed SRAM; decode is the product.

## Deal list (short)

| Year | Counterparty | What |
|---|---|---|
| 2017 | OpenAI / Tesla | Merger talk. Dead. |
| 2021–25 | G42 / MBZUAI | Anchor revenue + minority equity; CFIUS. Not a takeout. |
| 2025-12 | OpenAI | >$20B / 750 MW inference; loan + warrants |
| 2025–26 | Nvidia | Purchase approach. Declined. |
| 2026-03 | AWS | Trainium prefill + CS-3 decode on Bedrock |
| 2026-04 | Arm / SoftBank | Pre-IPO approach. Rebuffed. |
| 2026 | Nordic / other colo | Capacity to feed the OpenAI MW |

No Mellanox-class acquisition *by* Cerebras. Contrast [Nvidia]({{ '/timelines/nvidia/' | relative_url }}).

Also on: [efficiency]({{ '/timelines/efficiency/' | relative_url }}), [nvidia]({{ '/timelines/nvidia/' | relative_url }}), [capability stack]({{ '/timelines/capability-stack/' | relative_url }}).
