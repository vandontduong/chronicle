---
layout: default
title: Evals
permalink: /timelines/evals/
---

# Evals

<p class="meta">The scarce object after 2023 is the test, not the net. This page is how the field decided what “better” meant.</p>

Architecture lives on [capability stack]({{ '/timelines/capability-stack/' | relative_url }}). Preference and reasoning recipes live on [post-training]({{ '/timelines/post-training/' | relative_url }}). Coding-agent *products* live on [agents]({{ '/timelines/agents/' | relative_url }}). Interactive worlds that claim to be simulators live on [world models]({{ '/timelines/world-models/' | relative_url }}).

## 2012 / 2015 — ImageNet as the public scoreboard

A labeled photo contest becomes the object every vision paper has to beat. Once the curve saturates, the field needs a new test — the pattern repeats for language.

- Russakovsky et al. *ImageNet Large Scale Visual Recognition Challenge*. [arXiv:1409.0575](https://arxiv.org/abs/1409.0575)

## 2018–19 — GLUE, then SuperGLUE

Nine NLU tasks, one leaderboard. SuperGLUE is the admission that GLUE is already too easy for the models it created.

- Wang et al. *GLUE*. [arXiv:1804.07461](https://arxiv.org/abs/1804.07461)
- Wang et al. *SuperGLUE*. [arXiv:1905.00537](https://arxiv.org/abs/1905.00537)

## 2019 — ARC-AGI-1

Chollet: intelligence as skill-acquisition efficiency on tasks the system was not trained for. Grid puzzles, few shots, core-knowledge priors only. Holds as a hard test from 2019 through late 2024. The other fork of “what better means” — not another language exam.

- Chollet. *On the Measure of Intelligence*. [arXiv:1911.01547](https://arxiv.org/abs/1911.01547)
- [ARC Prize](https://arcprize.org/)

## 2020-09 — MMLU

57-subject multiple choice. The exam that frontier labs still quote in 2026. Weakness is the point: static items leak into the crawl.

- Hendrycks et al. *Measuring Massive Multitask Language Understanding*. [arXiv:2009.03300](https://arxiv.org/abs/2009.03300)

## 2021 — Code and grade-school math

HumanEval: generate a function that passes hidden tests. GSM8K: word problems written so the answer is not in the crawl. Two LM-native exams that pretrain leaderboards did not already contain.

- Chen et al. *Evaluating Large Language Models Trained on Code*. [arXiv:2107.03374](https://arxiv.org/abs/2107.03374)
- Cobbe et al. *Training Verifiers to Solve Math Word Problems* (GSM8K). [arXiv:2110.14168](https://arxiv.org/abs/2110.14168)

## 2022-06 / 2022-11 — BIG-bench and HELM

BIG-bench is a task zoo the community can keep adding to. HELM is the opposite move: one taxonomy, many models, the same scenarios, so comparisons stop being apples-to-oranges press releases.

- Srivastava et al. *Beyond the Imitation Game*. [arXiv:2206.04615](https://arxiv.org/abs/2206.04615)
- Liang et al. *Holistic Evaluation of Language Models*. [arXiv:2211.09110](https://arxiv.org/abs/2211.09110) · [CRFM](https://crfm.stanford.edu/2022/11/17/helm.html)

## 2023-10 / 2023-11 — SWE-bench, GPQA, MMMU

GitHub issues with tests attached. Graduate-level questions written so Google does not already contain the answer. MMMU: college exams that are images as well as text. Three answers to “MMLU is contaminated,” in code, knowledge, and multimodality.

- Jimenez et al. *SWE-bench: Can Language Models Resolve Real-World GitHub Issues?* [arXiv:2310.06770](https://arxiv.org/abs/2310.06770)
- Rein et al. *GPQA: A Graduate-Level Google-Proof Q&A Benchmark*. [arXiv:2311.12022](https://arxiv.org/abs/2311.12022)
- Yue et al. *MMMU: A Massive Multi-discipline Multimodal Understanding and Reasoning Benchmark*. [arXiv:2311.16502](https://arxiv.org/abs/2311.16502)

## 2023– — Arena as the human eval

LMSYS Chatbot Arena: pairwise votes, Elo. Not a paper that invents a task — a running market for taste. Labs start optimizing for it the way they optimized for MMLU.

- Chiang et al. *Chatbot Arena*. [arXiv:2403.04132](https://arxiv.org/abs/2403.04132) · [LMSYS](https://lmsys.org/blog/2023-05-03-arena/)

## 2024-03 / 2024-04 — Live tasks, live desktops

LiveCodeBench: problems posted *after* the model cutoff. OSWorld: a computer-use exam with real apps, not a screenshot quiz. Contamination and environment become design constraints.

- Jain et al. *LiveCodeBench*. [arXiv:2403.07974](https://arxiv.org/abs/2403.07974)
- Xie et al. *OSWorld*. [arXiv:2404.07972](https://arxiv.org/abs/2404.07972)

## 2024-11 — Facts, and expert math

SimpleQA: short questions with one answer; grade correct / wrong / not attempted. FrontierMath: unpublished research-level problems that take a mathematician hours. Two different refusals of “MMLU is the exam” — one tests whether the model knows what it knows, the other whether it can do new math.

- Wei et al. *Measuring short-form factuality in large language models* (SimpleQA). [arXiv:2411.04368](https://arxiv.org/abs/2411.04368) · [OpenAI](https://openai.com/index/introducing-simpleqa/)
- Glazer et al. *FrontierMath*. [arXiv:2411.04872](https://arxiv.org/abs/2411.04872) · [Epoch](https://epoch.ai/frontiermath/about)

## 2024-12 — o3 vs ARC-AGI-1

OpenAI reports o3-preview near the top of ARC-AGI-1 with large test-time compute. The 2019 test is no longer the ceiling. Cost per task becomes part of the scoreboard. See also [post-training]({{ '/timelines/post-training/' | relative_url }}) and [efficiency]({{ '/timelines/efficiency/' | relative_url }}).

- [Analyzing o3 with ARC-AGI](https://arcprize.org/blog/analyzing-o3-with-arc-agi)

## 2025-01 / 2025-03 — Humanity's Last Exam, then ARC-AGI-2

HLE: 2,500 expert closed-ended items billed as the last academic exam of its kind. ARC-AGI-2: same grid format, harder composition, humans still solve the set; early reasoners are in the low single digits. Prize 2025 top private score is 24%. Labs start putting ARC-AGI on model cards.

- Phan et al. *Humanity's Last Exam*. [arXiv:2501.14249](https://arxiv.org/abs/2501.14249)
- Chollet et al. *ARC-AGI-2: A New Challenge for Frontier AI Reasoning Systems*. [arXiv:2505.11831](https://arxiv.org/abs/2505.11831) · [announcement](https://arcprize.org/blog/announcing-arc-agi-2-and-arc-prize-2025)
- Chollet, Knoop, Kamradt, Landers. *ARC Prize 2025: Technical Report*. [arXiv:2601.10904](https://arxiv.org/abs/2601.10904)

## 2026-03 — ARC-AGI-3

The format changes. Interactive, turn-based environments with no instructions: explore, infer the goal, model the dynamics, plan. Humans 100%; harness-free frontier systems below 1% at launch. Efficiency scored against a human action baseline (RHAE). This is the ARC series meeting [agents]({{ '/timelines/agents/' | relative_url }}).

- ARC Prize Foundation. *ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence*. [arXiv:2603.24621](https://arxiv.org/abs/2603.24621)

## What this page is not

A living leaderboard. New benches land here only if they change what labs train for or how they report. Safety evals that gate a release live on [safety]({{ '/timelines/safety/' | relative_url }}).
