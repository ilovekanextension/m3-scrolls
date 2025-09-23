**Theorem.** Let $\mathsf{C}$ be a locally small category. Let $f:x\to y$ be a morphism in $\mathsf{C}$. Then, the map $\nu$ that assigns to each object $a$ in $\mathsf{C}$ the pre-composition function $$-\circ f:\mathsf{C}(y,a)\to \mathsf{C}(x,a)$$is a natural transformation from $h^y$ to $h^x$. Likewise, the map $\nu$ that assigns to each object $a$ in $\mathsf{C}$ the post-composition function $$f\circ -:\mathsf{C}(a,x)\to \mathsf{C}(a,y)$$is a natural transformation from $h_{x}$ to $h_{y}$.

**Proof of First Statement.** Suppose $s:a\to b$ is a morphism in $\mathsf{C}$. Consider the following diagram.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{C}(y,a) & \mathsf{C}(y,b) \\
\mathsf{C}(x,a) & \mathsf{C}(x,b)
\arrow["s\circ -", from=1-1, to=1-2]
\arrow["\nu_a", from=1-1, to=2-1]
\arrow["s\circ -", from=2-1, to=2-2]
\arrow["\nu_b", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

By [[Evaluations of Composite Functions]], for all $t:y\to a$ we have 
$$\begin{align}
\nu_{b}\circ(s\circ -)(t) & =\nu_{b}(s\circ t) \\
 & =(s\circ t)\circ f \\
 & =s\circ (t\circ f) \\
 & =(s\circ -)(\nu_{a}(t)) \\
 & =(s\circ -)\circ \nu_{a}(t).
\end{align}$$
Therefore, by [[Extensionality of Functions]] $\nu_{b}\circ (s\circ -)=(s\circ -)\circ \nu_{a}$, so the diagram commutes. $\blacksquare$

**Proof of Second Statement.** This follows by applying [[Principle of Duality]] on the first statement. $\blacksquare$
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
- [[Principle of Duality]]
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]