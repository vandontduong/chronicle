---
layout: default
title: TSMC
permalink: /timelines/tsmc/
---

# TSMC

<p class="meta">Who can print the die — then who can glue it to HBM.</p>

The physics of the transistor live on [integrated circuits]({{ '/timelines/integrated-circuits/' | relative_url }}). The board and the cheque live on [Nvidia]({{ '/timelines/nvidia/' | relative_url }}). This page is the foundry: nodes, EUV, CoWoS, and the Arizona political object.

## 1987 — Pure-play foundry

Morris Chang. TSMC makes other people's designs and does not compete with them. That split — design vs print — is why Nvidia can exist as a fabless firm.

- [TSMC — company](https://www.tsmc.com/english/aboutTSMC/company_profile)

## 2011–18 — 28 nm to 7 nm

Mobile SoCs pay for the plants. 7 nm (2018) is the node AI training parts start to care about. ASML EUV is in the building; high-volume EUV is the next beat.

## 2019–20 — EUV at volume, then CoWoS as the AI step

N5 / N7+ use EUV in production. Separately, Chip-on-Wafer-on-Substrate stops being a specialty for networking ASICs and becomes how you attach HBM to a training GPU. After this, *packaging capacity* is a second scarce object next to wafer starts.

- [TSMC CoWoS](https://www.tsmc.com/english/dedicatedFoundry/technology/cowos)

## 2022-10 — Export controls hit the tool flow

US BIS rules restrict leading-edge tools and high-end GPUs to the PRC. TSMC is not the target on paper. It is the plant the rules are written around: N5/N4/N3 and CoWoS sit in Taiwan. Subsequent years tighten HBM and add-on packaging. Die physics: [integrated circuits]({{ '/timelines/integrated-circuits/' | relative_url }}).

- [BIS, 7 Oct 2022](https://www.bis.doc.gov/index.php/documents/about-bis/newsroom/press-releases/3158-2022-10-07-bis-press-release-advanced-computing-and-semiconductor-manufacturing-controls-final/file)

## 2024-04 / 2024-11 — Arizona as industrial policy

CHIPS Act: up to $6.6B direct plus loans against a $65B+ Phoenix cluster (later expanded). Fab 1 (N4/N5) targets volume in 2025. Early yields reported in line with Taiwan. The wafers still fly back to Taiwan for CoWoS.

- [NIST — TSMC Arizona award](https://www.nist.gov/news-events/news/2024/11/biden-harris-administration-announces-chips-incentives-award-tsmc-arizona)
- [NIST project page](https://www.nist.gov/chips/tsmc-arizona-phoenix)

## 2025–26 — N2, and packaging as the bottleneck

N2 (GAA nanosheet) ramps. CoWoS demand for 2026 is cited near a million wafers vs ~370k in 2024; Nvidia alone is widely estimated as the majority book. TSMC talks 5.5-reticle CoWoS in 2026 and much larger interposers later. The constraint on GB200-class racks is often the package, not the litho.

- Also on: [Nvidia]({{ '/timelines/nvidia/' | relative_url }}), [clouds]({{ '/timelines/clouds/' | relative_url }})

## 2026-04 — CoWoS in Arizona, later

TSMC says advanced packaging (CoWoS / 3D-IC) on the Arizona site before 2029. Until then the US fab is a front-end. Amkor is the nearer-term US packaging bet (Apple / Nvidia).

- [Reuters, 22 Apr 2026](https://www.reuters.com/world/asia-pacific/tsmc-plans-open-chip-packaging-plant-arizona-by-2029-executive-says-2026-04-22/)

## What this page is not

A node roadmap slide. N3 vs N3E vs A16 only land here when they change who can buy capacity. Samsung and Intel foundry are contrast, not a second spine, until one of them takes a meaningful slice of AI CoWoS-class packaging.
