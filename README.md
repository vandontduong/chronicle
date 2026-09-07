# Chronicle

Dated beats on AI research: timelines, model lineages, and paper notes.

Site (after Pages is on): **https://vandontduong.github.io/chronicle/**

## Enable GitHub Pages

1. Repo **Settings → Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` / `/` (root)

Jekyll builds from this repo. No extra Action required.

## Spine

| Timeline | What it tracks |
|---|---|
| [Capability stack](timelines/capability-stack.md) | AlexNet → Transformer → GPT → ChatGPT → reasoning |
| [DeepMind](timelines/deepmind.md) | Atari → AlphaGo → MuZero → AlphaFold → Gemini |
| [Lab fission](timelines/lab-fission.md) | OpenAI → Anthropic → xAI → SSI → Thinking Machines |
| [Post-training](timelines/post-training.md) | RLHF → Constitutional AI → DPO → RL-for-reasoning |
| [Agents](timelines/agents.md) | Tools → coding agents → computer use |

Papers live as short stubs under `papers/`. Full text stays on [arXiv](https://arxiv.org) / [alphaXiv](https://www.alphaxiv.org).

## Beat format

```
YYYY-MM  Name
  What changed (2–4 sentences).
  Paper + links.
  What followed.
```

A paper can sit on more than one timeline.
