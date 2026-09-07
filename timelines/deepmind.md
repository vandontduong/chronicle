---
layout: default
title: DeepMind
permalink: /timelines/deepmind/
---

# DeepMind

<p class="meta">Games → science · highest scientific yield of any single lab line</p>

## 2013-12 / 2015 — DQN

One network learns many Atari games from pixels. Nature follow-up makes deep RL a field, not a preprint.

- Mnih et al. *Playing Atari with Deep Reinforcement Learning*. [stub]({{ '/papers/1312.5602/' | relative_url }}) · [arXiv:1312.5602](https://arxiv.org/abs/1312.5602) · [alphaXiv](https://www.alphaxiv.org/abs/1312.5602)
- Mnih et al. *Human-level control through deep reinforcement learning* (Nature, 2015). Same line, the version that landed.

## 2015–17 — The Atari toolkit

Double Q, prioritized replay, dueling nets, A3C, Rainbow. Incremental, but they become the default RL stack.

- van Hasselt et al. *Deep Reinforcement Learning with Double Q-learning*. [arXiv:1509.06461](https://arxiv.org/abs/1509.06461)
- Schaul et al. *Prioritized Experience Replay*. [arXiv:1511.05952](https://arxiv.org/abs/1511.05952)
- Wang et al. *Dueling Network Architectures*. [arXiv:1511.06581](https://arxiv.org/abs/1511.06581)
- Mnih et al. *Asynchronous Methods for Deep Reinforcement Learning* (A3C). [arXiv:1602.01783](https://arxiv.org/abs/1602.01783)
- Hessel et al. *Rainbow*. [arXiv:1710.02298](https://arxiv.org/abs/1710.02298)

## 2016-03 — AlphaGo

Policy net + value net + MCTS beats Lee Sedol. Public shock; RL talent floods the field. Nature paper, not arXiv-first.

- Silver et al. *Mastering the game of Go with deep neural networks and tree search*. Nature 529 (2016). [DeepMind](https://deepmind.google/research/publications/68208/)

## 2017-10 / 2017-12 — AlphaGo Zero / AlphaZero

Self-play, no human games. Tabula rasa becomes a method. Chess and shogi fall in the same algorithm.

- Silver et al. *Mastering the game of Go without human knowledge*. Nature 550 (2017).
- Silver et al. *Mastering Chess and Shogi by Self-Play with a General Reinforcement Learning Algorithm*. [arXiv:1712.01815](https://arxiv.org/abs/1712.01815) · [alphaXiv](https://www.alphaxiv.org/abs/1712.01815)

## 2019-11 — MuZero

Learns the rules. Planning with a learned model instead of a given simulator. Closes the games line as a research program.

- Schrittwieser et al. *Mastering Atari, Go, Chess and Shogi by Planning with a Learned Model*. [arXiv:1911.08265](https://arxiv.org/abs/1911.08265) · [alphaXiv](https://www.alphaxiv.org/abs/1911.08265)

## 2020-11 / 2021-07 — AlphaFold 2

Protein structure at useful accuracy. First DeepMind result that changes a natural science. Nature paper + code.

- Jumper et al. *Highly accurate protein structure prediction with AlphaFold*. Nature 596 (2021). [DeepMind](https://deepmind.google/discover/blog/alphafold-a-solution-to-a-50-year-old-grand-challenge-in-biology/)
- [AlphaFold Protein Structure Database](https://alphafold.ebi.ac.uk/)

## 2021-12 / 2022-03 — Language at scale, then Chinchilla

Gopher is a big LM. Chinchilla is the correction: more tokens, fewer params. That recipe leaks into everyone else's training runs.

- Rae et al. *Scaling Language Models: Methods, Analysis & Insights from Training Gopher*. [arXiv:2112.11446](https://arxiv.org/abs/2112.11446)
- Hoffmann et al. *Training Compute-Optimal Large Language Models*. [arXiv:2203.15556](https://arxiv.org/abs/2203.15556) · [alphaXiv](https://www.alphaxiv.org/abs/2203.15556)

## 2022-04 / 2022-05 — Flamingo and Gato

Vision-language few-shot (Flamingo). One generalist agent, many tasks (Gato). Uneven results; the lab's language shifts from games to general agents.

- Alayrac et al. *Flamingo*. [arXiv:2204.14198](https://arxiv.org/abs/2204.14198) · [alphaXiv](https://www.alphaxiv.org/abs/2204.14198)
- Reed et al. *A Generalist Agent*. [arXiv:2205.06175](https://arxiv.org/abs/2205.06175) · [alphaXiv](https://www.alphaxiv.org/abs/2205.06175)

## 2023–26 — Gemini line

Brain + DeepMind merge. Frontier multimodal models; long context and agents become the product surface.

- Gemini team. *Gemini: A Family of Highly Capable Multimodal Models*. [arXiv:2312.11805](https://arxiv.org/abs/2312.11805) · [alphaXiv](https://www.alphaxiv.org/abs/2312.11805)
- *Gemini 1.5*. [arXiv:2403.05530](https://arxiv.org/abs/2403.05530) · [alphaXiv](https://www.alphaxiv.org/abs/2403.05530)
- *Gemini 2.5*. [arXiv:2507.06261](https://arxiv.org/abs/2507.06261) · [alphaXiv](https://www.alphaxiv.org/abs/2507.06261)
- AlphaGeometry 2. [arXiv:2502.03544](https://arxiv.org/abs/2502.03544)

Also on: [capability stack]({{ '/timelines/capability-stack/' | relative_url }}), [agents]({{ '/timelines/agents/' | relative_url }}).
