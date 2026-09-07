---
layout: default
title: Clouds
permalink: /timelines/clouds/
---

# Hyperscalers and neoclouds

<p class="meta">Who owns the rack, and who lent against the chip</p>

Hyperscalers (Microsoft, Google, Amazon, Meta, then Oracle) fund campuses from cash flow and parent-level bonds. Neoclouds (CoreWeave, Lambda, Crusoe, Nebius, Nscale) fund *this generation of GPUs* against the boxes and the take-or-pay behind them. The financing is the beat.

## How the money used to work

Pre-2023 data centers were real-estate credit: land, power, a long lease to a rated tenant. The server was a depreciating fixture. AI inverted that. The GPU is the scarce asset; the building is the host. Lenders had no playbook for a chip that can be obsolete in three years.

Also on: [Nvidia]({{ '/timelines/nvidia/' | relative_url }}) (circular cheques), [Cerebras]({{ '/timelines/cerebras/' | relative_url }}) (offtake without owning the cloud).

## 2023-08 — CoreWeave $2.3B, GPUs as collateral

Magnetar and Blackstone lead a delayed-draw facility. Reuters is explicit: **collateralized by Nvidia chips** (H100s), with a negotiated depreciation vs payoff schedule. Coatue, DigitalBridge, BlackRock, PIMCO, Carlyle in the book. Cash buys more GPUs against contracts already signed. First large public case of GPU-backed private debt.

Rate context later filings give ~15% floating — junk pricing for unfamiliar collateral.

- [Reuters](https://www.reuters.com/technology/coreweave-raises-23-billion-debt-collateralized-by-nvidia-chips-2023-08-03/)
- [CoreWeave blog](https://www.coreweave.com/blog/coreweave-secures-2-3-billion-debt-financing-magnetar-capital-blackstone)
- [TechCrunch](https://techcrunch.com/2023/08/03/coreweave-which-provides-cloud-infrastructure-for-ai-training-secures-2-3b-loan/)

## 2024-05 — $7.5B, same structure, bigger book

Blackstone leads, Magnetar co-leads. Accordion to $7.5B. Investment-grade and speculative tranches split so CoreWeave can attach different customer credits. Blackstone: first time anyone had financed GPU chips at this size.

- [Blackstone](https://www.blackstone.com/news/press/coreweave-secures-7-5-billion-debt-financing-facility-led-by-blackstone-and-magnetar/)
- [IFR on the structure](https://www.ifre.com/ifr-awards/1443849/north-america-private-debt-loan-coreweaves-us7.5bn-financing)

## 2025-01 / 2025-09 — Stargate as a *headline* stack

OpenAI + Oracle + SoftBank announce a $100B-now / $500B-later US build (10 GW). Later: OpenAI–Oracle compute pact on the order of **$300B** over ~five years; more US sites. The JV itself is messy (staffing, who builds). The financing that actually closes is campus-level debt under Oracle and SoftBank names, not a single Stargate bond.

- [SoftBank, Sep 2025 site expansion](https://group.softbank/en/news/press/20250924)
- [NYT on the Oracle pact](https://www.nytimes.com/2025/09/10/technology/openai-oracle-data-centers-deal.html)

## 2025-03 — CoreWeave IPO

The GPU-debt model gets a ticker. Nvidia is both supplier and a capacity buyer (take-or-pay on unsold hours — see [Nvidia]({{ '/timelines/nvidia/' | relative_url }})).

## 2025-07 — DDTL 3.0, $2.6B, OpenAI-tied

CoreWeave 8-K: SOFR + 4.00%, due 2030, tied to a long OpenAI contract. Spreads collapse versus 2023 because the *customer* is now the credit, chips are the recovery floor.

- [Forbes reconstruction from filings](https://www.forbes.com/sites/daraabasiita/2026/06/09/gpu-debt-has-gone-investment-grade-heres-who-holds-the-risk/)

## 2026-03 — DDTL 4.0, $8.5B, investment-grade

Secured by GPUs *and* a Meta take-or-pay. Moody’s A3 / DBRS A (low). Fitch later A-sf on the Compute Acquisition Co. VIII vehicle. First widely cited IG rating on this collateral class. Floating piece ~SOFR + 2.25%.

- [Fitch on CCAC VIII](https://www.fitchratings.com/research/structured-finance/fitch-rates-coreweave-compute-acquisition-co-viii-loans-a-sf-outlook-stable-01-04-2026)
- Same Forbes filing recap as above

## 2026-04 — Oracle campus debt at Stargate scale

Single-site package reported ~$16.3B (Michigan / Saline), PIMCO anchoring the bond book after banks pulled back. Part of a larger Oracle partner-debt stack across Texas, Wisconsin, New Mexico. Hyperscaler variant: the *tenant contract* (OpenAI) is the story; the chip is inside Oracle’s order book.

- [The Next Web on the Michigan package](https://thenextweb.com/news/oracle-data-centre-16-billion-financing-stargate)

## 2026 — The rest of the neocloud book copies the template

Same instrument (delayed-draw term loan against GPUs + offtake), smaller names:

- **Lambda** — repeated secured facilities to buy Nvidia kits for Microsoft / Nvidia itself as tenant. [TechCrunch, $1B, Aug 2026](https://techcrunch.com/2026/08/28/neocloud-lambda-secures-1b-in-debt-to-buy-more-chips/)
- **Nebius** — first secured GPU loan (~$775M) after a Microsoft offtake; converts and Nvidia warrants fill the capex gap.
- **Nscale / Crusoe / IREN** — project SPVs, some with Microsoft or unnamed hyperscaler take-or-pays; IREN hardware package reported IG once Microsoft sits behind it.

By mid-2026 the rating agencies are explicit: hardware-only is still speculative; **investment-grade offtake** is what moves the spread.

## What the page is not

A capex scoreboard for Microsoft, Google, and Amazon. Those firms still mostly finance AI campuses as ordinary corporate cash and bonds. The new object is the neocloud SPV that pledges the chip *and* the contract.
