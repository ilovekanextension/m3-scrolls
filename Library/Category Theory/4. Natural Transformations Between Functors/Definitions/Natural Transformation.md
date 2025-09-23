**Definition.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F,G:\mathsf{C}\to \mathsf{D}$. A map $\nu$ that assigns to each object $a$ in $\mathsf{C}$ a morphism $\nu_{a}:F(a)\to G(a)$ is called a **natural transformation** from $F$ to $G$ if for all morphisms $f:a\to b$ in $\mathsf{C}$ the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(a) & F(b) \\
G(a) & G(b)
\arrow["F(f)", from=1-1, to=1-2]
\arrow["G(f)", from=2-1, to=2-2]
\arrow["\nu_a", from=1-1, to=2-1]
\arrow["\nu_b", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. The morphism $\nu_{a}$ is called the **component** of $\nu$ at $a$.

If $\nu$ is a natural transformation from $F$ to $G$, we may write $\nu:F\Rightarrow G$.
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]