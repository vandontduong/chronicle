---
layout: default
title: Clouds
permalink: /timelines/clouds/
---

# Hyperscalers and neoclouds

<p class="meta">Who owns the rack, and who lent against the chip</p>

Hyperscalers fund campuses from cash flow and parent bonds. Neoclouds fund this generation of GPUs against the boxes and the offtake. SpaceX is a third object: a rocket company that built Colossus for Grok, then rented the surplus to rivals. A fourth origin story sits underneath the neoclouds: **proof-of-work miners who already had cheap megawatts**.

## How the money used to work

Pre-2023 data centers were real-estate credit: land, power, a long lease to a rated tenant. The server was a depreciating fixture. AI inverted that. The GPU is the scarce asset; the building is the host. Lenders had no playbook for a chip that can be obsolete in three years.

Also on: [Nvidia]({{ '/timelines/nvidia/' | relative_url }}), [Cerebras]({{ '/timelines/cerebras/' | relative_url }}), [lab fission]({{ '/timelines/lab-fission/' | relative_url }}) (xAI → SpaceX).

## 2019–26 — Miners become landlords

Bitcoin and Ethereum mining taught a generation of operators to hunt interconnects, substations, and ugly power that utilities would not sell to a hyperscaler on a five-year lead time. After ETH's Merge killed GPU mining, and after the 2024 BTC halving crushed hash margins, those sites were the only liquid *megawatts with a building*. The pivot is not “ASICs run GPT.” ASICs do not. The asset that transferred is **power + land + a permitted shed**. Liquid cooling, fiber, and GPU debt get bolted on later.

Three shapes:

1. **GPU miner → GPU cloud.** Same chip family. CoreWeave leaves ETH mining and keeps the cards.
2. **BTC miner → HPC landlord.** Tear out miners, host someone else's GPUs (Core Scientific → CoreWeave).
3. **BTC miner → own neocloud.** Keep the campus, buy GB300s, sell cloud (IREN, Crusoe after selling the flare-gas mine).

### CoreWeave — ETH GPUs, then a cloud

Started as a GPU miner. Merge ends the hash business; the same boxes become an AI cloud. The $2.3B GPU-backed loan (next beat) is that pivot with a capital-markets wrapper.

