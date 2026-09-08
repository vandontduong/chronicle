# Chronicle

Constrained wiki of dated beats on AI research. The unit is what changed, not a paper dump.

This repo is a knowledge harness: fixed homes, one deal per page, short beats, verified links. An editor or agent follows the chrome and the beat rules instead of free-writing a news feed.

Site (after Pages is on): **https://vandontduong.github.io/chronicle/**

## Enable GitHub Pages

1. Repo **Settings → Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` / `/` (root)

Confirm the URL returns 200 before sending anyone there.

## Navigation

Header is four doors only. Do not grow it.

| Door | Page |
|---|---|
| Map | [timelines/index.md](timelines/index.md) |
| Stack | [timelines/capability-stack.md](timelines/capability-stack.md) |
| Fission | [timelines/lab-fission.md](timelines/lab-fission.md) |
| Clouds | [timelines/clouds.md](timelines/clouds.md) |

Home, map, and footer use the same five groups: **Train / Loop / Labs / Substrate / Science**. Thirty-three pages. Map start-here is stack, evals, fission, clouds, techbio — not a new company page.

Breadcrumb on every timeline: Chronicle · Map · this page · **History** (git log for that file). No hand-typed `updated:` dates.

New timeline: add it to `timelines/index.md`, `index.md`, `_includes/sitemap.html`, and this README. Header stays four links.

### Train

- [Capability stack](timelines/capability-stack.md) — architecture and scale
- [Post-training](timelines/post-training.md) — distill as a recipe
- [Evals](timelines/evals.md) — what “better” meant
- [Data](timelines/data.md) — crawl, mix, books, poison
- [Memory](timelines/memory.md) — context window as asset
- [Information theory](timelines/information-theory.md) — the bit and the loss
- [Essays](timelines/essays.md) — named frames, Turing to Altman

### Loop

- [Agents](timelines/agents.md) — a model plus a loop
- [Robotics](timelines/robotics.md) — VLAs / motor tokens
- [World models](timelines/world-models.md) — next-state predictors
- [Safety](timelines/safety.md) — regimes that changed what shipped
- [RSI](timelines/rsi.md) — what is allowed to rewrite itself
- [Efficiency](timelines/efficiency.md) — distill as a ratio; capability per flop

### Labs

- [OpenAI](timelines/openai.md) — the firm
- [Anthropic](timelines/anthropic.md) — the firm
- [DeepMind](timelines/deepmind.md) — games → science → Gemini
- [Lab fission](timelines/lab-fission.md) — forks, not a calendar
- [SpaceX](timelines/spacex.md) — franchise, Colossus, xAI, Cursor, Starmind
- [China labs](timelines/china-labs.md) — open weights, cheap reasoners, HK listings
- [Stripe](timelines/stripe.md) — payments API to agent and token rails

### Substrate

- [Integrated circuits](timelines/integrated-circuits.md) — the die as constraint
- [TSMC](timelines/tsmc.md) — foundry and CoWoS
- [HBM](timelines/hbm.md) — the stack next to the GPU
- [Disaggregated compute](timelines/disaggregated-compute.md) — pools and phase split
- [Nvidia](timelines/nvidia.md) — silicon and the cheques
- [Cerebras](timelines/cerebras.md) — wafer-scale decode
- [Clouds](timelines/clouds.md) — GPU debt and offtakes
- [Cryptocurrency](timelines/cryptocurrency.md) — hash, GPU mines, Merge
- [Storage](timelines/storage.md) — rust and NAND under the window

### Science

- [Techbio](timelines/techbio.md) — structure → clinic
- [Illumina](timelines/illumina.md) — the short-read meter
- [Intuitive](timelines/intuitive.md) — console, wrist, installed base

## Harness rules

A paper may sit on two pages. A deal has one home. Length is not quality. Leave thin pages thin.

Canonical homes (tell once, point everywhere else):

- Musk stack company object — [spacex.md](timelines/spacex.md)
- GPU debt, offtakes, Colossus *rents* — [clouds.md](timelines/clouds.md)
- Lab theses and the papers that proved the fork — [lab-fission.md](timelines/lab-fission.md)
- Architecture and scale — [capability-stack.md](timelines/capability-stack.md)
- SFT / prefs / reasoning RL — [post-training.md](timelines/post-training.md)
- Loops that touch the world — [agents.md](timelines/agents.md)
- What is allowed to rewrite itself — [rsi.md](timelines/rsi.md)
- Capability per flop — [efficiency.md](timelines/efficiency.md)
- Named frames (Turing, Sutton, Altman) — [essays.md](timelines/essays.md)
- Structure models → clinic — [techbio.md](timelines/techbio.md)
- Short-read meter — [illumina.md](timelines/illumina.md)
- Agent checkout, token metering, OpenRouter — [stripe.md](timelines/stripe.md)
- HBM stacks and vendor quals — [hbm.md](timelines/hbm.md)

Cite arXiv, the journal, the lab post, or the filing. No AlphaXiv. No `papers/` tree. No invented tweet IDs.

## Beat format

```
YYYY-MM  Name
  What changed (2–4 sentences).
  Paper or announcement + links.
  What followed.
```

A deal is a beat only if it changes who trains, who ships, or what the thesis is.

## Edit rule

Prefer one new beat over a rewrite. Do not turn a timeline into a news feed.
