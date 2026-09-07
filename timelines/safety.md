---
layout: default
title: Safety
permalink: /timelines/safety/
---

# Safety

<p class="meta">Regimes that changed what shipped — not a mood. Alignment methods that are also product live on [post-training]({{ '/timelines/post-training/' | relative_url }}) and [Anthropic]({{ '/timelines/anthropic/' | relative_url }}).</p>

Preparedness cards and constitutions belong here when they gate a release. Dual-use evals that are just a bench live on [evals]({{ '/timelines/evals/' | relative_url }}).

## 2016-06 — The problem list

Amodei, Olah, et al. write down specification, robustness, and assurance as engineering work. The later lab safety orgs are this memo with a budget.

- Amodei et al. *Concrete Problems in AI Safety*. [arXiv:1606.06565](https://arxiv.org/abs/1606.06565)

## 2022-03 / 2022-12 — Preferences, then a constitution

InstructGPT makes human preference the loss. Constitutional AI makes the preference list readable and partly automated. Both are post-training; both are the safety stack the products actually run.

- Ouyang et al. *InstructGPT*. [arXiv:2203.02155](https://arxiv.org/abs/2203.02155)
- Bai et al. *Constitutional AI*. [arXiv:2212.08073](https://arxiv.org/abs/2212.08073)
- [Claude's constitution](https://www.anthropic.com/research/claudes-constitution)

## 2023-12 / 2025-04 — Frontier pledges become org charts

Anthropic Responsible Scaling Policy. OpenAI Preparedness (Dec 2023). The unit is a capability threshold with a promised eval, not a paper. OpenAI moved the original announcement off `/introducing-the-preparedness-framework/`; the living page is the 2025 update. The beta PDF is the first public text.

- [Anthropic RSP](https://www.anthropic.com/news/anthropics-responsible-scaling-policy)
- [Preparedness Framework, Dec 2023 PDF](https://cdn.openai.com/openai-preparedness-framework-beta.pdf)
- [OpenAI — updated Preparedness Framework](https://openai.com/index/updating-our-preparedness-framework/) (Apr 2025)

## 2023-12 / 2024-01 — Hidden goals

Hubinger et al.: models can keep a backdoor through safety training. “Sleeper” is the empirical version of the old deceptive-alignment story.

- Hubinger et al. *Sleeper Agents*. [arXiv:2401.05566](https://arxiv.org/abs/2401.05566) · [Anthropic](https://www.anthropic.com/research/sleeper-agents-training-deceptive-llms-that-persist-through-safety-training)

## 2024-04 — Many-shot jailbreaks

Long context is an attack surface. Safety training that assumed short prompts does not transfer when the attacker can write a novel of examples.

- [Many-shot jailbreaking](https://www.anthropic.com/research/many-shot-jailbreaking)

## 2024-05 — Features, not just policies

Templeton et al.: dictionary learning on a production Claude. Interpretability as a paper you can cite, not a slide. Still not a control method.

- [Scaling Monosemanticity](https://www.anthropic.com/research/mapping-mind-language-model)

## 2024-05 — Model Spec

OpenAI publishes the intended behavior as a document the model is trained to follow. The analogue of a constitution, from the other lab.

- [OpenAI Model Spec](https://openai.com/index/introducing-the-model-spec/)

## 2025-10 — Poison count

Same Anthropic / AISI result as on [data]({{ '/timelines/data/' | relative_url }}): a few hundred docs. Cited here because it moves safety from “filter the mix” to “assume the mix is hostile.”

- [A small number of samples can poison LLMs of any size](https://www.anthropic.com/research/small-samples-poison)

## What this page is not

Policy commentary or a list of every system card. System cards that only score a model stay on the lab page. Capability evals that do not gate shipping stay on [evals]({{ '/timelines/evals/' | relative_url }}).
