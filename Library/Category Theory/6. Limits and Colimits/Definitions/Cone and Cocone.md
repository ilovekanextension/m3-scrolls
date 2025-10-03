**Definition.** Let $\mathsf{I}$ and $\mathsf{C}$ be categories. Let $F:\mathsf{I}\to \mathsf{C}$. Suppose $A$ is an object in $\mathsf{C}$. A **cone** $(A,\nu)$ over $F$ consists of
- an object $A$ in $\mathsf{C}$ and
- a natural transformation $\nu:\Delta_{A}\Rightarrow F$. 

That is, a cone over $F$ consists of an object $A$ in $\mathsf{C}$ and a collection of morphisms $\nu_{X}:A\to F(X)$ in $\mathsf{C}$ for each object $X$ in $\mathsf{I}$ such that for all morphisms $f:X\to Y$ in $\mathsf{I}$ the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
A & \\
F(X) & F(Y)
\arrow["\nu_X", from=1-1, to=2-1, swap]
\arrow["F(f)", from=2-1, to=2-2, swap]
\arrow["\nu_Y", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. The object $A$ is called the **summit** of the cone, and the morphism $\nu_{X}$ is called the **leg** of the cone at $X$.

A **cocone** $(A,\sigma)$ over $F$ with **summit** $A$ consists of
- an object $A$ in $\mathsf{C}$ and
- a natural transformation $\sigma:F\Rightarrow \Delta_{A}$.

That is, a cocone over $F$ consists of an object $A$ in $\mathsf{C}$ collection of morphisms $\sigma_{X}:F(X)\to A$ in $\mathsf{C}$ for each object $X$ in $\mathsf{I}$ such that for all morphisms $f:X\to Y$ in $\mathsf{I}$ the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(X) & F(Y) \\
A &
\arrow["F(f)", from=1-1, to=1-2]
\arrow["\sigma_X", from=1-1, to=2-1, swap]
\arrow["\sigma_Y", from=1-2, to=2-1]
\end{tikzcd}
\end{document}
```

commutes. The object $A$ is called the **nadir** of the cocone, and the morphism $\sigma_{X}$ is called the **leg** of the cocone at $X$.

If $\mathsf{I}$ is small, then the collection of cones and cocones over $F$ forms a set. The set of all cones over $F$ with summit $A$ is denoted as $\text{Cone}(A,F)$, and the set of all cocones over $F$ with nadir $A$ is denoted as $\text{Cone}(F,A)$.
***
Definitions used;
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Constant Functor]]
- [[Natural Transformation]]