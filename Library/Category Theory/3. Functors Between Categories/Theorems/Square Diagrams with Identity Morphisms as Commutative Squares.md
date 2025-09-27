**Theorem.** Let $\mathsf{C}$ be a category. Let $f:A\to B$ be a morphism in $\mathsf{C}$. Then, the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
A & B \\
A & B
\arrow["f", from=1-1, to=1-2]
\arrow["\text{id}_A", from=1-1, to=2-1, swap]
\arrow["f", from=2-1, to=2-2]
\arrow["\text{id}_B", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes.

**Proof.** We have $$f\circ \text{id}_{A}=f=\text{id}_{B}\circ f,$$so the diagram posed in the statement commutes. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Categorical Diagram]]