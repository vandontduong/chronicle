---
layout: default
title: HBM
permalink: /timelines/hbm/
---

# HBM

<p class="meta">The stack next to the GPU. TSMC glues it. SK Hynix, Samsung, and Micron print it. Nvidia decides who ships.</p>

Who *packages* the stack onto the logic die: [TSMC]({{ '/timelines/tsmc/' | relative_url }}) (CoWoS). Who *sells* the board: [Nvidia]({{ '/timelines/nvidia/' | relative_url }}). Why bandwidth is the scarce object: [integrated circuits]({{ '/timelines/integrated-circuits/' | relative_url }}) (Horowitz, then Gholami). The context *window* is [memory]({{ '/timelines/memory/' | relative_url }}). Disk-to-GPU DMA is [storage]({{ '/timelines/storage/' | relative_url }}).

This page is the DRAM cube: TSV stacks, JEDEC generations, and the qualification that turns a stack into revenue.

## 2013-10 / 2015 — A standard, then a card

AMD and SK Hynix propose a wide, short-reach interface on a silicon interposer. JEDEC publishes JESD235 (HBM) in October 2013. SK Hynix builds the first TSV stack. The first shipping product is AMD's Fiji / Radeon R9 Fury (2015) — graphics, not training. Hybrid Memory Cube (Micron / Intel) is the rival that does not become the GPU default.

- [JEDEC JESD235 family](https://www.jedec.org/standards-documents/docs/jesd235a)
- [SK Hynix on the AMD joint development](https://news.skhynix.com/en/the-story-of-sk-hynixs-hbm-development/)

## 2016 — HBM2 on a training board

JEDEC HBM2 (JESD235A, Jan 2016). Nvidia P100 ships with Samsung HBM2 and the first NVLink. The object moves from a graphics bus to the memory next to a training GPU. DGX-1 is eight of those boards — [Nvidia]({{ '/timelines/nvidia/' | relative_url }}).

- [NVIDIA DGX-1](https://www.nvidia.com/en-us/data-center/dgx-1/)

## 2022-01 / 2022-06 — HBM3, and SK Hynix on H100

JEDEC HBM3 (JESD238). SK Hynix mass-produces first, June 2022, into Nvidia H100. Qualification, not a press-spec, is the gate: an unqualified stack earns nothing on that platform. Samsung and Micron spend the next two years chasing the same socket.

- [JEDEC publishes HBM3](https://www.jedec.org/news/pressreleases/jedec-publishes-hbm3-update-standard)
- [SK Hynix HBM history](https://news.skhynix.com/en/the-story-of-sk-hynixs-hbm-development/)

## 2021 / 2024 — The wall has a name again

Decoder inference is memory-bound. FLOPs grew faster than DRAM bandwidth. HBM is the industrial reply; CoWoS is how you attach enough stacks. The paper lives on [integrated circuits]({{ '/timelines/integrated-circuits/' | relative_url }}); the product lives here.

- Gholami et al. *AI and Memory Wall*. [arXiv:2403.14123](https://arxiv.org/abs/2403.14123)
- Horowitz. *Computing's energy problem*. ISSCC 2014. [IEEE](https://ieeexplore.ieee.org/document/6757323)

## 2024 — HBM3E and a three-vendor race

SK Hynix volume on HBM3E (March 2024) for H200. Micron qualifies an 8-hi 24 GB part for the same socket. Samsung misses Nvidia's heat and power bar through 2024, then passes 12-hi HBM3E in September 2025. Share moves with *who passed qual*, not who announced a terabyte-per-second slide.

Blackwell boards take more stacks and a larger interposer. The scarce step is often CoWoS, not the DRAM wafer — [TSMC]({{ '/timelines/tsmc/' | relative_url }}).

## 2025-04 — HBM4 is a spec

JEDEC JESD270-4: up to 8 Gb/s on a 2048-bit interface (~2 TB/s per stack), 32 channels, 4- to 16-hi, up to 64 GB per cube. Backwards compatible with HBM3 controllers. AMD, Nvidia, Google, Micron, Samsung, SK Hynix on the press note. Samples ship before the PDF; Rubin-class parts are the intended socket.

- [JEDEC, 16 Apr 2025](https://www.jedec.org/news/pressreleases/jedec-and-industry-leaders-collaborate-release-jesd270-4-hbm4-standard-advancing)

## 2026-06 / 2026-07 — Partnership, then a larger LOI

8 Jun 2026: SK Hynix and Nvidia announce a multi-year technology partnership — co-develop next-gen memory against Nvidia's roadmap (Vera Rubin, Vera CPU, Jetson Thor). Supply is the point; no dollar figure on that note.

25 Jul 2026: SK Group and Nvidia sign letters of intent on a **$500B+** package that mixes AI-factory buildout *and* memory supply. Treat the headline as an LOI, not a closed HBM purchase.

- [SK Hynix — multi-year partnership](https://news.skhynix.com/en/multi-year-tech-partnership-with-nvidia/)
- [SK Hynix — SK Group / Nvidia LOI](https://news.skhynix.com/en/skhynix-nvidia-partnership-2026/)

## 2026-06 / 2026-08 — HBM4E samples, Indiana dirt

SK Hynix ships 12-hi HBM4E samples (claimed 16 Gb/s/pin, 48 GB, Advanced MR-MUF). August: groundbreaking on a US HBM production base in Indiana. Yongin Y2 / Cheongju M17 are the Korean capacity bets (board-approved capex, cleanrooms late-2020s). Capacity follows qual, not the other way around.

- [SK Hynix — HBM4E samples](https://news.skhynix.com/en/sk-hynix-ships-samples-of-12-layer-next-gen-hbm4e-2/)

## What this page is not

A SKU table (8-hi vs 12-hi vs every GB number on H100 / H200 / B200). GDDR and LPDDR stay off unless a training board ships on them. HMC is the road not taken, not a second spine. Custom base-die gossip lands here only when a vendor *ships* on a named Nvidia or AMD socket.
