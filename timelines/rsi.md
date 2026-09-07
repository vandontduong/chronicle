---
layout: default
title: RSI
permalink: /timelines/rsi/
---

# Recursive self-improvement

<p class="meta">What is allowed to change: weights, prompts, code, environments, papers</p>

Most published “RSI” is an *outer* loop — search over artifacts a frozen model emits — not a net rewriting its own weights while it runs. SSI claims the inner version and has not published. Judge each beat by the **object that evolves**.

Agent products that do not rewrite themselves are [agents]({{ '/timelines/agents/' | relative_url }}). AlphaZero-style self-play with a known game is [DeepMind]({{ '/timelines/deepmind/' | relative_url }}). STaR-style bootstrap that *fine-tunes* on its own traces is [post-training]({{ '/timelines/post-training/' | relative_url }}) — cited there, not duplicated here.

## 1965 — The explosion argument

Good: an ultraintelligent machine can design a better machine; that is a singularity of intelligence. The paper is a speculation, not a method. Every later “RSI” claim is measured against this sentence.

- Good. *Speculations Concerning the First Ultraintelligent Machine*. Advances in Computers, 1965. [DOI](https://doi.org/10.1016/S0065-2458(08)60418-0)

## 2003-09 — A machine that rewrites itself if it can prove it should

Schmidhuber's Gödel machine: search for a proof that a self-rewrite raises expected utility, then execute the rewrite. The object is the *entire program*, including the proof searcher. No practical implementation. Namesake for later “Gödel Agent” / “Darwin Gödel Machine” papers that drop the proof requirement.

- Schmidhuber. *Goedel Machines*. [arXiv:cs/0309048](https://arxiv.org/abs/cs/0309048)

## 2017-12 — Evolution instead of gradients

Genetic algorithms train deep policies at all. Not self-improvement of a deployed model; proof that the *search loop* can be non-SGD.

- Such et al. *Deep Neuroevolution*. [arXiv:1712.06567](https://arxiv.org/abs/1712.06567)

## 2019 — Environments, and a program to grow the grower

POET co-evolves agents and the worlds they inhabit. Clune's AI-GAs paper states the research program the rest of this page is still inside: meta-learn architectures, meta-learn the learner, generate the environments.

- Wang et al. *Paired Open-Ended Trailblazer (POET)*. [arXiv:1901.01753](https://arxiv.org/abs/1901.01753)
- Clune. *AI-GAs: AI-generating algorithms*. [arXiv:1905.10985](https://arxiv.org/abs/1905.10985)
- Follow-up environment search: *OMNI*. [arXiv:2306.01711](https://arxiv.org/abs/2306.01711)

## 2020-03 — Algorithms from scratch

AutoML-Zero evolves whole learning algorithms as programs. The artifact is code, not weights.

- Real et al. *AutoML-Zero*. [arXiv:2003.03384](https://arxiv.org/abs/2003.03384)

## 2023-05 — A skill library that accumulates

Voyager keeps executable code skills in Minecraft and writes new ones. Frozen GPT-4. The evolving object is the library, not the net.

- Wang et al. *Voyager*. [arXiv:2305.16291](https://arxiv.org/abs/2305.16291)

## 2023-09 / 2023-10 — Prompts and improvers that breed

Promptbreeder mutates task-prompts and the mutation-prompts themselves. STOP takes a seed *improver* (code that calls a frozen LM) and runs it on itself. The authors are explicit: the weights do not change; this is RSI of scaffolding.

- Fernando et al. *Promptbreeder*. [arXiv:2309.16797](https://arxiv.org/abs/2309.16797)
- Zelikman et al. *Self-Taught Optimizer (STOP)*. [arXiv:2310.02304](https://arxiv.org/abs/2310.02304)

## 2023-12 / 2025-06 — Search in function space, then whole files

FunSearch pairs a frozen LM with an evaluator and evolves programs until they beat the literature (cap sets). AlphaEvolve is the same loop on diffs across a codebase: matrix-multiply records, datacenter scheduling, a speedup of the model that writes the diffs. The object is still code. The claim that matters is a *verified* better artifact, not a higher chatbot score.

- Romera-Paredes et al. *Mathematical discoveries from program search with large language models*. Nature 2023. [paper](https://www.nature.com/articles/s41586-023-06924-6) · [DeepMind](https://deepmind.google/blog/funsearch-making-new-discoveries-in-mathematical-sciences-using-large-language-models/)
- Novikov et al. *AlphaEvolve*. [arXiv:2506.13131](https://arxiv.org/abs/2506.13131)

## 2024-08 — Search over agent designs

ADAS treats the agent's code (tools, control flow) as the genome. Meta-search, not a single trained policy.

- Hu, Lu, Clune. *Automated Design of Agentic Systems*. [arXiv:2408.08435](https://arxiv.org/abs/2408.08435)

## 2024-08 / 2025-04 — Papers that write papers

The AI Scientist runs idea → code → experiment → manuscript. v2 adds tree search. The evolving object is a research artifact. Reliability is the open problem, not the demo.

- Lu et al. *The AI Scientist*. [arXiv:2408.06292](https://arxiv.org/abs/2408.06292)
- Yamada et al. *The AI Scientist-v2*. [arXiv:2504.08066](https://arxiv.org/abs/2504.08066)

## 2024-10 / 2025-05 — Gödel in the name, no proof obligation

Gödel Agent lets an LM rewrite its own policy and the improvement routine, scored on benchmarks. Darwin Gödel Machine keeps a population of coding agents and retains variants that do better. Closest public objects to a running Gödel machine. Still frozen foundation weights.

- Yin et al. *Gödel Agent*. [arXiv:2410.04444](https://arxiv.org/abs/2410.04444)
- Zhang, Lu, et al. *Darwin Godel Machine*. [arXiv:2505.22954](https://arxiv.org/abs/2505.22954)

## 2025-06 — Self-edits that change weights

SEAL: the model writes its own finetune data and update directives; those edits are applied as persistent weight updates; RL rewards edits that help the updated model. First widely cited public loop where the evolving object is *weights*, not just prompts or files. Still an offline adaptation cycle, not a deployed net rewriting itself mid-forward-pass.

- Zweiger et al. *Self-Adapting Language Models*. [arXiv:2506.10943](https://arxiv.org/abs/2506.10943)

## 2025-09 / 2025-10 — Papers and contexts as agents

Paper2Agent turns a paper into an interactive agent. ACE evolves the *context* (playbooks, memories) instead of weights. Self-improvement as memory edit.

- Paper2Agent. [arXiv:2509.06917](https://arxiv.org/abs/2509.06917)
- *Agentic Context Engineering*. [arXiv:2510.04618](https://arxiv.org/abs/2510.04618)

## What is missing

A published system that modifies its trained weights *in deployment* and keeps the gains without an offline SFT job. SEAL is the nearest public step. SSI's charter points at the inner problem and does not show work. See [lab fission]({{ '/timelines/lab-fission/' | relative_url }}).
