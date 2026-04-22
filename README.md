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

## How to compile (typical)

From within `paper/` (exact main `.tex` filename may vary depending on how the project evolves):

1. Run `pdflatex` (or `latexmk -pdf`) on the main paper file
2. Run `bibtex` (if using BibTeX for references)
3. Re-run `pdflatex` as needed to resolve citations and references

Example (if you use `latexmk`):
```bash
cd paper
latexmk -pdf
```

## What to read first

- For the core theoretical setup: `paper/sections/model.tex`
- For the motivation and framing: `paper/sections/introduction.tex`

## License

See `LICENSE`.
