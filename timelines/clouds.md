---
layout: default
title: Clouds
permalink: /timelines/clouds/
---

# Hyperscalers and neoclouds

<p class="meta">Who owns the rack, and who lent against the chip</p>

Hyperscalers fund campuses from cash flow and parent bonds. Neoclouds fund this generation of GPUs against the boxes and the offtake. SpaceX is a third object: a rocket company that built Colossus for Grok, then rented the surplus. A fourth origin sits under the neoclouds: **miners who already had cheap megawatts**. Company object for Colossus build and takeouts: [SpaceX]({{ '/timelines/spacex/' | relative_url }}). Protocol papers for the hash that paid for those sheds: [cryptocurrency]({{ '/timelines/cryptocurrency/' | relative_url }}). Silicon and lab cheques: [Nvidia]({{ '/timelines/nvidia/' | relative_url }}). The 2026 manager platforms that try to turn that GPU loan into an asset class live **here**.

The first public clouds were a side quest. Retail, search, and Windows paid for the plants. Renting leftover capacity was the experiment.

## How the money used to work

Pre-2023 data centers were real-estate credit: land, power, a long lease to a rated tenant. The server was a depreciating fixture. AI inverted that. The GPU is the scarce asset; the building is the host. Lenders had no playbook for a chip that can be obsolete in three years.

## 2006–12 — Cloud as overflow from the main business

Amazon did not start as a cloud company. It started as a catalog. By the mid-2000s the hard problem inside Amazon was provisioning for seasonal spikes, then watching the fleet sit idle. S3 launched 14 Mar 2006. EC2 followed that summer as the internal platform with a price list. Two decades later AWS is the profit engine; it is not larger than retail *revenue*.

