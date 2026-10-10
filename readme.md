# Notes on Hadwiger's conjecture

Personal reading notes by Pei Wu on the manuscript *A counterexample to Hadwiger's conjecture*, attributed to OpenAI.

## Contents

- `Hardwiger.tex`: the editable LaTeX source.
- `Hardwiger.pdf`: the compiled notes; regenerate after changing the source.
- The summary defines the connected matching number and explains how a small connected matching number gives a clique-minor bound below the chromatic number.
- Appendix A discusses the counting proof of Proposition 3.5 using singleton, two-vertex, and larger branch sets.

These notes are a work in progress.

## Notation

The notes use `G` for the triangle-free hole graph and its complement for the proposed counterexample. The manuscript uses `G` for the counterexample itself.

- `cm(H)`: the maximum number of edges in a matching in which every pair of matching edges is joined by an edge of `H`.
- `h(H)`: the largest integer `t` for which `H` contains a complete graph `K_t` as a minor.
- `alpha(H)`: the independence number.
- `chi(H)`: the chromatic number.
- `m`: the number of vertices.

## Editing and compilation

Edit `Hardwiger.tex` and compile it with the Codex LaTeX editor or a local LaTeX installation. With a local installation, run the following command twice from this folder to resolve references:

```sh
pdflatex Hardwiger.tex
```

The `.aux`, `.log`, and `.synctex.gz` files are generated during compilation.
