**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$. Suppose

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
A & B \\
 & C
\arrow["f", from=1-1, to=1-2]
\arrow["g", from=1-2, to=2-2]
\arrow["h", from=1-1, to=2-2, swap]
\end{tikzcd}
\end{document}
```

is a commutative diagram in $\mathsf{C}$. Then, the image of this diagram under $F$ i.e. the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(A) & F(B) \\
 & F(C)
\arrow["F(f)", from=1-1, to=1-2]
\arrow["F(g)", from=1-2, to=2-2]
\arrow["F(h)", from=1-1, to=2-2, swap]
\end{tikzcd}
\end{document}
```

is also commutative.

**Proof.** Since the first diagram commutes, $g\circ f=h$. This means $$F(g)\circ F(f)=F(g\circ f)=F(h).$$Therefore, the second diagram also commutes. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]