# Elite Endorsements (ongoing)

This repository contains **in-progress research via formal theoretical model** about **how political elites choose endorsements in primary elections**, and what those choices imply for **coordination, factional conflict, and candidate selection**.

At a high level, the project treats endorsements as *strategic actions* taken under uncertainty: elites may prefer different candidates for ideological or factional reasons, but they also care about being aligned with a winner (and about the rewards that come from backing the eventual nominee). The central goal is to build a model that makes these tradeoffs explicit and helps clarify when elites will:
- **coordinate** on a single “establishment” option,
- **split** across multiple candidates (intentionally or due to incentives),
- or **fail to coordinate** even when coordination might seem collectively beneficial.

## Status / important note

**This is ongoing work. The theoretical model is under major revisions.**  
The current draft should be viewed as a **starting point**—a baseline from which I am iterating—rather than a finished or stable statement of assumptions, mechanisms, or results.

## Repository structure

- `paper/` — LaTeX source for the paper
  - `paper/sections/` — main section files
    - `introduction.tex` — motivation and contribution overview
    - `literature-review.tex` — related literature
    - `model.tex` — the **current draft** of the formal model (under revision)
    - `analysis.tex` — analysis / results and discussion (evolving)
  - `paper/bib/citations.bib` — BibTeX bibliography
  - `paper/figures/` — figures used in the paper
    - Includes endorsement-share plots (e.g., `1988D_endorse_share.png`, `2000R_endorse_share.png`)
    - `paper/figures/simulations/` — simulation output figures (e.g., `Complementarity.png`, `CoordinationThresholds.png`, etc.)

## Compiling the Paper

To compile the paper, the main entrypoint is `paper/paper.tex`. The project uses `biblatex` with `biber` (as specified in `paper/sections/preamble.tex`).

Users should run the following command:

```
latexmk -pdf -interaction=nonstopmode paper/paper.tex
```

Alternatively, for manual compilation, use the following steps from the `paper/` directory:

```
pdflatex paper.tex
biber paper
pdflatex paper.tex
pdflatex paper.tex
```

Ensure you are in the `paper/` directory when executing these commands.

## What to read first

- For the core theoretical setup: `paper/sections/model.tex`
- For the motivation and framing: `paper/sections/introduction.tex`

## License

See `LICENSE`.
