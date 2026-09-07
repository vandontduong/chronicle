---
layout: default
title: Storage
permalink: /timelines/storage/
---

# Storage

<p class="meta">Tokens sit on rust and NAND before they sit in HBM.</p>

The *window* and the KV cache live on [memory]({{ '/timelines/memory/' | relative_url }}). KV spilled onto SSD as a serving pool lives on [disaggregated compute]({{ '/timelines/disaggregated-compute/' | relative_url }}). Who owns the rack lives on [clouds]({{ '/timelines/clouds/' | relative_url }}). The mix that gets written here lives on [data]({{ '/timelines/data/' | relative_url }}). Die physics and the memory wall live on [integrated circuits]({{ '/timelines/integrated-circuits/' | relative_url }}).

This page is persistent media and the path from disk to GPU. Not a Seagate / WD catalog.

## 1988 — RAID

Patterson, Gibson, Katz: many cheap disks as one reliable volume. Hyperscale nearline is still this paper with bigger platters.

- Patterson, Gibson, Katz. *A Case for Redundant Arrays of Inexpensive Disks (RAID)*. SIGMOD 1988. [PDF](https://www.cs.cmu.edu/~garth/RAIDpaper/Patterson88.pdf)

## 1979–80 / 2012 — Two disk companies, one nearline market

Seagate (ST-506) and Western Digital start as controller and drive vendors. WD buys HGST from Hitachi (2012) and inherits Ultrastar, the label clouds still buy as cold capacity. Product lines that matter later: Seagate **Exos**, WD **Ultrastar DC HC** (HDD) and **Ultrastar DC SN** (NVMe). IronWolf and Purple are not the AI object.

- [Seagate Exos](https://www.seagate.com/products/enterprise-drives/exos/)
- [WD Ultrastar](https://www.westerndigital.com/products/internal-drives/data-center-drives)

## 1984 / 2000s — NAND, then a server SSD

Masuoka (Toshiba): flash as a device. Decades later Samsung, Kioxia, WD (SanDisk), and Micron sell 3D NAND as the *checkpoint and feature-store* tier. HDD keeps the crawl and the backups; NVMe takes the hot set.

- Masuoka et al. *A new flash E2PROM cell*. IEDM 1984.

## 2003 / 2006 — A filesystem for the warehouse, then a product

GFS: commodity disks, single-master metadata, chunkservers. S3 (2006) is the public product of that idea — already a beat on [clouds]({{ '/timelines/clouds/' | relative_url }}). Training corpora still land here first.

- Ghemawat, Gobioff, Leung. *The Google File System*. SOSP 2003. [PDF](https://research.google.com/archive/gfs-sosp2003.pdf)

## 2008 — Heat the bit

Kryder et al.: heat-assisted magnetic recording. A laser writes a grain too stable to flip at room temperature. Seagate spends the next fifteen years turning the paper into a platform.

- Kryder et al. *Heat Assisted Magnetic Recording*. Proc. IEEE 96 (2008). [IEEE](https://ieeexplore.ieee.org/document/4694068)

## 2021 — Disk to HBM without the CPU

GPUDirect Storage: DMA between NVMe (or a NIC in front of a fabric) and GPU memory. No bounce buffer. Checkpoints, sharded datasets, and retrieval start to look like a CUDA path. Software home: [Nvidia]({{ '/timelines/nvidia/' | relative_url }}).

- [Accelerating IO: Magnum IO Storage](https://developer.nvidia.com/blog/accelerating-io-in-the-modern-data-center-magnum-io-storage/)
- [GPUDirect Storage Design Guide (PDF)](https://docs.nvidia.com/gpudirect-storage/pdf/design-guide.pdf)

## 2024–25 — Mozaic 3+ ships

Seagate Exos M / IronWolf Pro at **30TB** on HAMR (Mozaic 3+, ~3TB per disk). First time the Kryder paper is a volume SKU, not a roadmap slide. WD answers on ePMR / UltraSMR Ultrastar capacities in the same band, without HAMR in volume.

- [Seagate Mozaic 3+](https://www.seagate.com/innovation/mozaic/)
- [Tom's Hardware, 30TB HAMR](https://www.tomshardware.com/pc-components/hdds/seagate-unveils-30tb-hdds-for-the-masses-laser-powered-ironwolf-pro-and-exos-drives-are-now-widely-available)

## 2026-03 — Mozaic 4+ at hyperscale

Seagate: Mozaic 4+ qualified with two cloud majors, capacities up to **44TB**, roadmap talk toward 10TB/disk. The claim is $/TB and watts per exabyte for *AI-scale retention*, not IOPS. Checkpoints still want NAND.

- [Seagate, 3 Mar 2026](https://investors.seagate.com/news/news-details/2026/Seagate-Delivers-Industrys-Highest-Capacity-Hard-Drives-with-Next-Generation-Mozaic-4/default.aspx)

## What this page is not

A consumer NAS list. Optane as a failed persistent-memory product. Parallel file systems (Weka, VAST, DDN) only if a paper or a lab deployment changes the path to the GPU. Mooncake's KV-on-SSD pool stays on [disaggregated compute]({{ '/timelines/disaggregated-compute/' | relative_url }}).
