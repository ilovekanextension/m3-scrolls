**Theorem.** Let $\mathsf{C}$ be a category. Let $f:a\to b$ be a morphism in $\mathsf{C}$. Then, the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
a & b \\
a & b
\arrow["f", from=1-1, to=1-2]
\arrow["\text{id}_a", from=1-1, to=2-1, swap]
\arrow["f", from=2-1, to=2-2]
\arrow["\text{id}_b", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes.

**Proof.** We have $$f\circ \text{id}_{a}=f=\text{id}_{b}\circ f,$$so the diagram posed in the statement commutes. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Categorical Diagram]]