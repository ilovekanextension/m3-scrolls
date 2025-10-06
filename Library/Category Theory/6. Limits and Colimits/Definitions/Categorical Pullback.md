**Definition.** Let $\mathsf{C}$ be a category. The limit of a functor $F:\mathsf{Sp}\to \mathsf{C}$, if it exists, is called the **pullback** of $F$.

Suppose that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & B \\
A & Z
\arrow["f", from=2-1, to=2-2]
\arrow["g", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

is the image of $\mathsf{Sp}$ under $F$. Then, the pullback of $F$ may be denoted as $A\times_{Z}B$.

Given a description of the image of $F$ above, a cone over $F$ consists of an object $P$ together with morphisms $p_{A}:P\to A$, $p_{B}:P\to B$, and $p_{Z}:P\to Z$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
P & B \\
A & Z
\arrow["p_B", from=1-1, to=1-2]
\arrow["p_A", from=1-1, to=2-1, swap]
\arrow["f", from=2-1, to=2-2, swap]
\arrow["g", from=1-2, to=2-2]
\arrow["p_Z" description, from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. Commutativity here means $f\circ p_{A}=p_{Z}$ and $g\circ p_{B}=p_{Z}$, so $f\circ p_{A}=g\circ p_{B}$; hence, $p_{Z}$ is completely determined from $p_{A}$ and $p_{B}$. We can therefore conclude that a cone over $F$ simply consists of an object $P$ together with morphisms $p_{A}:P\to A$ and $p_{B}:P\to B$ such that $f\circ p_{A}=g\circ p_{B}$.

Explicitly, the limit property of $A\times_{Z}B$ therefore states that
- $A\times_{Z}B$ is equipped with morphisms $\pi_{A}:A\times_{Z}B\to A$ and $\pi_{B}:A\times_{Z}B\to B$ satisfying $f\circ \pi_{A}=g\circ \pi_{B}$ and
- for all objects $P$ equipped with morphisms $p_{A}:P\to A$ and $p_{B}:P\to B$ satisfying $f\circ p_{A}=g\circ p_{B}$, there is a unique morphism $k:P\to A\times_{Z}B$ such that $p_{A}=\pi_{A}\circ k$ and $p_{B}=\pi_{B}\circ k$.

***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Cone and Cocone]]
- [[Categorical Limit and Colimit]]
- [[Span Category]]