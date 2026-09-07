---
layout: default
title: RSI
permalink: /timelines/rsi/
---

# Recursive self-improvement

<p class="meta">What is allowed to change: weights, prompts, code, environments, papers</p>

Most published “RSI” is an *outer* loop — search over artifacts a frozen model emits — not a net rewriting its own weights while it runs. SSI claims the inner version and has not published. Judge each beat by the **object that evolves**.

Agent products that do not rewrite themselves are [agents]({{ '/timelines/agents/' | relative_url }}). AlphaZero-style self-play with a known game is [DeepMind]({{ '/timelines/deepmind/' | relative_url }}). STaR-style bootstrap that *fine-tunes* on its own traces is [post-training]({{ '/timelines/post-training/' | relative_url }}) — cited there, not duplicated here.

## 2017-12 — Evolution instead of gradients

Genetic algorithms train deep policies at all. Not self-improvement of a deployed model; proof that the *search loop* can be non-SGD.

- Such et al. *Deep Neuroevolution*. [arXiv:1712.06567](https://arxiv.org/abs/1712.06567)

## 2019-01 — Environments that get harder

POET co-evolves agents and the worlds they inhabit. Open-endedness as a pair of loops, not one smarter net.

- Wang et al. *Paired Open-Ended Trailblazer (POET)*. [arXiv:1901.01753](https://arxiv.org/abs/1901.01753)
- Follow-up: *OMNI*. [arXiv:2306.01711](https://arxiv.org/abs/2306.01711)

## 2020-03 — Algorithms from scratch

AutoML-Zero evolves whole learning algorithms as programs. The artifact is code, not weights.

- Real et al. *AutoML-Zero*. [arXiv:2003.03384](https://arxiv.org/abs/2003.03384)

## 2023-09 — Prompts that breed prompts

Promptbreeder mutates task-prompts and the mutation-prompts themselves. Cheap, language-only self-reference.

- Fernando et al. *Promptbreeder*. [arXiv:2309.16797](https://arxiv.org/abs/2309.16797)

## 2024-08 — Search over agent designs

ADAS treats the agent's code (tools, control flow) as the genome. Meta-search, not a single trained policy.

- Hu, Lu, Clune. *Automated Design of Agentic Systems*. [arXiv:2408.08435](https://arxiv.org/abs/2408.08435)

## 2024-08 / 2025-04 — Papers that write papers

The AI Scientist runs idea → code → experiment → manuscript. v2 adds tree search. The evolving object is a research artifact. Reliability is the open problem, not the demo.

- Lu et al. *The AI Scientist*. [arXiv:2408.06292](https://arxiv.org/abs/2408.06292)
- Yamada et al. *The AI Scientist-v2*. [arXiv:2504.08066](https://arxiv.org/abs/2504.08066)

## 2025-05 — Darwin Gödel Machine

An agent rewrites its own code and keeps variants that do better on coding benchmarks. Closest public object to a Gödel machine that actually runs. Still an outer loop with frozen foundation weights.

- Zhang, Lu, et al. *Darwin Godel Machine*. [arXiv:2505.22954](https://arxiv.org/abs/2505.22954)

## 2025-09 / 2025-10 — Papers and contexts as agents

Paper2Agent turns a paper into an interactive agent. ACE evolves the *context* (playbooks, memories) instead of weights. Self-improvement as memory edit.

- Paper2Agent. [arXiv:2509.06917](https://arxiv.org/abs/2509.06917)
- *Agentic Context Engineering*. [arXiv:2510.04618](https://arxiv.org/abs/2510.04618)

## What is missing

A published system that modifies its *trained weights* in deployment and keeps the gains. SSI's charter points at that problem and does not show work. See [lab fission]({{ '/timelines/lab-fission/' | relative_url }}).
