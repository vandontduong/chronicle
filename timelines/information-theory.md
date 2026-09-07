---
layout: default
title: Information theory
permalink: /timelines/information-theory/
---

# Information theory

<p class="meta">Surprise as a number. The bit becomes the training loss, then a claim that modeling is compression.</p>

Architectures that *minimize* that loss live on [capability stack]({{ '/timelines/capability-stack/' | relative_url }}). The tokens being compressed live on [data]({{ '/timelines/data/' | relative_url }}). Perplexity as a scoreboard lives on [evals]({{ '/timelines/evals/' | relative_url }}). Bits per parameter as a ratio live on [efficiency]({{ '/timelines/efficiency/' | relative_url }}).

Not a coding-theory survey. A result lands here when it changed how models are trained or how labs talk about scale.

## 1948 — Shannon

A source has entropy. A channel has a capacity. The unit is the bit: expected surprise under a code. Everything later — cross-entropy training, perplexity, “language modeling is compression” — is this paper applied to a net.

- Shannon. *A Mathematical Theory of Communication*. Bell System Technical Journal 27 (1948). [PDF reprint](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf)

## 1951 — KL

Kullback and Leibler: the extra bits you spend when you code for the wrong distribution. Cross-entropy is entropy plus this gap. Training a classifier or an LM is shrinking KL to the data.

- Kullback and Leibler. *On Information and Sufficiency*. Ann. Math. Statist. 22 (1951). [Project Euclid](https://projecteuclid.org/journals/annals-of-mathematical-statistics/volume-22/issue-1/On-Information-and-Sufficiency/10.1214/aoms/1177729694.full)

## 1965 — Kolmogorov

Complexity of a string as the length of the shortest program that prints it. Algorithmic cousin of Shannon entropy. Solomonoff's induction sits next to it. The Hutter Prize later treats Wikipedia compression as a proxy for intelligence. Pointer, not a second spine: [RSI]({{ '/timelines/rsi/' | relative_url }}) for machines that rewrite the program.

- Kolmogorov. *Three approaches to the quantitative definition of information*. Problems of Information Transmission 1 (1965).

## 2003 — Cross-entropy as the LM loss

Bengio et al.: a neural net that assigns a probability to the next word, trained by maximum likelihood — i.e. minimum cross-entropy. After this, “better language model” means lower CE on held-out text. GPT-class training is this objective at scale.

- Bengio, Ducharme, Vincent, Jauvin. *A Neural Probabilistic Language Model*. JMLR 3 (2003). [PDF](https://www.jmlr.org/papers/volume3/bengio03a/bengio03a.pdf)

## 2006 — Compress Wikipedia

Hutter Prize: cash for the shortest program that reconstructs a Wikipedia dump. Compression as a public exam for “understanding.” Labs do not train frontier models to win it. They do quote bits-per-byte.

- [Hutter Prize](http://prize.hutter1.net/)

## 2018-07 — Contrastive bits in the representation

CPC / InfoNCE: score a true future against noise so the representation carries mutual information with what comes next. Contrastive pretraining (CLIP-class) is this loss with a different encoder pair. Not next-token CE; still Shannon's mutual information.

- van den Oord, Li, Vinyals. *Representation Learning with Contrastive Predictive Coding*. [arXiv:1807.03748](https://arxiv.org/abs/1807.03748)

## 2023-09 — Modeling is compression

Delétang et al.: an LM is a compressor. Arithmetic-code the data under the model's probabilities; better models yield shorter files. Makes explicit what CE training already was. Scaling-law plots on [capability stack]({{ '/timelines/capability-stack/' | relative_url }}) are the same claim with a different axis.

- Delétang et al. *Language Modeling Is Compression*. [arXiv:2309.10668](https://arxiv.org/abs/2309.10668)

## What this page is not

Turbo codes, LDPC, or a Cover & Thomas chapter list. Huffman and arithmetic coding only as the mechanism inside “modeling is compression,” not as a product log. VAEs / bits-back stay a pointer from [world models]({{ '/timelines/world-models/' | relative_url }}) unless the claim is the loss.
