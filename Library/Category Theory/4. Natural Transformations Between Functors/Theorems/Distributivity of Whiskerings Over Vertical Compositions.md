**Theorem.** Let the following be a diagram in $\mathsf{Cat}$ or $\mathsf{LCat}$.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{C} & \mathsf{D} & \mathsf{E}
\arrow["F", from=1-1, to=1-2, bend left=50]
\arrow["G" description, from=1-1, to=1-2]
\arrow["H", from=1-1, to=1-2, bend right=50, swap]
\arrow["K", from=1-2, to=1-3]
\arrow[""{name=f}, phantom, from=1-1, to=1-2, bend left=50]
\arrow[""{name=g1, above}, phantom, from=1-1, to=1-2]
\arrow[""{name=g2, below}, phantom, from=1-1, to=1-2]
\arrow[""{name=h}, phantom, from=1-1, to=1-2, bend right=50]
\arrow["\nu"{inner sep=0.8ex}, from=f, to=g1, Rightarrow]
\arrow["\sigma"{inner sep=0.8ex}, from=g2, to=h, Rightarrow]
\end{tikzcd}
\end{document}
```

Then, $$K(\sigma\circ \nu)=K\sigma\circ K\nu.$$Likewise, let the following be a diagram in $\mathsf{Cat}$ or $\mathsf{LCat}$.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{C} & \mathsf{D} & \mathsf{E}
\arrow["F", from=1-2, to=1-3, bend left=50]
\arrow["G" description, from=1-2, to=1-3]
\arrow["H", from=1-2, to=1-3, bend right=50, swap]
\arrow["K", from=1-1, to=1-2]
\arrow[""{name=f}, phantom, from=1-2, to=1-3, bend left=50]
\arrow[""{name=g1, above}, phantom, from=1-2, to=1-3]
\arrow[""{name=g2, below}, phantom, from=1-2, to=1-3]
\arrow[""{name=h}, phantom, from=1-2, to=1-3, bend right=50]
\arrow["\nu"{inner sep=0.8ex}, from=f, to=g1, Rightarrow]
\arrow["\sigma"{inner sep=0.8ex}, from=g2, to=h, Rightarrow]
\end{tikzcd}
\end{document}
```

Then, $$(\sigma\circ \nu)K=\sigma K\circ \nu K.$$
**Proof of First Statement.** For all objects $A$ in $\mathsf{C}$ we have
$$\begin{align}
(K(\sigma\circ \nu))_{A} & =K((\sigma \circ \nu)_{A}) \\
 & =K(\sigma_{A}\circ \nu_{A}) \\
 & =K(\sigma_{A})\circ K(\nu_{A}) \\
 & =(K\sigma)_{A}\circ(K\nu_{A}) \\
 & =(K\sigma\circ K\nu)_{A}.
\end{align}$$
Therefore, $K(\sigma\circ \nu)=K\sigma\circ K\nu$. $\blacksquare$

**Proof of Second Statement.** For all objects $A$ in $\mathsf{C}$ we have
$$\begin{align}
((\sigma\circ \nu)K)_{A} & =(\sigma\circ \nu)_{K(A)} \\
 & =\sigma_{K(A)}\circ \nu_{K(A)} \\
 & =(\sigma K)_{A}\circ(\nu K)_{A} \\
 & =(\sigma K\circ \nu K)_{A}.
\end{align}$$
Therefore, $(\sigma\circ \nu)K=\sigma K\circ \nu K$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Natural Transformation]]
- [[Vertical Composition of Natural Transformations]]
- [[Whiskering]]