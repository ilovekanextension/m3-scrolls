**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$. Then, the transformation $\iota$ from $F$ to $F$ defined as $$\iota_{A}=\text{id}_{F(A)}$$is a natural transformation.

**Proof.** Suppose $f:A\to B$ is a morphism in $\mathsf{C}$. Consider the following diagram.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(A) & F(B) \\
F(A) & F(B)
\arrow["\iota_A", from=1-1, to=2-1, swap]
\arrow["F(f)", from=1-1, to=1-2]
\arrow["\iota_B", from=1-2, to=2-2]
\arrow["F(f)", from=2-1, to=2-2]
\end{tikzcd}
\end{document}
```

By definition of $\iota$, we have $\iota_{A}=\text{id}_{F(A)}$ and $\iota_{B}=\text{id}_{F(B)}$, so by [[Square Diagrams with Identity Morphisms as Commutative Squares]] the diagram commutes. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Natural Transformation]]

Theorems used:
- [[Square Diagrams with Identity Morphisms as Commutative Squares]]