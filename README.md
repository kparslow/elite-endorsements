# Project Title

... (rest of README content preserved)

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