---
layout: default
title: Disaggregated compute
permalink: /timelines/disaggregated-compute/
---

# Disaggregated compute

<p class="meta">Stop putting memory, compute, and the KV cache in one box. Split the phases that hate each other.</p>

The energy reason this matters lives on [integrated circuits]({{ '/timelines/integrated-circuits/' | relative_url }}). The fabric that makes a split cheap lives on [Nvidia]({{ '/timelines/nvidia/' | relative_url }}). Who owns the rack lives on [clouds]({{ '/timelines/clouds/' | relative_url }}). Serving kernels that stay on one GPU live on [efficiency]({{ '/timelines/efficiency/' | relative_url }}).

## 2018 — Disaggregate the machine

LegoOS treats CPU, memory, and storage as network-attached components with a split kernel. The paper is the OS version of a claim the industry later makes with CXL: the motherboard is a historical accident.

- Shan et al. *LegoOS: A Disseminated, Distributed OS for Hardware Resource Disaggregation*. OSDI 2018. [USENIX](https://www.usenix.org/conference/osdi18/presentation/shan)

## 2022–23 — CXL as a memory pool

Compute Express Link lets a host treat remote DRAM almost as local. Pond sizes a shared CXL pool for cloud VMs. TPP places pages across local and CXL tiers without rewriting the app. This is rack-scale disaggregation for *general* memory, before anyone splits a transformer.

- Li et al. *Pond: CXL-Based Memory Pooling Systems for Cloud Platforms*. [arXiv:2203.00241](https://arxiv.org/abs/2203.00241)
- Maruf et al. *TPP: Transparent Page Placement for CXL-Enabled Tiered-Memory*. [arXiv:2206.02878](https://arxiv.org/abs/2206.02878)
- [CXL Consortium](https://www.computeexpresslink.org/)

## 2023-11 — Splitwise

Prefill is compute-heavy. Decode is memory-bandwidth-heavy. Microsoft runs them on different machines and moves the KV cache over the backplane. Heterogeneous pools: H100-class for prompt, cheaper/slower parts for tokens. Power and cost, not just latency.

- Patel et al. *Splitwise: Efficient generative LLM inference using phase splitting*. [arXiv:2311.18677](https://arxiv.org/abs/2311.18677) · [Microsoft Research](https://www.microsoft.com/en-us/research/blog/splitwise-improves-gpu-usage-by-splitting-llm-inference-phases/)

## 2024-01 — DistServe

Same split, different objective: goodput under TTFT *and* TPOT. Prefill and decode get their own parallelism plan. Colocation is treated as interference, not a convenience.

- Zhong et al. *DistServe: Disaggregating Prefill and Decoding for Goodput-optimized Large Language Model Serving*. [arXiv:2401.09670](https://arxiv.org/abs/2401.09670)

## 2024-06 / 2025-02 — Mooncake

Moonshot's Kimi stack. Prefill and decode are separate clusters; the KV cache is a first-class pool on leftover DRAM and SSD, scheduled like a storage system. Production, not a prototype: FAST '25 best paper.

- Qin et al. *Mooncake: A KVCache-centric Disaggregated Architecture for LLM Serving*. [arXiv:2407.00079](https://arxiv.org/abs/2407.00079) · [FAST '25](https://www.usenix.org/conference/fast25/presentation/qin)
- [Mooncake project](https://kvcache-ai.github.io/Mooncake/)

## 2024-06 — MemServe

A memory pool API under both colocated and disaggregated serving, plus context caching. The beat is the *pool*, not another scheduler paper.

- Hu et al. *MemServe: Context Caching for Disaggregated LLM Serving with Elastic Memory Pool*. [arXiv:2406.17565](https://arxiv.org/abs/2406.17565)

## What this page is not

An NVLink SKU list. Scale-up inside one rack stays on [Nvidia]({{ '/timelines/nvidia/' | relative_url }}). Wafer-scale SRAM as an alternative to a pool stays on [Cerebras]({{ '/timelines/cerebras/' | relative_url }}). Later PD-Serve / DOPD variants land here only if they change the argument (new interconnect, new pool, or a production deployment).
