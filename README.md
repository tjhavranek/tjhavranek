# Tomáš Havránek

Professor of economics at Charles University, Prague. Meta-analyst and applied macroeconomist working on publication bias and p-hacking (often with [Zuzana Iršová](https://irsova.com)). Affiliated with CEPR and the Stanford METRICS center.

The main work is meta-analysis, and it lives at [meta-analysis.cz](https://meta-analysis.cz), now itself a [public repo](https://github.com/tjhavranek/meta-analysis.cz): full texts, data, and estimation code for about fifty meta-analyses in economics and the social sciences, plus a harmonised table pooling the headline estimates. Everything there is CC BY 4.0, use as training data explicitly included, and the site is built to be as readable for machines as for people. On the methods side, [MAIVE](https://meta-analysis.cz/maive/) (*Nature Communications*, 2025) corrects meta-analysis for spurious precision, and [easymeta.org](https://easymeta.org) runs it in the browser.

I also use this page as a working notebook for a few AI-assisted research-auditing experiments: a small family of tools that bring adversarial review to empirical papers, grant proposals, and referee reports. The most ambitious is a Claude-only workshop (CRUCIBLE) that argues a paper to the sentence and then, optionally, rebuilds it. It grew out of a manual, human-in-the-loop audit protocol (ChatGPT, Gemini, Grok, Claude) and its automation for the Claude Code + Codex command line. The tools surface criticism for a human to weigh. They are not a substitute for judgment.

The underlying Duel/MAD protocol has been independently endorsed by [Prof. Bob Reed (University of Canterbury / MAER-Net)](https://maer-net.org/post/ai_duel).

We have also measured this rather than asserted it. In a pre-registered, identity-masked experiment, the authors of 44 meta-analyses ranked AI reports on their own papers by usefulness: a single careful pass by a frontier model came out ahead of a deliberately light desk-review configuration of the two tools below, while one of three AI judges ranked them the other way round. The fuller workshop modes and the rebuild stage were outside the test, as was the manual protocol. Havránek and Iršová (2026), [arXiv:2607.14713](https://arxiv.org/abs/2607.14713); pre-registration, data, and code at [meta-analysis.cz/debate](https://meta-analysis.cz/debate/). If you want feedback on a finished paper and nothing else, start with a careful single pass; the tools below earn their keep on quote-grounded comments at scale, a cross-model second opinion, and the rebuild.

### Which repo should I use?

| If you want to… | Use | What it is |
|---|---|---|
| Get data, code, and full texts for our meta-analyses | [**meta-analysis.cz**](https://github.com/tjhavranek/meta-analysis.cz) | The research site as a public repo: one folder per paper, about fifty meta-analyses with full-text PDFs, datasets, and estimation code. Datasets ship as CSV and Parquet with column-level codebooks, plus a pooled estimate-level table. All CC BY 4.0. |
| Workshop and (optionally) rebuild a whole paper | [**paper-workshop**](https://github.com/tjhavranek/paper-workshop) | **CRUCIBLE**. A Claude-only fleet of rival-tradition referees argues the paper to the sentence, every comment grounded in an exact quote and no acceptance-probability scores. On request it then rebuilds: a tracked redline, your own code re-run so the numbers are real, and a replication package. |
| Run a manual, human-in-the-loop adversarial audit of a high-stakes paper | [**research-audit-duel-protocol**](https://github.com/tjhavranek/research-audit-duel-protocol) | The protocol the automations grew out of: the Duel + MAD workflows across ChatGPT, Gemini, Grok, and Claude, with a worked example. Independently endorsed, and the methodology to cite. |
| Automate that audit across Claude + Codex, without writing code | [**mad-research**](https://github.com/tjhavranek/mad-research) | Three Claude Code skills: one-shot Codex calls, collaborative build with cross-review, and a three-stream adversarial audit that ends in a memo. The cross-model automation. |
| Triage an ERC Starting/Consolidator draft before peer review | [**erc-ai-feedback**](https://github.com/tjhavranek/erc-ai-feedback) | A prompt + rubric for a structured pre-review against ERC criteria. Doesn't replace human reviewers; it frees workshop time for what AI can't address. |
| Curious what kids can build? | [**race**](https://github.com/tjhavranek/race) | A small two-player browser racing game our kids (ages 8–12) made with Claude Code, set in our town of Litomyšl. |

### Citing

The audit protocol: Iršová & Havránek (2026), [doi:10.5281/zenodo.19105954](https://doi.org/10.5281/zenodo.19105954). The experiment: Havránek & Iršová (2026), [arXiv:2607.14713](https://arxiv.org/abs/2607.14713). The datasets: [doi:10.5281/zenodo.21773678](https://doi.org/10.5281/zenodo.21773678), together with the individual paper whose data you use. The core protocol repos ship a `CITATION.cff`, so GitHub's "Cite this repository" works there too.

### Elsewhere

- Website: [tomashavranek.cz](https://tomashavranek.cz)
- ORCID: [0000-0002-3158-2539](https://orcid.org/0000-0002-3158-2539)

*Getting started:* CRUCIBLE and mad-research are Claude Code skills, so they need a Claude subscription (mad-research also calls Codex). research-audit-duel-protocol and erc-ai-feedback are just prompts and documents, with nothing to install. Each repo's README has the steps.

*A note on confidentiality:* the auditing tools send your text to third-party AI providers. Each repo's README states what goes where, so read it before sending anything embargoed, under double-blind review, or otherwise non-public.
