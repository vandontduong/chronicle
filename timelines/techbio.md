---
layout: default
title: Techbio
permalink: /timelines/techbio/
---

# Techbio

<p class="meta">AI × biology · structure, sequence, then a molecule in a patient</p>

Major beats only. A method counts when biologists actually use it; a company counts when a molecule leaves the slide deck. The lab culture that spent games-talent on folding: [DeepMind]({{ '/timelines/deepmind/' | relative_url }}). The short-read meter those models train on: [Illumina]({{ '/timelines/illumina/' | relative_url }}).

## 2018 — AlphaFold 1

DeepMind enters CASP13. Not solved, but the first time a net is in the conversation with physics-based folding. The 2020 Nature paper is the citable object; treat earlier blog posts as press.

- Senior et al. *Improved protein structure prediction using potentials from deep learning*. [Nature](https://www.nature.com/articles/s41586-019-1923-7) 577 (2020)

## 2018–21 — Proteins as language

Masked LMs on UniRef. Sequence → structure/function without an MSA at inference. The other spine, next to AlphaFold.

- Rives et al. *Biological structure and function emerge from scaling unsupervised learning to 250 million protein sequences*. [bioRxiv](https://www.biorxiv.org/content/10.1101/622803v4) · PNAS 2021. [Code](https://github.com/facebookresearch/esm)
- Lin et al. *Evolutionary-scale prediction of atomic-level protein structure with a language model* (ESM-2 / ESMFold). Science 2023. [arXiv:2204.06125](https://arxiv.org/abs/2204.06125) · [Science](https://www.science.org/doi/10.1126/science.ade2574)

## 2020-11 / 2021-07 — AlphaFold 2

CASP14. Then the Nature paper and the public database. First DeepMind result that changes a natural science. Every later design model filters against AF2.

- Jumper et al. *Highly accurate protein structure prediction with AlphaFold*. [Nature](https://www.nature.com/articles/s41586-021-03819-4) 596 (2021) · [DeepMind publication](https://deepmind.google/research/publications/45151/)
- [AlphaFold DB](https://alphafold.ebi.ac.uk/)
- Also on: [DeepMind]({{ '/timelines/deepmind/' | relative_url }})

## 2021 — RoseTTAFold, then Isomorphic

Baker lab net, released as the open counterpart. Same year Hassabis spins out **Isomorphic Labs** — AF as a drug company, not a paper.

- Baek et al. *Accurate prediction of protein structures and interactions using a three-track neural network*. Science 2021. [Science](https://www.science.org/doi/10.1126/science.abj8754)
- [Isomorphic Labs](https://www.isomorphiclabs.com/)

## 2023-07 — RFdiffusion

Denoise a protein backbone. Binders, motifs, symmetries. Design yield jumps; AF2 is the filter, diffusion is the generator.

- Watson et al. *De novo design of protein structure and function with RFdiffusion*. Nature 2023. [Nature](https://www.nature.com/articles/s41586-023-06415-8)

## 2023 — AlphaMissense

Classify missense variants at proteome scale. Structure model → clinical genetics, not just CASP trophies.

- Cheng et al. *Accurate proteome-wide missense variant effect prediction with AlphaMissense*. Science 2023. [Science](https://www.science.org/doi/10.1126/science.adg7492) · [code](https://github.com/google-deepmind/alphamissense)

## 2024-05 — AlphaFold 3

Diffusion over all atoms: proteins + ligands + nucleic acids + ions. Drug-like poses without a separate docking stack. Code delayed, then released.

- Abramson et al. *Accurate structure prediction of biomolecular interactions with AlphaFold 3*. Nature 2024. [Nature](https://www.nature.com/articles/s41586-024-07487-w) · [Google](https://blog.google/technology/ai/google-deepmind-isomorphic-alphafold-3-ai-model/)
- Inference code: [github.com/google-deepmind/alphafold3](https://github.com/google-deepmind/alphafold3)

## 2024-06 — ESM3

Sequence + structure + function in one generative LM. Synthesized GFP far from natural sequences (“500 million years”). Meta ESM team → **EvolutionaryScale**.

- Hayes et al. *Simulating 500 million years of evolution with a language model*. Science 2025. [bioRxiv](https://www.biorxiv.org/content/10.1101/2024.07.01.600583) · [Science](https://www.science.org/doi/10.1126/science.ads0018) · [EvolutionaryScale](https://www.evolutionaryscale.ai/blog/esm3-release)

## 2024-11 — Recursion × Exscientia

Phenomics shop buys the chemistry-AI shop. First large *platform merger* in public techbio. Pipeline later culled; the beat is the stack combining, not a single asset.

- [Pharmacological Reviews, 2025 landscape](https://pharmrev.aspetjournals.org/article/S0031-6997(25)07511-8/fulltext)

## 2025-06 — A molecule works in people

Insilico's TNIK inhibitor (rentosertib / ISM001-055) Phase IIa in IPF. Not “AI designed a pretty pose.” An end-to-end generative-chemistry origin with a randomized human efficacy signal.

- Xu et al. *A generative AI-discovered TNIK inhibitor for idiopathic pulmonary fibrosis: a randomized phase 2a trial*. [Nature Medicine](https://www.nature.com/articles/s41591-025-03743-2)

## 2025-06 — Boltz-2

Open co-folding plus affinity. MIT + Recursion. The AF3-class object other people can run, with a binding-energy head that claims FEP-like correlation at a fraction of the cost.

- Passaro et al. *Boltz-2: Towards Accurate and Efficient Binding Affinity Prediction*. [bioRxiv](https://www.biorxiv.org/content/10.1101/2025.06.14.659707v1)

## 2025–26 — Clinic, not CASP

Generate:Biomedicines GB-0895 into Phase 3 (anti-TSLP asthma). Insilico registers Phase 3. Absci, Iambic, Schrödinger assets in-human. Xaira (Baker-lineage, $1B) is the design-platform bet at fund scale.

The scoreboard leaves structure papers and becomes trial readouts. That is the point of this page.

## What this page is not

CRISPR as a tool (2012) is prior art, not an AI beat. Single-cell atlases and lab automation matter; they are infrastructure, listed only when they change a *model* or a *pipeline company*.
