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
**Proof of First Statement.** Suppose $a$ is an object in $\mathsf{C}$. We have
$$\begin{align}
(K(\sigma\circ \nu))_{a} & =K((\sigma \circ \nu)_{a}) \\
 & =K(\sigma_{a}\circ \nu_{a}) \\
 & =K(\sigma_{a})\circ K(\nu_{a}) \\
 & =(K\sigma)_{a}\circ(K\nu_{a}) \\
 & =(K\sigma\circ K\nu)_{a}.
\end{align}$$
Therefore, $K(\sigma\circ \nu)=K\sigma\circ K\nu$. $\blacksquare$

**Proof of Second Statement.** Suppose $a$ is an object in $\mathsf{C}$. We have
$$\begin{align}
((\sigma\circ \nu)K)_{a} & =(\sigma\circ \nu)_{K(a)} \\
 & =\sigma_{K(a)}\circ \nu_{K(a)} \\
 & =(\sigma K)_{a}\circ(\nu K)_{a} \\
 & =(\sigma K\circ \nu K)_{a}.
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