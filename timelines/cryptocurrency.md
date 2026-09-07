---
layout: default
title: Cryptocurrency
permalink: /timelines/cryptocurrency/
---

# Cryptocurrency

<p class="meta">Hashing paid for the sheds. After the Merge, the sheds trained models.</p>

This page is the protocols that made *ugly megawatts and GPUs* a business. Who lent against those GPUs, and which miners became landlords, lives on [clouds]({{ '/timelines/clouds/' | relative_url }}). The cards themselves live on [Nvidia]({{ '/timelines/nvidia/' | relative_url }}).

Not a coin catalogue. A token is a beat only if it changed what hardware was bought or what power was energized.

## 2002 — Hashcash

Back: burn CPU on a SHA puzzle so email costs something. Proof-of-work as a meter. Bitcoin later points at this paper by name.

- Back. *Hashcash — A Denial of Service Counter-Measure*. [PDF](http://www.hashcash.org/papers/hashcash.pdf) (1 Aug 2002)

## 2008-10 / 2009-01 — Bitcoin

Nakamoto: timestamps, proof-of-work, a chain anyone can verify, no issuer. Product ships January 2009. The scarce object is *energy plus an ASIC path that does not exist yet* — early mining is CPU, then GPU.

- Nakamoto. *Bitcoin: A Peer-to-Peer Electronic Cash System*. [PDF](https://bitcoin.org/bitcoin.pdf) (31 Oct 2008)

## 2013-08 — Selfish mining

Eyal and Sirer: a minority pool can earn more than its hash share by withholding blocks. The security assumption in the white paper is not free. Protocol research, not a product.

- Eyal and Sirer. *Majority is not Enough: Bitcoin Mining is Vulnerable*. [arXiv:1311.0243](https://arxiv.org/abs/1311.0243)

## 2013–14 — Ethereum as a machine

Buterin: a chain that runs programs, not just transfers. Wood: the formal machine (yellow paper). The product that matters for this wiki is the *GPU-minable* proof-of-work (Ethash / Dagger-Hashimoto) that, for years, paid for consumer and datacenter Nvidia cards.

- Buterin. *Ethereum White Paper*. [ethereum.org](https://ethereum.org/whitepaper/) (2014)
- Wood. *Ethereum: A Secure Decentralised Generalised Transaction Ledger*. [Yellow Paper PDF](https://ethereum.github.io/yellowpaper/paper.pdf) (2014–)

## 2013–17 — ASICs take Bitcoin; GPUs take ETH

Bitcoin hash migrates onto application-specific silicon (Bitmain and peers). Ethereum stays on GPUs longer because the memory-hard puzzle resists cheap ASICs. That split is why a 2022 ETH miner still owned H100-adjacent buildings and cards, and a BTC miner owned substations and sheds. Hardware home: [Nvidia]({{ '/timelines/nvidia/' | relative_url }}).

## 2022-09-15 — The Merge

Ethereum turns off proof-of-work. GPU mining of ETH ends the same day. The cards and the interconnects do not. Operators who already had cheap power and a permitted building look for a new offtake. That landlord story — CoreWeave, Core Scientific, IREN, Crusoe — is [clouds]({{ '/timelines/clouds/' | relative_url }}).

- [ethereum.org — The Merge](https://ethereum.org/en/roadmap/merge/)

## 2024-04 — BTC halving

Subsidy drops. Hash margin compresses. More BTC sites try the same pivot the ETH miners already made: host someone else's training rack, or sell cloud themselves. Again the dollars are on [clouds]({{ '/timelines/clouds/' | relative_url }}).

## What is missing

A proof-of-*useful*-work that trains a frontier model on-chain and ships. Papers exist. The path that paid for Colossus-class power was ordinary PoW, then a lease.

## What this page is not

An L2 list, an NFT cycle, or a token price chart. Casper / Gasper internals only if they change who buys GPUs. Decentralized-training demos stay off until a lab actually pretrains that way.
