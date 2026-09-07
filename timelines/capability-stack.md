---
layout: default
title: Capability stack
permalink: /timelines/capability-stack/
---

# Capability stack

<p class="meta">2012–now · the spine every lab is reacting to</p>

## 2012-09 — AlexNet

ConvNets win ImageNet by a wide margin. Deep learning becomes the default bet.

- Paper: [ImageNet Classification with Deep Convolutional Neural Networks](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks)
- What followed: ResNets, then sequence models still stuck on recurrence.

## 2017-06 — Transformer

Self-attention replaces recurrence for sequence transduction. Training parallelizes across the sequence. This is the architecture every frontier model still uses.

- Paper: [Attention Is All You Need]({{ '/papers/1706.03762/' | relative_url }}) · [arXiv](https://arxiv.org/abs/1706.03762) · [alphaXiv](https://www.alphaxiv.org/abs/1706.03762)
- What followed: BERT, GPT, scaling laws.

## 2020-05 — GPT-3

175B parameters, in-context learning without fine-tuning. Scale starts looking like a method, not a hack.

- Paper: [Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165) · [alphaXiv](https://www.alphaxiv.org/abs/2005.14165)

## 2022-11 — ChatGPT

Instruct-tuned GPT-3.5 with a chat UI. First mass-market LLM product. Forces every lab onto a product clock.

- Lineage: [post-training]({{ '/timelines/post-training/' | relative_url }})

## 2023-03 — GPT-4 / Claude / Gemini race

Multimodal frontier models. Capability is no longer a single-lab story.

## 2024-09 — Test-time compute

o1-class models spend tokens on hidden reasoning. Inference-time search becomes a second scaling axis, next to pretraining.

- See also: [post-training]({{ '/timelines/post-training/' | relative_url }})
