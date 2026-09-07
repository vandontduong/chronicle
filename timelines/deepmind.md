---
layout: default
title: DeepMind
permalink: /timelines/deepmind/
---

# DeepMind

<p class="meta">Games → science → Gemini</p>

Read this as one lab changing *what counts as a result*. Atari and Go created the talent pool. AlphaFold spent it on a natural science. Gemini is the product the merger had to ship. Structure and clinic continue on [techbio]({{ '/timelines/techbio/' | relative_url }}).

## 2010 / 2014 — Lab, then Google

Hassabis, Suleyman, Legg. Bought by Google in 2014. The scientific culture stays a lab inside a product company until the 2023 Brain merge forces a frontier-model clock.

## 2013-12 / 2015 — DQN

One network learns many Atari games from pixels. The Nature follow-up makes deep RL a field, not a preprint.

- Mnih et al. *Playing Atari with Deep Reinforcement Learning*. [arXiv:1312.5602](https://arxiv.org/abs/1312.5602)
- Mnih et al. *Human-level control through deep reinforcement learning*. [Nature](https://www.nature.com/articles/nature14236) (2015)

## 2015–17 — The Atari toolkit

Double Q, prioritized replay, dueling nets, A3C, Rainbow. Incremental papers that became the default RL stack — including the stack OpenAI later uses for PPO-era work.

- van Hasselt et al. *Double Q-learning*. [arXiv:1509.06461](https://arxiv.org/abs/1509.06461)
- Schaul et al. *Prioritized Experience Replay*. [arXiv:1511.05952](https://arxiv.org/abs/1511.05952)
- Wang et al. *Dueling Network Architectures*. [arXiv:1511.06581](https://arxiv.org/abs/1511.06581)
- Mnih et al. *A3C*. [arXiv:1602.01783](https://arxiv.org/abs/1602.01783)
- Hessel et al. *Rainbow*. [arXiv:1710.02298](https://arxiv.org/abs/1710.02298)

## 2016-03 — AlphaGo

Policy net + value net + MCTS beats Lee Sedol. Public shock; RL talent floods the field.

- Silver et al. *Mastering the game of Go with deep neural networks and tree search*. [Nature](https://www.nature.com/articles/nature16961) 529 (2016)

## 2017-10 / 2017-12 — AlphaGo Zero / AlphaZero

Self-play, no human games. Tabula rasa becomes a method. Chess and shogi fall to the same algorithm. This is the cleanest statement of "the search loop is the method." Cousin of later [RSI]({{ '/timelines/rsi/' | relative_url }}) outer loops, with a known game as the evaluator.

- Silver et al. *Mastering the game of Go without human knowledge*. [Nature](https://www.nature.com/articles/nature24270) 550 (2017)
- Silver et al. *Mastering Chess and Shogi by Self-Play*. [arXiv:1712.01815](https://arxiv.org/abs/1712.01815)

## 2019-11 — MuZero

Learns the rules. Planning with a learned model instead of a given simulator. Closes the games line as a research program.

- Schrittwieser et al. *Mastering Atari, Go, Chess and Shogi by Planning with a Learned Model*. [arXiv:1911.08265](https://arxiv.org/abs/1911.08265)

## 2020-11 / 2021-07 — AlphaFold 2

Protein structure at useful accuracy. First DeepMind result that changes a natural science. Nature paper, code, and a public database. Every later design model filters against it.

- Jumper et al. *Highly accurate protein structure prediction with AlphaFold*. [Nature](https://www.nature.com/articles/s41586-021-03819-4) 596 (2021) · [DeepMind](https://deepmind.google/research/publications/45151/)
- [AlphaFold DB](https://alphafold.ebi.ac.uk/)
- Continuation: [techbio]({{ '/timelines/techbio/' | relative_url }})

## 2021 — Isomorphic

Hassabis spins out a drug company on the AF stack. The lab's science becomes a firm. [Isomorphic Labs](https://www.isomorphiclabs.com/)

## 2021-12 / 2022-03 — Gopher, then Chinchilla

Gopher is a big LM. Chinchilla is the correction: more tokens, fewer params, same compute. That recipe leaks into everyone else's training runs — also on [efficiency]({{ '/timelines/efficiency/' | relative_url }}).

- Rae et al. *Gopher*. [arXiv:2112.11446](https://arxiv.org/abs/2112.11446)
- Hoffmann et al. *Training Compute-Optimal Large Language Models*. [arXiv:2203.15556](https://arxiv.org/abs/2203.15556)

## 2022-04 / 2022-05 — Flamingo and Gato

Vision-language few-shot (Flamingo). One generalist agent, many tasks (Gato). Uneven results; the lab's language shifts from games to general agents.

- Alayrac et al. *Flamingo*. [arXiv:2204.14198](https://arxiv.org/abs/2204.14198)
- Reed et al. *A Generalist Agent*. [arXiv:2205.06175](https://arxiv.org/abs/2205.06175)

## 2023–26 — Gemini line

Brain + DeepMind merge. Frontier multimodal models; long context and agents become the product surface. AlphaGeometry 2 is the old games-science habit applied to olympiad proofs. Gemini 1.5's window is also on [memory]({{ '/timelines/memory/' | relative_url }}).

- *Gemini*. [arXiv:2312.11805](https://arxiv.org/abs/2312.11805)
- *Gemini 1.5*. [arXiv:2403.05530](https://arxiv.org/abs/2403.05530)
- *Gemini 2.5*. [arXiv:2507.06261](https://arxiv.org/abs/2507.06261)
- AlphaGeometry 2. [arXiv:2502.03544](https://arxiv.org/abs/2502.03544)
- AlphaFold 3. Nature 2024 — [techbio]({{ '/timelines/techbio/' | relative_url }})

People who leave (Reflection, and the broader 2024–26 wave) are on [lab fission]({{ '/timelines/lab-fission/' | relative_url }}).

## What this page is not

A Gemini release log. Product versions only count when they change the research program (long context, geometry, structure).
