---
layout: default
title: Illumina
permalink: /timelines/illumina/
---

# Illumina

<p class="meta">The short-read meter. Almost every later AI×bio model trains on data this company sold.</p>

The franchise is sequencing-by-synthesis instruments and the reagents that run them. AI here is interpretation on top of that meter (SpliceAI, PrimateAI-3D, DRAGEN on GPUs) plus multiomics M&A after GRAIL blew up. Structure models live on [techbio]({{ '/timelines/techbio/' | relative_url }}).

## 2007–08 — Solexa becomes the stack

Illumina buys Solexa. Bentley et al. then show a whole human genome on reversible-terminator chemistry — massively parallel short reads. That paper is the industrial standard the field still runs, not a one-off demo.

- Bentley et al. *Accurate whole human genome sequencing using reversible terminator chemistry*. Nature 456:53–59 (2008). [Nature](https://www.nature.com/articles/nature07517)

Roche later tries a hostile takeout (~$6.8B, 2012) and fails. The franchise stays independent.

## 2019 / 2023 — Models on the reads

SpliceAI (Illumina) predicts splice-altering variants from sequence alone. PrimateAI-3D uses tolerated primate missense variation plus 3D structure to score human pathogenicity — the sequencing company shipping a structure-aware net, years after AlphaFold.

- Jaganathan et al. *Predicting splicing from primary sequence with deep learning*. Cell 176 (2019). [doi:10.1016/j.cell.2018.12.015](https://doi.org/10.1016/j.cell.2018.12.015)
- Gao et al. *The landscape of tolerated genetic variation in humans and primates* (PrimateAI-3D). Science 2023. [Science](https://www.science.org/doi/10.1126/science.abn8197)

## 2020-09 / 2021-08 — GRAIL in

Illumina agrees ~$8B to buy back GRAIL, the liquid-biopsy spinout it helped start. Closes over FTC/EU objections (gun-jumping). Thesis: own the cancer-test that consumes the genomes. It is the wrong deal for a tools company — regulators, Icahn, a CEO exit.

- [TechCrunch on the 2020 bid](https://techcrunch.com/2020/09/21/illumina-grail/)

## 2022-09 — NovaSeq X

XLEAP-SBS chemistry, denser flow cells, onboard DRAGEN. Claim: >20k genomes/year on one box, lower plastic, no dry ice. This is the current production workhorse, not a paper.

- [Illumina launch](https://www.prnewswire.com/news-releases/illumina-unveils-revolutionary-novaseq-x-series-to-rapidly-accelerate-genomic-discoveries-and-improve-human-health-301636881.html)

## 2024-06 — GRAIL out

EU restorative measures force an unwind. Spin-off completes 24 Jun 2024; GRAIL trades as GRAL. Illumina keeps 14.5%. The beat is not the test. It is that a tools firm cannot buy the downstream assay without becoming a defendant.

- [Illumina completes the divestiture](https://www.illumina.com/company/news-center/press-releases/2024/d2e2aec7-563a-4301-9d60-db56ea067bfb.html)
- [Commission approved the unwind plan, Apr 2024](https://ec.europa.eu/commission/presscorner/detail/en/ip_24_1964)

## 2024-07 — Fluent BioSciences

Cash deal for PIPseq single-cell partitioning. After GRAIL, M&A is *inputs to the sequencer* (cells, proteins), not a closed clinical franchise.

- [Illumina / Fluent](https://www.prnewswire.com/news-releases/illumina-acquires-fluent-biosciences-to-accelerate-single-cell-analysis-and-discovery-to-a-broader-customer-base-302192516.html)

## 2025-01 — Nvidia

JPM week: DRAGEN onto Nvidia GPUs inside Connected Analytics; joint work on biology foundation models. Illumina already had SpliceAI / PrimateAI / Emedgene. This is distribution onto the same accelerators the labs use for ESM and AF.

- [Illumina](https://www.prnewswire.com/news-releases/illumina-and-nvidia-collaborate-to-decode-biology-and-propel-precision-health-302348920.html)
- [Nvidia](https://nvidianews.nvidia.com/news/nvidia-partners-with-industry-leaders-to-advance-genomics-drug-discovery-and-healthcare)
- Also on: [nvidia]({{ '/timelines/nvidia/' | relative_url }}), [techbio]({{ '/timelines/techbio/' | relative_url }})

## 2026-01 — SomaLogic

Buys SomaLogic (and related assets) from Standard BioTools: $350M cash at close + milestones/royalties. SomaScan proteomics on the NGS rail. Multiomics as the stated strategy after the GRAIL scar.

- [Illumina completes the acquisition](https://www.illumina.com/company/news-center/press-releases/2026/b7bf54f5-b534-47b4-a629-02ade3b10178.html)
- [Hub](https://www.illumina.com/company/news-center/somalogic-acquisition.html)

## 2026 — The meter still compounds

Feb: NovaSeq X roadmap (higher output, Q70 talk). Roche ships Axelios as a long-read / nanopore-ish assault on the same labs. Illumina's share of short-read NGS remains the default prior for every foundation model that starts from a FASTQ.

## What this page is not

A $1,000-genome price chart. Cost only matters here when a new chemistry or a forced deal changes who owns the sample.
