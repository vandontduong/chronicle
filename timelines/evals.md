---
layout: default
title: Evals
permalink: /timelines/evals/
---

# Evals

<p class="meta">The scarce object after 2023 is the test, not the net. This page is how the field decided what “better” meant.</p>

Architecture lives on [capability stack]({{ '/timelines/capability-stack/' | relative_url }}). Preference and reasoning recipes live on [post-training]({{ '/timelines/post-training/' | relative_url }}). Coding-agent *products* live on [agents]({{ '/timelines/agents/' | relative_url }}).

## 2012 / 2015 — ImageNet as the public scoreboard

A labeled photo contest becomes the object every vision paper has to beat. Once the curve saturates, the field needs a new test — the pattern repeats for language.

- Russakovsky et al. *ImageNet Large Scale Visual Recognition Challenge*. [arXiv:1409.0575](https://arxiv.org/abs/1409.0575)

## 2018–19 — GLUE, then SuperGLUE

Nine NLU tasks, one leaderboard. SuperGLUE is the admission that GLUE is already too easy for the models it created.

- Wang et al. *GLUE*. [arXiv:1804.07461](https://arxiv.org/abs/1804.07461)
- Wang et al. *SuperGLUE*. [arXiv:1905.00537](https://arxiv.org/abs/1905.00537)

## 2019 — A test that is not a language exam

Chollet: intelligence as skill-acquisition efficiency, measured on tasks the system was not trained for. ARC stays hard after MMLU saturates. The other fork of “what better means.”

- Chollet. *On the Measure of Intelligence*. [arXiv:1911.01547](https://arxiv.org/abs/1911.01547)

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

## 2023-10 / 2023-11 — SWE-bench and GPQA

GitHub issues with tests attached. Graduate-level questions written so Google does not already contain the answer. Two different answers to “MMLU is contaminated.”

- Jimenez et al. *SWE-bench: Can Language Models Resolve Real-World GitHub Issues?* [arXiv:2310.06770](https://arxiv.org/abs/2310.06770)
- Rein et al. *GPQA: A Graduate-Level Google-Proof Q&A Benchmark*. [arXiv:2311.12022](https://arxiv.org/abs/2311.12022)

## 2023– — Arena as the human eval

LMSYS Chatbot Arena: pairwise votes, Elo. Not a paper that invents a task — a running market for taste. Labs start optimizing for it the way they optimized for MMLU.

- Chiang et al. *Chatbot Arena*. [arXiv:2403.04132](https://arxiv.org/abs/2403.04132) · [LMSYS](https://lmsys.org/blog/2023-05-03-arena/)

## 2024-03 / 2024-04 — Live tasks, live desktops

LiveCodeBench: problems posted *after* the model cutoff. OSWorld: a computer-use exam with real apps, not a screenshot quiz. Contamination and environment become design constraints.

- Jain et al. *LiveCodeBench*. [arXiv:2403.07974](https://arxiv.org/abs/2403.07974)
- Xie et al. *OSWorld*. [arXiv:2404.07972](https://arxiv.org/abs/2404.07972)

## What this page is not

A living leaderboard. New benches land here only if they change what labs train for. Safety evals that gate a release live on [safety]({{ '/timelines/safety/' | relative_url }}).
