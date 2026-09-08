---
layout: default
title: Nvidia
permalink: /timelines/nvidia/
---

# Nvidia

<p class="meta">The substrate under every other timeline — chips, interconnect, then checks into the labs.</p>

This is not a GPU catalog. Beats are the things that changed *how* models get trained or served — plus the deals that lock that substrate to specific labs. Who prints the die: [TSMC]({{ '/timelines/tsmc/' | relative_url }}). Who prints the memory cube: [HBM]({{ '/timelines/hbm/' | relative_url }}). Capability per flop: [efficiency]({{ '/timelines/efficiency/' | relative_url }}). Who lent against the chip, including the 2026 manager platforms: [clouds]({{ '/timelines/clouds/' | relative_url }}).

## 1993 / 1999 — A graphics company, then a GPU

Founded 1993. GeForce 256 (1999) is sold as a “GPU” — transform and lighting on the card, not the CPU. The later AI story is a second use of the same programmable pipeline. TSMC is already the fab.

- [NVIDIA company](https://www.nvidia.com/en-us/about-nvidia/)

## 2006-11 — CUDA on G80

GeForce 8800 / G80 ships with a C toolchain. The card is no longer only a graphics API. This is the lock-in: models that train on CUDA stay on CUDA. AlexNet (2012) runs here whether the paper names the vendor or not.

- [CUDA](https://developer.nvidia.com/cuda-zone)
- Also on: [capability stack]({{ '/timelines/capability-stack/' | relative_url }}), [integrated circuits]({{ '/timelines/integrated-circuits/' | relative_url }})

## 2007–12 — Tesla as an HPC SKU, then Titan

“Tesla” is the brand for compute boards without a display. Oak Ridge Titan (2012) puts Kepler in a top supercomputer. Scientific computing pays for the plants before transformers do.

## 2014 — cuDNN

Convolution primitives as a library. Convnets become a product on CUDA instead of a research kernel. Every later framework (Caffe, then TensorFlow, then PyTorch) sits on this layer.

- Chetlur et al. *cuDNN: Efficient Primitives for Deep Learning*. [arXiv:1410.0759](https://arxiv.org/abs/1410.0759)

## 2016 — Pascal, NVLink, HBM2, DGX-1

P100 puts HBM2 and the first NVLink on a training board. Samsung supplied that generation. DGX-1 (8×P100) is the first AI *appliance*. OpenAI is the mythic first customer. The unit of sale shifts from a card to a system. Later HBM3/3E/4 quals: [HBM]({{ '/timelines/hbm/' | relative_url }}).

- [NVIDIA DGX-1](https://www.nvidia.com/en-us/data-center/dgx-1/)

## 2017 — Volta + Tensor Cores

Mixed-precision matrix units on V100. Training throughput jumps without a new algorithm. NVLink 2 starts to make multi-GPU look like one device.

- Markidis et al. *NVIDIA Tensor Core Programmability*. [arXiv:1803.04014](https://arxiv.org/abs/1803.04014)
- Micikevicius et al. *Mixed Precision Training*. [arXiv:1710.03740](https://arxiv.org/abs/1710.03740)
- [V100 / Volta](https://www.nvidia.com/en-us/data-center/v100/)

## 2020-04 — Mellanox closes ($6.9B)

Announced 2019. InfiniBand + SmartNICs. Scale-*out* becomes an Nvidia product, not a partner SKU.

- [NVIDIA completes Mellanox](https://nvidianews.nvidia.com/news/nvidia-completes-acquisition-of-mellanox-creating-major-force-driving-next-gen-data-centers)

## 2020-05 — Ampere A100 and MIG

A100 unifies training and inference on one die (TF32, sparsity). Multi-Instance GPU slices one card into as many as seven. Clouds can sell *fractions* of a GPU. DGX A100 is the box the 2020–22 lab wave actually bought.

- [Newsroom: A100 in production](https://nvidianews.nvidia.com/news/nvidias-new-ampere-data-center-gpu-in-full-production)
- [Developer blog](https://developer.nvidia.com/blog/nvidia-ampere-architecture-in-depth/)

## 2020–22 — Arm attempt fails

$40B+ bid for Arm. Killed by US/UK/EU antitrust (2022). The road not taken: own the CPU ISA too.

- [Forbes on the collapse](https://www.forbes.com/sites/kevindowd/2022/02/08/nvidias-arm-acquisition-is-the-latest-chip-mega-deal-to-crumble/)

## 2022 — Hopper / H100 + Transformer Engine

FP8 paths aimed at transformers. The chip the GPT-4 / Claude / Gemini wave rented. Transformer Engine is the software that makes FP8 a default. Memory on the package is SK Hynix HBM3 — [HBM]({{ '/timelines/hbm/' | relative_url }}).

- [Transformer Engine](https://github.com/NVIDIA/TransformerEngine)
- [Hopper architecture in-depth](https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/)

## 2022 — FlashAttention (not an Nvidia paper)

Dao et al. make attention IO-aware on *this* hardware. Belongs on [efficiency]({{ '/timelines/efficiency/' | relative_url }}); listed here because the kernel assumes Tensor Cores + HBM.

- Dao et al. *FlashAttention*. [arXiv:2205.14135](https://arxiv.org/abs/2205.14135)

## 2023 — Grace, then GH200

An Nvidia Arm CPU, NVLink-C2C to a Hopper GPU, coherent memory. Later GB200 pairs Grace with Blackwell the same way.

- [Grace CPU](https://www.nvidia.com/en-us/data-center/grace-cpu/)

## 2024 — Run:ai (~$700M)

GPU orchestration on Kubernetes. After this, Nvidia sells the scheduler that sits between the customer and the GPUs it already sold them.

- [NVIDIA Run:ai](https://www.nvidia.com/en-us/software/run-ai/)

## 2024–25 — Blackwell, then NVL72

B200 / GB200. 72 GPUs as one NVLink domain. CoWoS packaging, not litho, is often the scarce step — [TSMC]({{ '/timelines/tsmc/' | relative_url }}). HBM3E quals: [HBM]({{ '/timelines/hbm/' | relative_url }}).

- [GB200 NVL72](https://www.nvidia.com/en-us/data-center/gb200-nvl72/)
- GTC sessions on NVL72 inference (e.g. [S72503](https://www.nvidia.com/en-us/on-demand/session/gtc25-s72503/))

## 2025 — Groq: license + hire, not a clean buy

Inference LPU tech and talent (Jonathan Ross). Structured to dodge a full acquisition review.

- Coverage of the license/hire structure: [TechArena](https://techarena.ai/content/from-ai-land-grab-to-full-stack-targeting-the-orchestration-layer)

## 2025-01 — Cosmos as a world-model SKU

Physical-AI foundation models, open weights, sold next to the robot stack. The paper lives on [world models]({{ '/timelines/world-models/' | relative_url }}). The beat here is: Nvidia now ships *weights*, not only silicon.

- NVIDIA Cosmos. [arXiv:2501.03575](https://arxiv.org/abs/2501.03575)

## 2025-09 / 2026-02 — OpenAI: LOI then a smaller cheque

Letter of intent: up to $100B and 10 GW of Nvidia systems. What closed: about **$30B** equity into OpenAI’s 2026 round, not the full $100B.

- [Fortune on the $100B headline](https://fortune.com/2025/09/28/nvidia-openai-circular-financing-ai-bubble/)
- [Reuters cluster of infra deals](https://www.reuters.com/business/autos-transportation/companies-pouring-billions-advance-ai-infrastructure-2026-07-22/)

## 2025-11 — Anthropic, with Microsoft

Nvidia up to $10B, Microsoft $5B; Anthropic pledges large Azure / Grace-Blackwell / Vera Rubin spend.

- Same Reuters / funding-tracker roundups as above.

## 2024–26 — CoreWeave and the other neoclouds

Equity + a $6.3B take-or-pay on unsold cloud capacity. Fund the landlord, buy leftover rack-hours. Landlord math: [clouds]({{ '/timelines/clouds/' | relative_url }}).

- [Bloomberg circular-deals guide](https://www.bloomberg.com/graphics/2026-ai-circular-deals/)

## 2026-03 — Thinking Machines raise

Nvidia among backers of Murati’s lab. Ties this page to [lab fission]({{ '/timelines/lab-fission/' | relative_url }}).

## 2026-06 — SK Hynix memory partnership

Multi-year co-development against the Vera Rubin roadmap. Home: [HBM]({{ '/timelines/hbm/' | relative_url }}).

- [SK Hynix](https://news.skhynix.com/en/multi-year-tech-partnership-with-nvidia/)

## 2026-07 — SSI × Vera Rubin (~$5B)

Compute partnership plus investment. First time SSI is visible as a *customer*, still not as a paper.

- [TechCrunch](https://techcrunch.com/2026/07/27/ilya-sutskevers-safe-superintelligence-partners-with-nvidia-to-scale-its-ai-research/)
- [lab fission — SSI]({{ '/timelines/lab-fission/' | relative_url }})

## 2026-08-10 — Financing platforms, not a $500B cheque

MOUs with Apollo, BlackRock, Blackstone, Brookfield, Goldman Sachs, and KKR to stand up independent platforms *designed to mobilize* over $500B of third-party capital over time. Residual-value support on some deals, up to 25%. Structure, what is not booked, and the CoreWeave lineage: [clouds]({{ '/timelines/clouds/' | relative_url }}).

- [Nvidia blog](https://blogs.nvidia.com/blog/nvidia-ai-factory-compute/)

## 2026 — Vera Rubin NVL72

Next rack: Rubin GPUs, Vera CPUs, NVLink 6. Starmind payload talk sits on [SpaceX]({{ '/timelines/spacex/' | relative_url }}). HBM4 / 4E: [HBM]({{ '/timelines/hbm/' | relative_url }}).

- GTC 2026 keynote cycle (Huang); architecture tables in trade writeups e.g. [GDEP GTC 2026 notes](https://www.gdep.co.jp/tech_report/gtc2026_tecnical_20260326/)

## 2026-09 — Hugging Face, agreed not closed

3 Sep 2026: Nvidia agrees to buy Hugging Face for **$12.93B**. Close aimed at H1 2027. The Hub stays multi-cloud per Huang. Mixes stay on [data]({{ '/timelines/data/' | relative_url }}).

- Huang. [NVIDIA to Acquire Hugging Face](https://blogs.nvidia.com/blog/nvidia-to-acquire-hugging-face/)
- [NYT](https://www.nytimes.com/2026/09/03/technology/nvidia-hugging-face.html)
- [TechCrunch](https://techcrunch.com/2026/09/03/nvidia-confirms-it-will-buy-hugging-face-for-12-9-billion/)

## Acquisition / deal list (short)

| Year | What | Why it matters |
|---|---|---|
| 2020 | Mellanox $6.9B | Own scale-out fabric |
| 2022 | Arm ~$40B **failed** | ISA control blocked |
| 2022 | Bright Computing, Excelero | Cluster + storage software |
| 2024 | Run:ai ~$700M | GPU scheduler |
| 2024–25 | Deci, LeptonAI | Compile / GPU cloud software |
| 2025 | Groq license + talent | Inference path without a full buy |
| 2026-06 | SK Hynix multi-year memory | Cube supply for Rubin-class parts |
| 2025–26 | OpenAI, Anthropic, CoreWeave, xAI/SpaceX, SSI, Thinking Machines | Demand locked with equity |
| 2026-08 | Apollo / BlackRock / Blackstone / Brookfield / GS / KKR MOUs | Compute financing platforms; dollars on [clouds]({{ '/timelines/clouds/' | relative_url }}) |
| 2026-09 | Hugging Face **$12.93B agreed** | Own the open-weight Hub; close 2027 |

## What this page is not

A list of GeForce or data-center SKUs. Ada, RTX, and gaming attach only if they change the training stack. Cosmos the *simulator paper* lives on [world models]({{ '/timelines/world-models/' | relative_url }}). HBM vendor quals live on [HBM]({{ '/timelines/hbm/' | relative_url }}). GPU-backed debt and the $500B *platform* live on [clouds]({{ '/timelines/clouds/' | relative_url }}).
