---
layout: default
title: Techbio
permalink: /timelines/techbio/
---

# Techbio

<p class="meta">AI × biology · structure, sequence, then a molecule in a patient</p>

Major beats only. A method counts when biologists actually use it; a company counts when a molecule leaves the slide deck.

## 2018 — AlphaFold 1

DeepMind enters CASP. Not solved, but the first time a net is in the conversation with physics-based folding.

- Senior et al. *Improved protein structure prediction using potentials from deep learning*. Nature 2018 / [DeepMind](https://deepmind.google/discover/blog/alphafold-using-ai-for-scientific-discovery/)

## 2018–21 — Proteins as language

Masked LMs on UniRef. Sequence → structure/function without an MSA at inference. The other spine, next to AlphaFold.

- Rives et al. *Biological structure and function emerge from scaling unsupervised learning to 250 million protein sequences*. [bioRxiv 2019](https://www.biorxiv.org/content/10.1101/622803v4) · PNAS 2021 · [arXiv:2010.xxxxx via ESM](https://github.com/facebookresearch/esm)
- ESM-1b / ESM-2 lineage. [ESM-2](https://github.com/facebookresearch/esm) · Lin et al. *Evolutionary-scale prediction of atomic-level protein structure with a language model*. Science 2023.

## 2020-11 / 2021-07 — AlphaFold 2

CASP14. Then the Nature paper and the public database. First DeepMind result that changes a natural science. Every later design model filters against AF2.

- Jumper et al. *Highly accurate protein structure prediction with AlphaFold*. Nature 596 (2021). [DeepMind blog](https://deepmind.google/discover/blog/alphafold-a-solution-to-a-50-year-old-grand-challenge-in-biology/)
- [AlphaFold DB](https://alphafold.ebi.ac.uk/)
- Also on: [DeepMind]({{ '/timelines/deepmind/' | relative_url }})

## 2021 — RoseTTAFold, then Isomorphic

Baker lab's two-track net, released as the open counterpart. Same year Hassabis spins out **Isomorphic Labs** — AF as a drug company, not a paper.

- Baek et al. *Accurate prediction of protein structures and interactions using a three-track neural network*. Science 2021. [arXiv:2110.xxxxx / Science](https://www.science.org/doi/10.1126/science.abj8754)
- [Isomorphic Labs](https://www.isomorphiclabs.com/)

## 2023-07 — RFdiffusion

Denoise a protein backbone. Binders, motifs, symmetries. Design yield jumps; AF2 is the filter, diffusion is the generator.

- Watson et al. *De novo design of protein structure and function with RFdiffusion*. Nature 2023. [PDF / Nature](https://www.nature.com/articles/s41586-023-06415-8)

## 2023 — AlphaMissense

Classify missense variants at proteome scale. Structure model → clinical genetics, not just CASP trophies.

- Cheng et al. *Accurate proteome-wide missense variant effect prediction with AlphaMissense*. Science 2023.

## 2024-05 — AlphaFold 3

Diffusion over all atoms: proteins + ligands + nucleic acids + ions. Drug-like poses without a separate docking stack. Code delayed, then released.

- Abramson et al. *Accurate structure prediction of biomolecular interactions with AlphaFold 3*. Nature 2024. [Nature](https://www.nature.com/articles/s41586-024-07487-w) · [Google](https://blog.google/technology/ai/google-deepmind-isomorphic-alphafold-3-ai-model/) · [Isomorphic](https://www.isomorphiclabs.com/articles/rational-drug-design-with-alphafold-3)
- Inference code: [github.com/google-deepmind/alphafold3](https://github.com/google-deepmind/alphafold3)

## 2024-06 — ESM3

Sequence + structure + function in one generative LM. Synthesized GFP far from natural sequences (“500 million years”). Meta ESM team → **EvolutionaryScale**.

- Hayes et al. *Simulating 500 million years of evolution with a language model*. Science 2025. [bioRxiv](https://www.biorxiv.org/content/10.1101/2024.07.01.600583) · [EvolutionaryScale](https://www.evolutionaryscale.ai/blog/esm3-release)

## 2024-11 — Recursion × Exscientia

Phenomics shop buys the chemistry-AI shop. First large *platform merger* in public techbio. Pipeline later culled; the beat is the stack combining, not a single asset.

- Coverage in reviews of 2025 platforms: [Pharmacological Reviews](https://pharmrev.aspetjournals.org/article/S0031-6997(25)07511-8/fulltext)

## 2025 — A molecule works in people

Insilico's TNIK inhibitor (rentosertib / ISM001-055) Phase IIa in IPF, *Nature Medicine*. Not “AI designed a pretty pose.” An end-to-end AI-originated small molecule with a human efficacy signal.

- Clinical surveys: [IntuitionLabs 2026 pipeline](https://intuitionlabs.ai/articles/ai-discovered-drugs-clinical-trials-2026)

## 2025 — Boltz-2

Open co-folding + affinity. MIT + Recursion + Nvidia. The AF3-class object other people can actually run.

- Listed in 2025 platform reviews above; model card / GitHub via Recursion–MIT release.

## 2025–26 — Clinic, not CASP

Generate:Biomedicines GB-0895 into Phase 3 (anti-TSLP asthma). Insilico registers Phase 3. Absci, Iambic, Schrödinger assets in-human. Xaira (Baker-lineage, $1B) is the design-platform bet at fund scale.

The scoreboard leaves structure papers and becomes trial readouts. That is the point of this page.

## What this page is not

CRISPR as a tool (2012) is prior art, not an AI beat. Single-cell atlases and lab automation matter; they are infrastructure, listed only when they change a *model* or a *pipeline company*.

Also on: [DeepMind]({{ '/timelines/deepmind/' | relative_url }}), [lab fission]({{ '/timelines/lab-fission/' | relative_url }}) (Isomorphic), [nvidia]({{ '/timelines/nvidia/' | relative_url }}) (bio cluster spend).
