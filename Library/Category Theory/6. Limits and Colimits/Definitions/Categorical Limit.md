**Definition.** Let $\mathsf{C}$ and $\mathsf{S}$ be categories, and suppose that $\mathsf{S}$ is small. Let $F:\mathsf{S}\to \mathsf{C}$ be a functor. A **limit** of $F$ consists of
- an object $L$ in $\mathsf{C}$ and
- a natural transformation $\nu:\Delta_{L}\Rightarrow F$

such that for all objects $A$ in $\mathsf{C}$ and natural transformations $\sigma:\Delta_{A}\Rightarrow F$ there is a unique morphism $f:A\to L$ making the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
A & \\
L & F(X)
\arrow["f", from=1-1, to=2-1, swap]
\arrow["\nu_X", from=2-1, to=2-2]
\arrow["\sigma_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commute for all objects $X$ in $\mathsf{S}$.