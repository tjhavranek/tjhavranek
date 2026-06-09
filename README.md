# Tomáš Havránek

Professor of economics at Charles University, Prague. Meta-analyst and applied macroeconomist working on publication bias, p-hacking, and Bayesian model averaging (often with [Zuzana Iršová](https://irsova.com)). Affiliated with CEPR and the Stanford METRICS center.

I use this page as a working notebook for a few **AI-assisted research-auditing** experiments: a small family of tools that bring adversarial review to empirical papers, grant proposals, and referee reports. The line runs from a manual, human-in-the-loop **audit protocol** (multi-model: ChatGPT, Gemini, Grok, Claude), to its **automation** for the Claude Code + Codex command line, to a Claude-only **workshop** that rebuilds a paper, to a **domain application** for ERC grant drafts, alongside, and feeding back into, the meta-analysis work in the labs below. The tools surface structured criticism for a human to weigh; they are not a substitute for judgment.

The main protocol has been independently endorsed by [Prof. Bob Reed (University of Canterbury / MAER-Net)](https://maer-net.org/post/ai_duel).

### Which repo should I use?

| If you want to… | Use | What it is |
|---|---|---|
| Run a manual, human-in-the-loop adversarial audit of a high-stakes paper | [**research-audit-duel-protocol**](https://github.com/tjhavranek/research-audit-duel-protocol) | The main protocol: the Duel + MAD workflows across ChatGPT, Gemini, Grok, and Claude, with a worked example and an external endorsement. This is the one to read first. |
| Automate that audit across Claude + Codex, without writing code | [**mad-research**](https://github.com/tjhavranek/mad-research) | Three Claude Code skills: one-shot Codex calls, collaborative build with cross-review, and a three-stream adversarial audit. The cross-model (Claude + Codex) automation; it produces an audit memo. |
| Workshop and (optionally) rebuild a whole paper | [**paper-workshop**](https://github.com/tjhavranek/paper-workshop) | **CRUCIBLE**: a Claude-only fleet of rival-tradition referees argues the paper to the sentence (every comment grounded in an exact quote, no acceptance-probability scores), then — opt-in — rebuilds it: a tracked redline, your own code re-run so the numbers are real, and a replication package. The newest of these tools, and the least battle-tested — effectiveness isn't measured yet. |
| Triage an ERC Starting/Consolidator draft before peer review | [**erc-ai-feedback**](https://github.com/tjhavranek/erc-ai-feedback) | A prompt + rubric for a structured pre-review against ERC criteria. Doesn't replace human reviewers; it frees workshop time for what AI can't address. |
| Curious what kids can build? | [**race**](https://github.com/tjhavranek/race) | A small two-player browser racing game our kids (ages 8–12) made with Claude Code, set in our town of Litomyšl. |

### Cite the protocol

Iršová & Havránek (2026) — [doi:10.5281/zenodo.19105954](https://doi.org/10.5281/zenodo.19105954). The core protocol repos ship a `CITATION.cff`, so GitHub's "Cite this repository" works there too.

### Elsewhere

- Website — [tomashavranek.cz](https://tomashavranek.cz)
- ORCID — [0000-0002-3158-2539](https://orcid.org/0000-0002-3158-2539)
- Labs — [meta-analysis.cz](https://meta-analysis.cz) · [easymeta.org](https://easymeta.org)

*A note on confidentiality:* these tools send your text to third-party AI providers. Each repo's README states what goes where — read it before sending anything embargoed, under double-blind review, or otherwise non-public.