- [Amazon on the S3 launch](https://www.aboutamazon.com/news/aws/the-earliest-aws-customers-who-helped-build-the-cloud)
- [ZDNET / Pinkham on EC2 as internal infra first](https://www.zdnet.com/article/how-amazon-exposed-its-guts-the-history-of-awss-ec2/)

Google: the plants existed to crawl the web and serve ads. App Engine (Apr 2008) let outsiders sit on Bigtable and GFS. Compute Engine (Jun 2012) is the explicit IaaS launch — Linux VMs on the search fleet.

- [TechCrunch, App Engine](https://techcrunch.com/2008/04/07/google-jumps-head-first-into-web-services-with-google-app-engine/)
- [TechCrunch, Compute Engine](https://techcrunch.com/2012/06/28/google-compute-engine/)

Microsoft was late because the franchise was Windows and Office on the customer's premises. Azure (PDC, 27 Oct 2008) is a cloud grafted onto that stack so .NET shops would not leave Redmond to rent a box.

- [WIRED, PDC 2008](https://www.wired.com/2008/10/pdc-2008-microsoft-aims-for-the-clouds-with-windows-azure-/)

Meta never productized the social-graph fleet as public IaaS at AWS scale. Oracle sold databases, then bolted a cloud onto the license.

The 2020s inversion: AI *is* the main business for the new names. Neoclouds have no store to amortize empty hours. SpaceX is the old pattern run in reverse — rockets paid for some of the plants; Colossus tries to pay for itself by renting to Anthropic and Google.

## 2019–26 — Miners become landlords

Bitcoin and Ethereum mining taught operators to hunt interconnects, substations, and ugly power that a hyperscaler could not energize on a five-year utility queue. After ETH's Merge (15 Sep 2022) killed GPU mining, and after the Apr 2024 BTC halving crushed hash margins, those sites were liquid *megawatts with a building*. The asset that transferred is **power + land + a permitted shed**. Why those protocols existed: [cryptocurrency]({{ '/timelines/cryptocurrency/' | relative_url }}).

Three shapes:

1. **GPU miner → GPU cloud.** Same chip family. CoreWeave leaves ETH mining and keeps the cards.
2. **BTC miner → HPC landlord.** Tear out miners, host someone else's GPUs (Core Scientific → CoreWeave).
3. **BTC miner → own neocloud.** Keep the campus, buy GB300s, sell cloud (IREN; Crusoe after selling the flare-gas mine).

### CoreWeave — ETH GPUs, then a cloud

Founded 2017 as Atlantic Crypto. ETH mining was 61% of 2022 revenue ($9.7M of $15.8M). Merge ends that line. The same Nvidia boxes become an AI cloud. The 2023 GPU-backed loan is that pivot with a capital-markets wrapper.

- [CNBC on the mining years](https://www.cnbc.com/2025/03/30/coreweaves-7-year-journey-to-ipo-wound-through-crypto-before-ai.html)
- [The Block on post-Merge revenue](https://www.theblock.co/news/business/2025-03-04-coreweave-previously-mined-ethereum-but-its-post-ipo-ai-focus-now-has-it-seeking-to-raise-4-billion-via-an-ipo-as-revenues-surge-344457)

### Core Scientific — hosting, then a bigger book

3 Jun 2024: 12-year HPC leases with CoreWeave. First cut **~200 MW** and **more than $3.5B** cumulative revenue over the initial terms. Later expansions take the book to **~590 MW** and **more than $10B** contracted value. As of mid-2026, hundreds of those megawatts have started billing.

- [Core Scientific, 3 Jun 2024](https://investors.corescientific.com/news-events/press-releases/detail/74/core-scientific-to-provide-approximately-200-mw-of-infrastructure-to-host-coreweaves-high-performance-computing-services-capturing-significant-ai-compute-opportunity)
- [CORZ 10-Q: ~590 MW contracted](https://www.sec.gov/Archives/edgar/data/1839341/000183934126000014/core-20260630.htm)

### Galaxy Helios — a mine that becomes a campus

West Texas site bought from Argo as a BTC mine. Mining wound down; Phase I hands CoreWeave **133 MW** IT load (Jul 2026) under a 15-year lease.

- [The Block](https://www.theblock.co/post/407396/galaxy-delivers-133-mw-of-critical-it-load-to-coreweave-as-helios-bitcoin-mine-turns-ai-hub)
- [DCD](https://www.datacenterdynamics.com/en/news/galaxy-digital-completes-first-phase-of-pivoting-cryptomine-to-ai-hosting/)

### Crusoe — flare gas, then exit mining

2018: modular miners on stranded / flared gas. 2024: Abilene campus that becomes an early Stargate site. **25 Mar 2025:** sale of the Bitcoin / Digital Flare Mitigation business to NYDIG (~425 modular sites, ~270 MW generation). After close, Crusoe is campuses and cloud.

- [Crusoe newsroom](https://www.crusoe.ai/resources/newsroom/nydig-to-acquire-crusoes-bitcoin-mining-operation-crusoe-to-scale-vertically)
- [DCD](https://www.datacenterdynamics.com/en/news/crusoe-exits-crypto-operations-to-focus-on-ai-sell-business-to-nydig/)

### IREN — miner that sells the cloud itself

Childress, Texas was a mine. **3 Nov 2025:** five-year **$9.7B** GPU-cloud contract with Microsoft (GB300s, 20% prepayment). Separate ~$5.8B equipment buy from Dell. GPU debt then prices off the Microsoft offtake.

- [Reuters](https://www.reuters.com/technology/microsoft-signs-97-billion-contract-with-iren-nvidia-chips-2025-11-03)
- [TechCrunch](https://techcrunch.com/2025/11/03/microsoft-inks-9-7bil-deal-with-australias-iren-for-ai-cloud-capacity/)

Hut 8, TeraWulf, MARA, HIVE run variations. The scarce input was a megawatt you could energize this year.

## 2023-08 — CoreWeave $2.3B, GPUs as collateral

Magnetar and Blackstone lead a delayed-draw facility announced 3 Aug 2023. Reuters: **collateralized by Nvidia chips**, with a negotiated depreciation vs payoff schedule. Coatue, DigitalBridge, BlackRock, PIMCO, Carlyle in the book. First large public case of GPU-backed private debt.

- [Reuters](https://www.reuters.com/technology/coreweave-raises-23-billion-debt-collateralized-by-nvidia-chips-2023-08-03/)
- [CoreWeave](https://www.coreweave.com/blog/coreweave-secures-2-3-billion-debt-financing-magnetar-capital-blackstone)

## 2024-05 — Up to $7.6B, same structure

Blackstone leads, Magnetar co-leads. Announced as $7.5B; S-1 / later coverage treat the facility as **up to $7.6B** (DDTL 2.0). Investment-grade and speculative borrowing bases split so CoreWeave can attach different customer credits. Drawn amount at IPO was only part of the commitment.

- [Blackstone](https://www.blackstone.com/news/press/coreweave-secures-7-5-billion-debt-financing-facility-led-by-blackstone-and-magnetar/)

## 2024–26 — Colossus (Memphis / Southaven)

xAI builds a training campus on the Tennessee–Mississippi line for Grok. SpaceX absorbs xAI (Feb 2026). Colossus 1 + 2 are cited in the SpaceX S-1 at about **1 GW** nameplate. Founder-balance-sheet capex that later gets rented — not a GPU-ABS issue. Build story: [SpaceX]({{ '/timelines/spacex/' | relative_url }}).

## 2025-01 / 2025-09 — Stargate the pledge, Oracle the contract

21 Jan 2025: OpenAI, SoftBank, Oracle, and MGX announce Stargate. **$100B** to start deploying; **up to $500B** over four years. SoftBank has financial responsibility; OpenAI has operational responsibility. That is a JV *intent*, not a single closed bond.

Sep 2025: OpenAI–Oracle compute pact reported at **~$300B over ~five years**, starting 2027, ~4.5 GW. Separate from the White House headline.

- [OpenAI, Stargate](https://openai.com/index/announcing-the-stargate-project/)
- [NYT on the Oracle pact](https://www.nytimes.com/2025/09/10/technology/openai-oracle-data-centers-deal.html)

## 2025-03 — CoreWeave IPO

28 Mar 2025, Nasdaq CRWV. Priced at **$40**, raise cut to about **$1.5B**. Microsoft was ~60%+ of 2024 revenue. Nvidia is supplier, investor, and a capacity buyer (take-or-pay on unsold hours — [Nvidia]({{ '/timelines/nvidia/' | relative_url }})).

## 2025-07 — DDTL 3.0, $2.6B, OpenAI-tied

Delayed-draw term loan closed 31 Jul 2025, **SOFR + 4.00%**, used to buy kit for a long OpenAI contract. Morgan Stanley and MUFG lead. Spreads are inside the 2023 book because the *customer* is the credit.

- [CoreWeave, 31 Jul 2025](https://investors.coreweave.com/news/news-details/2025/CoreWeave-Closes-2-6-Billion-Secured-Debt-Financing-Facility-Strengthening-Market-Position-as-AI-Cloud-Leader/default.aspx)

## 2026-03 — DDTL 4.0, $8.5B, investment-grade

Closed 31 Mar 2026. Initially drawable ~$7.5B, expandable to **$8.5B**. Moody’s **A3** / DBRS **A (low)** on the Compute Acquisition Co. VIII vehicle. Floating piece **SOFR + 2.25%**, maturity Mar 2032. First widely cited IG rating on GPU + contract collateral. Later reconstructions name a Meta take-or-pay as the offtake; the launch release said only “customer contracts.”

- [Fitch on CCAC VIII](https://www.fitchratings.com/research/structured-finance/fitch-rates-coreweave-compute-acquisition-co-viii-loans-a-sf-outlook-stable-01-04-2026)

## 2026-04 — Oracle campus debt at Stargate scale

Related Digital closes a **$16B** package for the Saline Township, Michigan campus (Oracle tenant, OpenAI workload, >1 GW). About **$14B** of bonds sold; PIMCO anchors ~$10B; Blackstone-affiliated funds put in equity (~$2B reported). Coupon on the long bonds ~7.5%, maturity 2045. The *tenant contract* is the story; the chip sits in Oracle's order book.

- [Reuters](https://www.reuters.com/technology/related-digital-secures-financing-16-billion-oracle-data-center-michigan-2026-04-24/)
- [Oracle / Related construction note](https://www.oracle.com/news/announcement/related-digital-oracle-openai-walbridge-and-governor-whitmer-celebrate-construction-of-stargate-campus-in-saline-township-2026-06-01/)

## 2026-05 — Anthropic takes Colossus 1

Anthropic rents the Colossus 1 slice: ~300 MW, on the order of 200k GPUs. SpaceX S-1: **$1.25B per month** through May 2029 after a cheap ramp — about **$15B/year if it runs**. Either side can terminate on **90 days' notice**. Do not treat the multi-year headline as locked cash.

- [WSJ](https://www.wsj.com/tech/ai/anthropic-inks-deal-to-use-all-of-spacexs-colossus-1-compute-capacity-56a7e2a1)
- [WIRED on the S-1 dollars](https://www.wired.com/story/spacex-ipo-anthropic-compute-finances-risks/)

## 2026-06 — Google rents Colossus too

Disclosed 5 Jun 2026: **$920M per month** from Oct 2026 through Jun 2029 for ~**110k GPUs** plus CPUs and memory. Cancellation after the first stretch. The two disclosed offtakes are **>$70B only if neither dies early**. Reflection later takes a smaller GB300 slice at Colossus 2.

- [Reuters](https://www.reuters.com/business/media-telecom/spacex-signs-cloud-deal-with-google-2026-06-05/)
- [The Next Web](https://thenextweb.com/news/google-spacex-920-million-month-compute-deal)

SpaceX skipped the GPU-ABS market: build on its own books, rent to labs, keep the termination option. Contrast CoreWeave, which borrows *against* the same kind of contract.

## 2026 — The rest of the neocloud book copies the template

Same instrument (delayed-draw term loan against GPUs + offtake), smaller names:

- **Lambda** — repeated secured facilities to buy Nvidia kits. [TechCrunch, $1B, Aug 2026](https://techcrunch.com/2026/08/28/neocloud-lambda-secures-1b-in-debt-to-buy-more-chips/)
- **Nscale / Crusoe / IREN** — project SPVs; IREN hardware debt later prices off the Microsoft offtake.

By mid-2026 the agencies are explicit: hardware-only is still speculative; **investment-grade offtake** is what moves the spread.

## 2026-08-10 — Nvidia tries to productize the loan

MOUs with **Apollo, BlackRock, Blackstone, Brookfield, Goldman Sachs, and KKR**. Independent platforms *designed to mobilize* **over $500B** of third-party capital over time for AI-factory kit — labs, enterprises, neoclouds. Not Nvidia revenue. Not one fund. Not a closed bond. The six underwrite customer, utilization, cash flow, and residual value themselves.

Nvidia's disclosed hook: on some deals, a **residual-value support** of **up to 25%** of an opportunity, project by project. Huang's line is that the chip is now an investable asset class (fungible, revenue-producing, transferable). That is the 2023 CoreWeave structure, standardized and aimed at pension-scale money. Disclosed GPU-backed facilities through mid-2026 are still tens of billions, not hundreds.

- [Nvidia blog](https://blogs.nvidia.com/blog/nvidia-ai-factory-compute/)
- [Reuters](https://www.reuters.com/technology/wall-street-giants-partner-with-nvidia-500-billion-ai-financing-deal-ft-reports-2026-08-10/)
- [CNBC](https://www.cnbc.com/2026/08/10/nvidia-wall-street-asset-managers-500-billion-ai-push.html)
- Firm page: [Nvidia]({{ '/timelines/nvidia/' | relative_url }})

## What the page is not

A capex scoreboard for Microsoft, Google, and Amazon cash-flow campuses. Those still look like ordinary corporate bonds. The new objects are the neocloud SPV that pledges the chip *and* the contract, SpaceX renting a cluster it already paid for, and a vendor-sponsored *platform* that has not yet raised the $500B it is designed to mobilize.
