---
layout: default
title: SpaceX
permalink: /timelines/spacex/
---

# SpaceX

<p class="meta">Rockets paid for the plants. Then the plants rented GPUs. Then the ticker bought a coding lab.</p>

This page is the company object. Deals that change *who trains* also sit on [lab fission]({{ '/timelines/lab-fission/' | relative_url }}) and [clouds]({{ '/timelines/clouds/' | relative_url }}). There is almost no SpaceX arXiv spine — the record is memos, S-1 language, and lab blogs.

## 2002–19 — The franchise

Founded 2002. Falcon 9 first flight 2010; first orbital booster landing 2015. Starlink starts deploying 2019. By the mid-2020s Starlink is most of *revenue*; launch is most of *mass to orbit*. That cash-flow and the Starship stack are what later pay for Colossus and get cited as the reason orbital compute is even discussable.

No paper beat. The scientific residue is engineering blogs and FAA/FCC filings, not NeurIPS.

## 2023-07 — xAI as a separate lab

Musk incorporates the anti-OpenAI lab after leaving the OpenAI board years earlier. Thesis: a truth-seeking model, trained outside the Bay safety stack. Colossus in Memphis is built for Grok, not for Starlink.

- [xAI announcement](https://x.ai/blog/about)
- Also on: [lab fission]({{ '/timelines/lab-fission/' | relative_url }})

## 2024-03 — Grok-1 weights

314B MoE, 25% active, Apache-2. First large open weight from the Musk stack. Not a capability frontier paper. It is a distribution beat: the lab will sometimes ship weights.

- [xAI: open release](https://x.ai/blog/grok-os)
- [Weights on Hugging Face](https://huggingface.co/xai-org/grok-1)

## 2025-03 — xAI acquires X

All-stock. Musk: xAI at $80B, X at $33B ($45B EV less $12B debt). Distribution (the feed) and the model sit in one holding company. Training data and product surface are no longer a commercial negotiation.

- [TechCrunch](https://techcrunch.com/2025/03/29/elon-musk-says-xai-acquired-x/)

## 2024–26 — Colossus 1 and 2

Memphis / Southaven training campus. SpaceX S-1 later cites ~**1 GW** nameplate across the pair, turbines then a permanent plant. Built for Grok; spare capacity becomes a rental product.

Also on: [clouds]({{ '/timelines/clouds/' | relative_url }}).

## 2026-02 — SpaceX acquires xAI

Share exchange. Boards: SpaceX ~$1T, xAI ~$250B. Combined ~$1.25T private. Musk memo: vertically integrated engine — AI, rockets, space internet, X — and **data centers in space** as a stated driver. xAI holders get 0.1433 SpaceX shares per xAI share.

- [NYT](https://www.nytimes.com/2026/02/02/business/spacex-xai-deal.html)
- [Reuters](https://www.reuters.com/business/musks-spacex-merge-with-xai-combined-valuation-125-trillion-bloomberg-news-2026-02-02/)
- [WSJ on the structure](https://www.wsj.com/tech/elon-musk-xai-spacex-merger-2896ae1e)

## 2026-04 / 2026-06 / 2026-08 — Cursor

April: option — buy Anysphere for **$60B** in stock *or* pay ~$10B to keep working together. June 16: option exercised, days after the IPO; close targeted Q3. August: deal closed; Grok Bot ships on the combined stack. Cursor is the first large *outside* lab purchase. Coding distribution that Grok did not win on its own.

- [The Verge, exercise](https://www.theverge.com/ai-artificial-intelligence/950571/spacex-is-officially-buying-cursor-for-60-billion)
- [NYT](https://www.nytimes.com/2026/06/16/business/spacex-cursor-aquisition-ipo.html)
- Also on: [lab fission]({{ '/timelines/lab-fission/' | relative_url }}), [agents]({{ '/timelines/agents/' | relative_url }})

## 2026-05 / 2026-06 — Anthropic and Google rent Colossus

Anthropic: full Colossus 1, ~300 MW / 200k+ GPUs, S-1 rate **$1.25B/month** through May 2029 with a short kill switch. Google: ~110k GPUs, **$920M/month** Oct 2026–Jun 2029, framed as Gemini Enterprise bridge capacity. Reflection takes a smaller Colossus 2 slice later.

This is SpaceX as landlord, not as GPU-ABS borrower.

- [WIRED on the S-1 Anthropic dollars](https://www.wired.com/story/spacex-ipo-anthropic-compute-finances-risks/)
- [Reuters on Google](https://www.reuters.com/business/media-telecom/spacex-signs-cloud-deal-with-google-2026-06-05/)
- [WSJ Anthropic announcement](https://www.wsj.com/tech/ai/anthropic-inks-deal-to-use-all-of-spacexs-colossus-1-compute-capacity-56a7e2a1)
- Full writeup: [clouds]({{ '/timelines/clouds/' | relative_url }})

## 2026-06 — IPO

Nasdaq SPCX. Record raise (~$75B at $135), ~$1.77T at pricing. Whole company lists — Starlink is not carved out. S-1 language: dual monetization of compute (train Grok *and* rent the cluster). AI capex already rivaling the space division in the trailing quarters.

- [Reuters on pricing](https://www.reuters.com/world/musks-spacex-prices-record-75-billion-ipo-135-share-2026-06-11/)

## 2026 — Starmind (orbital compute)

FCC filing earlier in 2026 for up to **one million** AI satellites. Public name: Starmind. AI1 birds specified ~120 kW average compute, ~600 km, Starship-class deploy. Aug 2024/26 reporting: Nvidia Vera/Rubin as the first payload partner. Prototypes talked for 2027. This is a thesis, not a fleet. Treat it as the *reason given* for folding xAI into SpaceX, not as capacity you can rent today.

- Context coverage: [Notebookcheck on AI1](https://www.notebookcheck.net/SpaceX-lists-AI1-satellite-cooling-specs-for-Starmind-data-center-in-space.1340218.0.html)
- [Nvidia payload reporting](https://interestingengineering.com/ai-robotics/spacex-nvidia-starmind-ai1-compute-payload)

## What this page is not

A launch log. Falcon and Starship matter here only as the cash and the heavy-lift that make Colossus and Starmind imaginable. Model-quality claims stay on [capability stack]({{ '/timelines/capability-stack/' | relative_url }}) when there is a paper.
