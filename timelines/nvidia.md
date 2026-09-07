---
layout: default
title: Nvidia
permalink: /timelines/nvidia/
---

# Nvidia

<p class="meta">The substrate under every other timeline · chips, interconnect, then checks into the labs</p>

This is not a GPU catalog. Beats are the things that changed *how* models get trained or served — plus the deals that lock that substrate to specific labs.

## 2006–14 — CUDA, then cuDNN

Programmable GPUs become a software platform. cuDNN makes convnets a product on that platform. AlexNet trains here; the stack timeline starts on Nvidia silicon whether it says so or not.

- [CUDA](https://developer.nvidia.com/cuda-zone)
- Chetlur et al. *cuDNN: Efficient Primitives for Deep Learning*. [arXiv:1410.0759](https://arxiv.org/abs/1410.0759)

## 2016 — DGX-1

First AI appliance: 8×P100, NVLink. OpenAI is the mythic first customer. The unit of sale shifts from a card to a *system*.

- [NVIDIA DGX-1](https://www.nvidia.com/en-us/data-center/dgx-1/)

## 2017 — Volta + Tensor Cores + NVLink 2

Mixed-precision matrix units. Training throughput jumps without a new algorithm. NVLink starts to make multi-GPU look like one device.

- Markidis et al. *NVIDIA Tensor Core Programmability*. [arXiv:1803.04014](https://arxiv.org/abs/1803.04014)
- [V100 / Volta](https://www.nvidia.com/en-us/data-center/v100/)

## 2020-04 — Mellanox closes ($6.9B)

InfiniBand + SmartNICs. Scale-*out* becomes an Nvidia product, not a partner SKU. The later “Nvidia is a networking company” line starts here.

- Deal announced 2019, closed Apr 2020 after CFIUS/China review. [NVIDIA on Mellanox](https://nvidianews.nvidia.com/news/nvidia-completes-acquisition-of-mellanox-creating-major-force-driving-next-gen-data-centers)

## 2020–22 — Arm attempt fails

$40B+ bid for Arm. Killed by US/UK/EU antitrust (2022). The road not taken: own the CPU ISA too.

- [Forbes on the collapse](https://www.forbes.com/sites/kevindowd/2022/02/08/nvidias-arm-acquisition-is-the-latest-chip-mega-deal-to-crumble/)

## 2022 — Hopper / H100 + Transformer Engine

FP8 paths aimed at transformers. The chip the GPT-4 / Claude / Gemini wave actually rented.

- [Transformer Engine](https://github.com/NVIDIA/TransformerEngine)
- Micikevicius et al. on mixed precision (earlier stack): [arXiv:1710.03740](https://arxiv.org/abs/1710.03740)

## 2022 — FlashAttention (not an Nvidia paper)

Dao et al. make attention IO-aware on *this* hardware. Belongs on [efficiency]({{ '/timelines/efficiency/' | relative_url }}); listed here because the kernel assumes Tensor Cores + HBM.

- [arXiv:2205.14135](https://arxiv.org/abs/2205.14135)

## 2024 — Run:ai (~$700M)

GPU orchestration on Kubernetes. After this, Nvidia sells the scheduler that sits between the customer and the GPUs it already sold them.

- [NVIDIA Run:ai](https://www.nvidia.com/en-us/software/run-ai/)

## 2024–25 — Blackwell, then NVL72

B200 / GB200. 72 GPUs as one NVLink domain. The scale-*up* story (inside the rack) becomes as important as scale-out.

- [GB200 NVL72](https://www.nvidia.com/en-us/data-center/gb200-nvl72/)
- GTC sessions on NVL72 inference (e.g. [S72503](https://www.nvidia.com/en-us/on-demand/session/gtc25-s72503/))

## 2025 — Groq: license + hire, not a clean buy

Inference LPU tech and talent (Jonathan Ross). Structured to dodge a full acquisition review. Later racks list Groq LPUs next to Vera Rubin.

- Coverage of the license/hire structure and the later Senate letter: see 2026 antitrust notes in [TechArena](https://techarena.ai/content/from-ai-land-grab-to-full-stack-targeting-the-orchestration-layer)

## 2025-09 / 2026-02 — OpenAI: LOI then a smaller cheque

Letter of intent: up to $100B and 10 GW of Nvidia systems. What closed: about **$30B** equity into OpenAI’s 2026 round, not the full $100B. Circular-financing debate starts here: invest in the lab that buys the chips.

- [Fortune on the $100B headline](https://fortune.com/2025/09/28/nvidia-openai-circular-financing-ai-bubble/)
- [Reuters cluster of infra deals](https://www.reuters.com/business/autos-transportation/companies-pouring-billions-advance-ai-infrastructure-2026-07-22/)

## 2025-11 — Anthropic, with Microsoft

Nvidia up to $10B, Microsoft $5B; Anthropic pledges large Azure / Grace-Blackwell / Vera Rubin spend.

- Same Reuters / funding-tracker roundups as above.

## 2024–26 — CoreWeave and the other neoclouds

Equity + a $6.3B take-or-pay on unsold cloud capacity. The pattern: fund the landlord, buy leftover rack-hours, book GPU revenue either way.

- [Bloomberg circular-deals guide](https://www.bloomberg.com/graphics/2026-ai-circular-deals/)

## 2026-03 — Thinking Machines raise

Nvidia among backers of Murati’s lab. Ties this page to [lab fission]({{ '/timelines/lab-fission/' | relative_url }}).

## 2026-07 — SSI × Vera Rubin (~$5B)

Compute partnership plus investment. Sutskever: research “worthy of scaling.” First time SSI is visible as a *customer*, still not as a paper.

- [TechCrunch](https://techcrunch.com/2026/07/27/ilya-sutskevers-safe-superintelligence-partners-with-nvidia-to-scale-its-ai-research/)
- [lab fission — SSI]({{ '/timelines/lab-fission/' | relative_url }})

## 2026 — Vera Rubin NVL72

Next rack: Rubin GPUs, Vera CPUs, NVLink 6, optional Groq LPUs in the GTC story. Annual cadence now includes the *system*, not just the die.

- GTC 2026 keynote cycle (Huang); architecture tables in trade writeups e.g. [GDEP GTC 2026 notes](https://www.gdep.co.jp/tech_report/gtc2026_tecnical_20260326/)

## Acquisition / deal list (short)

| Year | What | Why it matters |
|---|---|---|
| 2020 | Mellanox $6.9B | Own scale-out fabric |
| 2022 | Arm ~$40B **failed** | ISA control blocked |
| 2022 | Bright Computing, Excelero | Cluster + storage software |
| 2024 | Run:ai ~$700M | GPU scheduler |
| 2024–25 | Deci, LeptonAI | Compile / GPU cloud software; Lepton later messy |
| 2025 | Groq license + talent | Inference path without a full buy |
| 2025–26 | OpenAI, Anthropic, CoreWeave, xAI/SpaceXAI, SSI, Thinking Machines | Demand locked with equity |

Also on: [efficiency]({{ '/timelines/efficiency/' | relative_url }}), [lab fission]({{ '/timelines/lab-fission/' | relative_url }}), [capability stack]({{ '/timelines/capability-stack/' | relative_url }}).
