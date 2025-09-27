**Definition.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F,G:\mathsf{C}\to \mathsf{D}$. A **transformation** $\nu$ from $F$ to $G$ consists of a collection of morphisms $\nu_{A}:F(A)\to G(A)$ in $\mathsf{D}$ for each object $A$ in $\mathsf{C}$. The morphism $\nu_{A}$ is called the **component** of $\nu$ at $A$.

A transformation $\nu$ from $F$ to $G$ is said to be **natural**, and then called a **natural transformation**, if for all morphisms $f:A\to B$ in $\mathsf{C}$ the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(A) & F(B) \\
G(A) & G(B)
\arrow["F(f)", from=1-1, to=1-2]
\arrow["\nu_A", from=1-1, to=2-1]
\arrow["G(f)", from=2-1, to=2-2]
\arrow["\nu_B", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes.

If $\nu$ is a natural transformation from $F$ to $G$, we may write $$\nu:F\Rightarrow G.$$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]