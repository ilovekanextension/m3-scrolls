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
\arrow["J", from=1-2, to=1-3, bend left=50]
\arrow["K" description, from=1-2, to=1-3]
\arrow["L", from=1-2, to=1-3, bend right=50, swap]
\arrow[""{name=f}, phantom, from=1-1, to=1-2, bend left=50]
\arrow[""{name=g1, above}, phantom, from=1-1, to=1-2]
\arrow[""{name=g2, below}, phantom, from=1-1, to=1-2]
\arrow[""{name=h}, phantom, from=1-1, to=1-2, bend right=50]
\arrow["\nu"{inner sep=0.8ex}, from=f, to=g1, Rightarrow]
\arrow["\sigma"{inner sep=0.8ex}, from=g2, to=h, Rightarrow]
\arrow[""{name=j}, phantom, from=1-2, to=1-3, bend left=50]
\arrow[""{name=k1, above}, phantom, from=1-2, to=1-3]
\arrow[""{name=k2, below}, phantom, from=1-2, to=1-3]
\arrow[""{name=ell}, phantom, from=1-2, to=1-3, bend right=50]
\arrow["\eta"{inner sep=0.8ex}, from=j, to=k1, Rightarrow]
\arrow["\varepsilon"{inner sep=0.8ex}, from=k2, to=ell, Rightarrow]
\end{tikzcd}
\end{document}
```

Then, $$(\varepsilon*\sigma)\circ(\eta*\nu)=(\varepsilon\circ \eta)*(\sigma\circ \nu).$$
**Proof.** By [[Horizontal Composites as Vertical Compositions of Whiskerings]] and [[Distributivity of Whiskerings Over Vertical Compositions]], we have
$$\begin{align}
(\varepsilon*\sigma)\circ(\eta*\nu) & =(L\sigma\circ\varepsilon G)\circ(K\nu\circ \eta F) \\
 & =L\sigma\circ(\varepsilon G\circ K\nu)\circ \eta F \\
 & =L\sigma\circ(L\nu\circ \varepsilon F)\circ \eta F \\
 & =(L\sigma\circ L\nu)\circ(\varepsilon F\circ \eta F) \\
 & =L(\sigma\circ \nu)\circ(\varepsilon\circ \eta)F \\
 & =(\varepsilon\circ \eta)*(\sigma\circ \nu).\blacksquare
\end{align}$$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Natural Transformation]]
- [[Vertical Composition of Natural Transformations]]
- [[Horizontal Composition of Natural Transformations]]
- [[Whiskering]]

Theorems used:
- [[Horizontal Composites as Vertical Compositions of Whiskerings]]
- [[Distributivity of Whiskerings Over Vertical Compositions]]