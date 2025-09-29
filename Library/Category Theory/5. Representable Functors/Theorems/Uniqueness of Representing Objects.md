**Theorem.** Let $\mathsf{C}$ be a locally small category. Let $F:\mathsf{C}\to \mathsf{Set}$ and $G:\mathsf{C}\to \mathsf{Set}$, and suppose $\nu:F\Rightarrow G$ is a natural isomorphism. Let $(X,\alpha)$ be a representation of $F$, and let $(Y,\beta)$ be a representation of $G$. Then, there is a unique isomorphism $f:Y\to X$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
h^X & F \\
h^Y & G
\arrow["\alpha", from=1-1, to=1-2]
\arrow["h^f", from=1-1, to=2-1]
\arrow["\beta", from=2-1, to=2-2]
\arrow["\nu", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes.

Likewise, let $F:\mathsf{C}^\text{op}\to \mathsf{Set}$ and $G:\mathsf{C}^\text{op}\to \mathsf{Set}$, and suppose $\nu:F\Rightarrow G$ is a natural isomorphism. Let $(X,\alpha)$ be a representation of $F$, and let $(Y,\beta)$ be a representation of $G$. Then, there is a unique isomorphism $f:X\to Y$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
h_X & F \\
h_Y & G
\arrow["\alpha", from=1-1, to=1-2]
\arrow["h_f", from=1-1, to=2-1]
\arrow["\beta", from=2-1, to=2-2]
\arrow["\nu", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes.

**Proof of First Statement.** The natural transformation $\beta^{-1}\circ \nu\circ \alpha:h^X\Rightarrow h^Y$ is an isomorphism, so by [[Fullness and Faithfulness of Yoneda Embeddings]] and [[Natural Transformations Induced From Isomorphisms as Natural Isomorphisms]] there is a unique isomorphism $f:Y\to X$ such that $h^f=\beta^{-1}\circ \nu\circ \alpha$. We then have $\beta\circ h^f=\nu\circ \alpha$, so the diagram posed commutes. $\blacksquare$

**Proof of Second Statement.** The natural transformation $\beta^{-1}\circ \nu\circ \alpha:h^X\Rightarrow h^Y$ is an isomorphism, so by [[Fullness and Faithfulness of Yoneda Embeddings]] and [[Natural Transformations Induced From Isomorphisms as Natural Isomorphisms]] there is an isomorphism $f:X\to Y$ such that $h_{f}=\beta^{-1}\circ \nu\circ \alpha$. We then have $\beta\circ h_{f}=\nu\circ \alpha$, so the diagram posed commutes. $\blacksquare$
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
- [[Fullness and Faithfulness of Yoneda Embeddings]]
- [[Natural Transformations Induced From Isomorphisms as Natural Isomorphisms]]