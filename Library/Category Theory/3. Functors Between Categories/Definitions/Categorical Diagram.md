**Definition.** Let $\mathsf{C}$ be a category. A **diagram** of $\mathsf{C}$ is a collection of objects and morphisms in $\mathsf{C}$ that is closed under composition and identities. That is,
- if $A$ is an object in the diagram, then $\text{id}_{A}$ is also in the diagram, and
- if $f:A\to B$ and $g:B\to C$ are morphisms in the diagram, then $g\circ f:A\to C$ is also in the diagram.

Formally, a diagram of $\mathsf{C}$ is therefore just (the image of) a functor $F$ from a small category $\mathsf{I}$ to $\mathsf{C}$. We proceed to say that $\mathsf{I}$ is the **index** of $F$ and that $F$ has the **shape** of $\mathsf{I}$.

Diagrams are usually depicted visually as directed edges between vertices as follows.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
A & B \\
 & C
\arrow["f", from=1-1, to=1-2]
\arrow["g", from=1-2, to=2-2]
\arrow["h", from=1-1, to=2-2, swap]
\end{tikzcd}
\end{document}
```

We say that a diagram **commutes** or **is commutative** if for all morphisms $f$ and $g$ in the diagram sharing the same source and target, we have $f=g$. For example, commutativity of the diagram above means $g\circ f=h$.
***
Definitions used:
- [[Category]]
- [[Functor]]