- Context: [how CoreWeave and miners pivoted](https://bitcoinethereumnews.com/tech/how-coreweave-and-miners-pivoted/)

### Core Scientific — 2024-06 hosting deal

Public BTC miner signs 12-year HPC leases with CoreWeave. First cut ~200 MW / >$3.5B; later expansions to ~590 MW and ~$10B over the terms. JPMorgan treated the announcement as the moment the whole listed-miner complex repriced as dual-use power.

- [Core Scientific, 3 Jun 2024](https://investors.corescientific.com/news-events/press-releases/detail/74/core-scientific-to-provide-approximately-200-mw-of-infrastructure-to-host-coreweaves-high-performance-computing-services-capturing-significant-ai-compute-opportunity)
- [CoinDesk on the later expansion](https://www.coindesk.com/business/2026/05/07/core-scientific-sold-usd208-million-of-bitcoin-in-q1-as-ai-pivot-continues)

### Galaxy Helios — a mine that becomes a campus

West Texas site bought from Argo as a BTC mine. Mining wound down; Phase I hands CoreWeave 133 MW IT load (2026-07) under a 15-year lease. Same tenant, same story: hash rate out, liquid-cooled racks in.

- [The Block](https://www.theblock.co/post/407396/galaxy-delivers-133-mw-of-critical-it-load-to-coreweave-as-helios-bitcoin-mine-turns-ai-hub)
- [DCD](https://www.datacenterdynamics.com/en/news/galaxy-digital-completes-first-phase-of-pivoting-cryptomine-to-ai-hosting/)

### Crusoe — flare gas → Stargate

2018: modular miners on stranded / flared gas. 2024: Abilene campus that becomes Stargate's first large site. 2025-03: **sells the Bitcoin / Digital Flare Mitigation business to NYDIG** so the firm is only AI campuses and cloud.

- [DCD on the NYDIG sale](https://www.datacenterdynamics.com/en/news/crusoe-exits-crypto-operations-to-focus-on-ai-sell-business-to-nydig/)
- [Forbes on the modular follow-on](https://www.forbes.com/sites/annatong/2026/03/12/from-gigawatts-to-grab-and-go-crusoe-leans-into-modular-ai-data-centers/)

### IREN (née Iris Energy) — miner that sells the cloud itself

Childress, Texas was a mine. Nov 2025: five-year, **$9.7B** cloud contract with Microsoft (GB300 / Horizon). Aug 2026: Horizon 1 accepted; Nvidia Exemplar Cloud. GPU debt then prices off the Microsoft offtake (see IREN in the 2026 book below).

- [IREN 8-K / Horizon 1](https://www.stocktitan.net/sec-filings/IREN/8-k-iren-ltd-reports-material-event-e67c1bd9fff6.html)
- [The Block](https://www.theblock.co/news/business/2026-08-17-iren-delivers-first-four-ai-cloud-deployments-microsoft-under-9-7-billion-deal-412016)

Hut 8, TeraWulf, MARA, HIVE run variations of the same conversion. The scarce input was never the ASIC. It was a megawatt you could energize this year.

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

## 2024–26 — Colossus (Memphis / Southaven)

xAI builds a training campus on the Tennessee–Mississippi line for Grok, then SpaceX absorbs xAI (Feb 2026). Colossus 1 + 2 are cited in the SpaceX S-1 at about **1 GW** nameplate, with more power being stood up on-site (turbines, then a permanent plant). This is not project-finance GPU debt. It is founder-balance-sheet capex that later gets rented.

Also on: [lab fission]({{ '/timelines/lab-fission/' | relative_url }}).

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

## 2026-05 — Anthropic takes Colossus 1

Anthropic rents the full Colossus 1 slice: ~300 MW, 200k+ Nvidia GPUs. SpaceX S-1: **$1.25B per month** through May 2029 after a cheap ramp, ~$15B/year if it runs. Either side can terminate on short notice (Musk: SpaceX wanted the option to take the cluster back). Do not treat the headline multi-year total as locked cash.

- [WSJ announcement](https://www.wsj.com/tech/ai/anthropic-inks-deal-to-use-all-of-spacexs-colossus-1-compute-capacity-56a7e2a1)
- [WIRED on the S-1 dollars](https://www.wired.com/story/spacex-ipo-anthropic-compute-finances-risks/)
- [The Verge](https://www.theverge.com/science/935229/spacex-anthropic-ipo-ai-capacity-deal-colossus)

## 2026-06 — Google rents Colossus too

Alphabet files / SpaceX discloses: **$920M per month** from Oct 2026 through Jun 2029 for ~110k GPUs plus CPUs and memory. Google’s line: bridge capacity for Gemini Enterprise while its own campuses catch up. Cancellation rights after the first stretch. Reuters: the two disclosed offtakes are >$70B *if* neither dies early.

- [Reuters](https://www.reuters.com/business/media-telecom/spacex-signs-cloud-deal-with-google-2026-06-05/)
- [The Next Web](https://thenextweb.com/news/google-spacex-920-million-month-compute-deal)

Reflection later takes a smaller GB300 slice at Colossus 2 (~$150M/month). Same landlord pattern, not a new financing instrument.

SpaceX here is a **hyperscaler that skipped the GPU-ABS market**: build on its own books, rent to IG and near-IG labs, keep the termination option. Contrast CoreWeave, which borrows *against* the same kind of contract.

## 2026 — The rest of the neocloud book copies the template

Same instrument (delayed-draw term loan against GPUs + offtake), smaller names:

- **Lambda** — repeated secured facilities to buy Nvidia kits for Microsoft / Nvidia itself as tenant. [TechCrunch, $1B, Aug 2026](https://techcrunch.com/2026/08/28/neocloud-lambda-secures-1b-in-debt-to-buy-more-chips/)
- **Nebius** — first secured GPU loan (~$775M) after a Microsoft offtake; converts and Nvidia warrants fill the capex gap.
- **Nscale / Crusoe / IREN** — project SPVs, some with Microsoft or unnamed hyperscaler take-or-pays; IREN hardware package reported IG once Microsoft sits behind it.

By mid-2026 the rating agencies are explicit: hardware-only is still speculative; **investment-grade offtake** is what moves the spread.

## What the page is not

A capex scoreboard for Microsoft, Google, and Amazon cash-flow campuses. Those still look like ordinary corporate bonds. The new objects are the neocloud SPV that pledges the chip *and* the contract, and SpaceX renting a cluster it already paid for.
