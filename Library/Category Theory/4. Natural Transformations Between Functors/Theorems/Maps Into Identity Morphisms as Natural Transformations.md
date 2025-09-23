**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$. Then, the map $\iota$ that assigns to each object $a$ in $\mathsf{C}$ the morphism $$\iota_{a}=\text{id}_{F(a)}$$is a natural transformation on $F$.

**Proof.** Suppose $f:a\to b$ is a morphism in $\mathsf{C}$. Consider the following diagram.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(a) \arrow["F(f)", r] \arrow["\iota_a", d] & F(b) \arrow["\iota_b", d] \\
F(a) \arrow["F(f)", r] & F(b)
\end{tikzcd}
\end{document}
```

By definition of $\iota$, we have $\iota_{a}=\text{id}_{F(a)}$ and $\iota_{b}=\text{id}_{F(b)}$, so by [[Square Diagrams with Identity Morphisms as Commutative Squares]] the diagram commutes. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Natural Transformation]]

Theorems used:
- [[Square Diagrams with Identity Morphisms as Commutative Squares]]