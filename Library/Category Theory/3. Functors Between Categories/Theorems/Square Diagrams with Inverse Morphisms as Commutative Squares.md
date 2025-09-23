**Theorem.** Let $\mathsf{C}$ be a category. Let the following be a diagram of $\mathsf{C}$.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
a_1 & b_1 \\
a_2 & b_2
\arrow["x_1", from=1-1, to=1-2]
\arrow["f", from=1-1, to=2-1]
\arrow["x_2", from=2-1, to=2-2]
\arrow["g", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

Suppose that $f$ and $g$ are isomorphisms. Then, the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
a_1 & b_1 \\
a_2 & b_2
\arrow["x_1", from=1-1, to=1-2]
\arrow["f^{-1}", from=2-1, to=1-1]
\arrow["x_2", from=2-1, to=2-2]
\arrow["g^{-1}", from=2-2, to=1-2, swap]
\end{tikzcd}
\end{document}
```

also commutes.

**Proof.** Since the first diagram commutes, $g\circ x_{1}=x_{2}\circ f$. This means $g\circ x_{1}\circ f^{-1}=x_{2}$, so $x_{1}\circ f^{-1}=g^{-1}\circ x_{2}$, which means the second diagram commutes. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Categorical Diagram]]