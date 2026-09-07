---
layout: default
title: Capability stack
permalink: /timelines/capability-stack/
---

# Capability stack

<p class="meta">2012–now · architecture and scale. Every lab is reacting to this line.</p>

Alignment methods live on [post-training]({{ '/timelines/post-training/' | relative_url }}). What “better” meant lives on [evals]({{ '/timelines/evals/' | relative_url }}). Where the tokens came from lives on [data]({{ '/timelines/data/' | relative_url }}). The *window* lives on [memory]({{ '/timelines/memory/' | relative_url }}). Labs live on [fission]({{ '/timelines/lab-fission/' | relative_url }}). Serving that *splits the box* lives on [disaggregated compute]({{ '/timelines/disaggregated-compute/' | relative_url }}).

## 2012-09 — AlexNet

A deep convnet wins ImageNet by a wide margin. GPUs + ReLU + dropout make depth practical. After this, “try a bigger net” is a serious strategy.

- Krizhevsky, Sutskever, Hinton. *ImageNet Classification with Deep Convolutional Neural Networks*. [NeurIPS PDF](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf)
- What followed: VGG, then ResNet. Sequence models still on LSTMs. The contest itself: [evals]({{ '/timelines/evals/' | relative_url }}).

## 2015-12 — ResNet

Residual connections let nets go to 100+ layers without falling over. The default vision backbone until transformers take vision too.

- He et al. *Deep Residual Learning for Image Recognition*. [arXiv:1512.03385](https://arxiv.org/abs/1512.03385)

## 2017-06 — Transformer

Self-attention replaces recurrence for sequence transduction. Training parallelizes across the sequence. This is still the architecture under every frontier model.

- Vaswani et al. *Attention Is All You Need*. [arXiv:1706.03762](https://arxiv.org/abs/1706.03762)
- What followed: BERT (encoder), GPT (decoder), scaling laws. Position encodings later become RoPE; decode bandwidth later becomes GQA — both on [efficiency]({{ '/timelines/efficiency/' | relative_url }}) for the ratio, cited here as architecture:
- Su et al. *RoFormer: Enhanced Transformer with Rotary Position Embedding*. [arXiv:2104.09864](https://arxiv.org/abs/2104.09864)
- Ainslie et al. *GQA*. [arXiv:2305.13245](https://arxiv.org/abs/2305.13245)

## 2018 — Pre-train, then transfer

Two forks of the same idea: bidirectional encoder vs autoregressive decoder.

- Radford et al. *Improving Language Understanding by Generative Pre-Training* (GPT-1). [PDF](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf)
- Devlin et al. *BERT*. [arXiv:1810.04805](https://arxiv.org/abs/1810.04805)

## 2019-02 — GPT-2

1.5B parameters, WebText, zero-shot tasks from next-token prediction. OpenAI stages the release as a safety experiment — first time a language model is treated as dual-use in public.

- Radford et al. *Language Models are Unsupervised Multitask Learners*. [PDF](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)

## 2020-05 — GPT-3

175B. In-context learning without weight updates. Scale starts looking like a method, not a hack.

- Brown et al. *Language Models are Few-Shot Learners*. [arXiv:2005.14165](https://arxiv.org/abs/2005.14165)

## 2020-10 — The same stack for pixels

Vision Transformer: split an image into patches, run a transformer. After ImageNet-scale pretrain it matches or beats ResNets. The architecture line is no longer “convnets for vision, transformers for text.”

- Dosovitskiy et al. *An Image is Worth 16x16 Words*. [arXiv:2010.11929](https://arxiv.org/abs/2010.11929)

## 2020-01 / 2022-03 — Scaling laws

Kaplan: loss is a power law in compute, data, and params — but the paper overweights params. Chinchilla: train smaller models on more tokens. The training recipe for the next four years. Data as the scarce input is also on [data]({{ '/timelines/data/' | relative_url }}).

- Kaplan et al. *Scaling Laws for Neural Language Models*. [arXiv:2001.08361](https://arxiv.org/abs/2001.08361)
- Hoffmann et al. *Training Compute-Optimal Large Language Models* (Chinchilla). [arXiv:2203.15556](https://arxiv.org/abs/2203.15556)

## 2022-03 / 2022-11 — Instruction following, then ChatGPT

RLHF turns a base model into something people will talk to. ChatGPT is the same stack with a chat UI — and the event that puts every other lab on a product clock.

- Ouyang et al. *Training language models to follow instructions with human feedback*. [arXiv:2203.02155](https://arxiv.org/abs/2203.02155)
- [ChatGPT launch](https://openai.com/index/chatgpt/)
- Detail: [post-training]({{ '/timelines/post-training/' | relative_url }}) · firm: [OpenAI]({{ '/timelines/openai/' | relative_url }})

## 2023 — Frontier becomes a race

GPT-4, Claude, Gemini, Llama. Multimodal in the closed labs; open weights as a parallel track. Capability is no longer a single-lab story.

- OpenAI. *GPT-4 Technical Report*. [arXiv:2303.08774](https://arxiv.org/abs/2303.08774)
- Touvron et al. *LLaMA*. [arXiv:2302.13971](https://arxiv.org/abs/2302.13971)
- Google. *Gemini: A Family of Highly Capable Multimodal Models*. [arXiv:2312.11805](https://arxiv.org/abs/2312.11805)
- Anthropic. Claude 3 — [announcement](https://www.anthropic.com/news/claude-3-family) (Mar 2024)

## 2024-09 — Test-time compute

o1-class models spend tokens on a hidden chain of thought, trained with large-scale RL. Inference-time search becomes a second scaling axis next to pretraining. OpenAI publishes evals and a system card, not a recipe.

- [Learning to reason with LLMs](https://openai.com/index/learning-to-reason-with-llms/)
- OpenAI. *o1 System Card*. [arXiv:2412.16720](https://arxiv.org/abs/2412.16720)
- Snell et al. *Scaling LLM Test-Time Compute Optimally*. [arXiv:2408.03314](https://arxiv.org/abs/2408.03314)
- Precursor: Wei et al. *Chain-of-Thought Prompting*. [arXiv:2201.11903](https://arxiv.org/abs/2201.11903)

## 2025-01 — DeepSeek-R1

A public recipe for reasoning models: outcome RL (GRPO), no separate critic required. Cost shock as much as a methods shock. After this, “base model ⇒ reasoner” is assumed to be cheap.

- DeepSeek-AI. *DeepSeek-R1*. [arXiv:2501.12948](https://arxiv.org/abs/2501.12948)
- Also: DeepSeek-V3. [arXiv:2412.19437](https://arxiv.org/abs/2412.19437)
- Lab context: [China labs]({{ '/timelines/china-labs/' | relative_url }}) · ratio: [efficiency]({{ '/timelines/efficiency/' | relative_url }})

## What this page is not

Agents, tools, and computer-use: [agents]({{ '/timelines/agents/' | relative_url }}). Motor policies: [robotics]({{ '/timelines/robotics/' | relative_url }}). Context as a product axis: [memory]({{ '/timelines/memory/' | relative_url }}). DeepMind games and science: [DeepMind]({{ '/timelines/deepmind/' | relative_url }}). Video simulators: [world models]({{ '/timelines/world-models/' | relative_url }}).
