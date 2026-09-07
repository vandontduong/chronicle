---
layout: default
title: Integrated circuits
permalink: /timelines/integrated-circuits/
---

# Integrated circuits

<p class="meta">The die as constraint. Nvidia sells a system. Cerebras sells a wafer. This page is why both of those sentences are possible.</p>

Company objects live on [Nvidia]({{ '/timelines/nvidia/' | relative_url }}) and [Cerebras]({{ '/timelines/cerebras/' | relative_url }}). Kernels and quantization live on [efficiency]({{ '/timelines/efficiency/' | relative_url }}). Who paid for the rack lives on [clouds]({{ '/timelines/clouds/' | relative_url }}).

## 1947–59 — Switch, then circuit

Point-contact transistor at Bell Labs, then Kilby (TI) and Noyce (Fairchild) put more than one device on one piece of semiconductor. After this, “more devices per package” is an industry, not a lab demo.

- Bardeen and Brattain. *The transistor, a semi-conductor triode*. Phys. Rev. 1948.
- Kilby. *Miniaturized electronic circuits*. US patent 3,138,743 (filed 1959).
- Noyce. *Semiconductor device-and-lead structure*. US patent 2,981,877 (filed 1959).

## 1965 — Moore

A doubling observation written as a planning document. The field spends the next fifty years treating transistor count as the independent variable.

- Moore. *Cramming more components onto integrated circuits*. Electronics, 19 Apr 1965. [PDF reprint](https://www.cs.utexas.edu/~fussell/courses/cs352h/papers/moore.pdf)

## 1974 — Dennard

Voltage, capacitance, and delay scale together. You get more transistors *and* they switch faster *and* they use about the same power per area. When this breaks (mid-2000s), the industry turns to multicore, then to specialized arrays.

- Dennard et al. *Design of ion-implanted MOSFET's with very small physical dimensions*. IEEE JSSC 1974. [IEEE](https://ieeexplore.ieee.org/document/1054856)

## 2014 — Energy, not transistors

Horowitz: an off-chip DRAM access costs orders of magnitude more energy than an arithmetic op. After Dennard, the scarce object is *data movement*, not gate count. Every later accelerator paper is a reply to this slide.

- Horowitz. *Computing's energy problem (and what we can do about it)*. ISSCC 2014. [IEEE](https://ieeexplore.ieee.org/document/6757323)

## 2016 — Dataflow as architecture

Eyeriss: row-stationary mapping so weights and activations reuse on-chip. Sze, Chen, Emer: a survey that names the problem — efficient *processing*, not a bigger ALU.

- Chen et al. *Eyeriss: An Energy-Efficient Reconfigurable Accelerator for Deep Convolutional Neural Networks*. [arXiv:1602.01602](https://arxiv.org/abs/1602.01602)
- Sze, Chen, Yang, Emer. *Efficient Processing of Deep Neural Networks: A Tutorial and Survey*. [arXiv:1703.09039](https://arxiv.org/abs/1703.09039)

## 2017-04 — TPU v1 in production

Google ships a 256×256 8-bit systolic array as a datacenter ASIC. Inference, not training. The paper is the first public proof that a domain-specific matrix unit beats a contemporary GPU on TOPS/W for real serving traffic.

- Jouppi et al. *In-Datacenter Performance Analysis of a Tensor Processing Unit*. [arXiv:1704.04760](https://arxiv.org/abs/1704.04760)

cuDNN and Tensor Cores — the GPU answer to the same energy slide — live on [Nvidia]({{ '/timelines/nvidia/' | relative_url }}).

## 2019– — Don't cut the wafer

Cerebras keeps the 300 mm wafer intact so SRAM and interconnect stay on-die. Decode bandwidth is the product. Architecture and takeout attempts: [Cerebras]({{ '/timelines/cerebras/' | relative_url }}).

- [Cerebras architecture deep dive](https://www.cerebras.ai/blog/cerebras-architecture-deep-dive-first-look-inside-the-hw-sw-co-design-for-deep-learning)
- Survey: *Wafer-scale Computing*. [arXiv:2310.09568](https://arxiv.org/abs/2310.09568)

## 2021 / 2024 — Memory wall, restated for transformers

Peak FLOPs have been growing faster than DRAM and interconnect bandwidth. Decoder models are memory-bound at serve time. HBM and NVLink are the industrial replies; they are products on [Nvidia]({{ '/timelines/nvidia/' | relative_url }}), not a new law.

- Gholami et al. *AI and Memory Wall*. [arXiv:2403.14123](https://arxiv.org/abs/2403.14123) · [IEEE Micro](https://doi.org/10.1109/MM.2024.3373763)

## What this page is not

A process-node log (7 nm, 5 nm, 3 nm) or a TSMC capacity brief. Export controls belong here only when a published training recipe depends on a specific stack. GPU SKUs and lab cheques stay on [Nvidia]({{ '/timelines/nvidia/' | relative_url }}).
