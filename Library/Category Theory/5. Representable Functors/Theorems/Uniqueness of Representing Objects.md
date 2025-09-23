**Theorem.** Let $\mathsf{C}$ be a locally small category. Let $F:\mathsf{C}\to \mathsf{Set}$ and $G:\mathsf{C}\to \mathsf{Set}$, and suppose $\nu:F\Rightarrow G$ is a natural isomorphism. Let $(x,\alpha)$ be a representation of $F$, and let $(y,\beta)$ be a representation of $G$. Then, there is a unique isomorphism $f:y\to x$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
h^x & F \\
h^y & G
\arrow["\alpha", from=1-1, to=1-2]
\arrow["h^f", from=1-1, to=2-1]
\arrow["\beta", from=2-1, to=2-2]
\arrow["\nu", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes.

Likewise, let $F:\mathsf{C}^\text{op}\to \mathsf{Set}$ and $G:\mathsf{C}^\text{op}\to \mathsf{Set}$, and suppose $\nu:F\Rightarrow G$ is a natural isomorphism. Let $(x,\alpha)$ be a representation of $F$, and let $(y,\beta)$ be a representation of $G$. Then, there is a unique isomorphism $f:x\to y$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
h_x & F \\
h_y & G
\arrow["\alpha", from=1-1, to=1-2]
\arrow["h_f", from=1-1, to=2-1]
\arrow["\beta", from=2-1, to=2-2]
\arrow["\nu", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes.

**Proof of First Statement.** By [[Isomorphism Relation as Equivalence Relation]], $\beta^{-1}\circ \nu\circ \alpha:h^x\Rightarrow h^y$ is a natural isomorphism. By [[Fullness and Faithfulness of Yoneda Embeddings]], $h^{\bullet}$ is full and faithful, so there is a unique morphism $f:y\to x$ such that $$\beta^{-1}\circ \nu\circ \alpha=h^f.$$By [[Induced Natural Transformations From Isomorphisms as Natural Isomorphisms]], since $h^f$ is an isomorphism, $f$ is also an isomorphism. By definition, $h^f$ makes the diagram posed in the statement commutes. $\blacksquare$

**Proof of Second Statement.** This follows by applying [[Principle of Duality]] on the first statement. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Locally Small Category]]
- [[Functor]]
- [[Covariant and Contravariant Functor]]
- [[Natural Isomorphism]]
- [[Representable Functor]]
- [[Category of Sets]]

Theorems used:
- [[Isomorphism Relation as Equivalence Relation]]
- [[Principle of Duality]]
- [[Fullness and Faithfulness of Yoneda Embeddings]]
- [[Induced Natural Transformations From Isomorphisms as Natural Isomorphisms]]