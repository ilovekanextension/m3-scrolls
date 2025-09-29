**Theorem.** Let $\mathsf{C}$ be a locally small category. Let $f:X\to Y$ be a morphism in $\mathsf{C}$. Then, the transformation $\nu$ from $h^Y$ to $h^X$ defined as $$\nu_{A}=-\circ f:\mathsf{C}(Y,A)\to \mathsf{C}(X,A)$$is a natural transformation. Likewise, the transformation $\sigma$ from $h_{X}$ to $h_{Y}$ defined as $$\sigma_{A}=f\circ -:\mathsf{C}(A,X)\to \mathsf{C}(A,Y)$$is a natural transformation.

**Proof of First Statement.** Suppose $s:A\to B$ is a morphism in $\mathsf{C}$. Consider the following diagram.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{C}(Y,A) & \mathsf{C}(Y,B) \\
\mathsf{C}(X,A) & \mathsf{C}(X,B)
\arrow["s\circ -", from=1-1, to=1-2]
\arrow["\nu_A", from=1-1, to=2-1]
\arrow["s\circ -", from=2-1, to=2-2]
\arrow["\nu_B", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

By [[Evaluations of Composite Functions]], for all $t:Y\to A$ we have 
$$\begin{align}
[\nu_{B}\circ(s\circ -)](t) & =\nu_{B}(s\circ t) \\
 & =(s\circ t)\circ f \\
 & =s\circ (t\circ f) \\
 & =[(s\circ -)](\nu_{A}(t)) \\
 & =[(s\circ -)\circ \nu_{A}](t).
\end{align}$$
Therefore, by [[Extensionality of Functions]] $\nu_{B}\circ (s\circ -)=(s\circ -)\circ \nu_{A}$, so the diagram commutes. $\blacksquare$

**Proof of Second Statement.** Suppose $s:A\to B$ is a morphism in $\mathsf{C}$. Consider the following diagram.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{C}(B,X) & \mathsf{C}(A,X) \\
\mathsf{C}(B,Y) & \mathsf{C}(A,Y)
\arrow["-\circ s", from=1-1, to=1-2]
\arrow["\sigma_B", from=1-1, to=2-1]
\arrow["-\circ s", from=2-1, to=2-2]
\arrow["\sigma_A", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

By [[Evaluations of Composite Functions]], for all $t:B\to X$ we have 
$$\begin{align}
[\sigma_{A}\circ(-\circ s)](t) & =\sigma_{A}(t\circ s) \\
 & =f\circ (t\circ s) \\
 & =(f\circ t)\circ s \\
 & =[(-\circ s)](f\circ t) \\
 & =[(-\circ s)\circ \sigma_{B}](t).
\end{align}$$
Therefore, by [[Extensionality of Functions]] $\sigma_{A}\circ (-\circ s)=(-\circ s)\circ \sigma_{B}$, so the diagram commutes. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Locally Small Category]]
- [[Categorical Diagram]]
- [[Natural Transformation]]
- [[Hom-Functor]]
- [[Function]]
- [[Composition of Functions]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]