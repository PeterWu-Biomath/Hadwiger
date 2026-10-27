# Notes on Hadwiger's conjecture

Personal reading notes on the manuscript *A counterexample to Hadwiger's conjecture*, attributed to OpenAI.

- The authors tend to use nonstandard terminology. For example, "holes" actually means "edges in the complement graph." They also use terms from other fields, such as "witness" and "certificate." These may be familiar to theoretical computer scientists, but I need to make an extra effort to understand what they mean in this context. Other terms, such as "demand" and "pin budget," were unclear to me when I first encountered them.
- In its proofs, the AI does not clearly distinguish between trivial steps and those that need emphasis. This makes the text lengthy and the central ideas hard to grasp.

The goal is to address these shortcomings and produce a clearer manuscript.

## Contents

- `Hadwiger.tex`: the editable LaTeX source.
- `Hadwiger.pdf`: the compiled notes; regenerate after changing the source.
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

Edit `Hadwiger.tex` and compile it with the Codex LaTeX editor or a local LaTeX installation. With a local installation, run the following command twice from this folder to resolve references:

```sh
pdflatex Hadwiger.tex
```

The `.aux`, `.log`, and `.synctex.gz` files are generated during compilation.

## Note (2026/10/27)

The construction remains beyond my current understanding, and I do not plan to return to this project in the near future. My main takeaway is that Theorem 3.1 is the key result. A possible starting point for simplifying the construction would be to find a simpler probability distribution on vertices, together with an edge rule, for which an analogue of Theorem 3.1 holds.
