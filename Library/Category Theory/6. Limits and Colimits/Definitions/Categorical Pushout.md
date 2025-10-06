**Definition.** Let $\mathsf{C}$ be a category. The colimit of a functor $F:\mathsf{Sp}^\text{op}\to \mathsf{C}$, if it exists, is called the **pushout** of $F$.

Suppose that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & B \\
A & Z
\arrow["f", from=2-2, to=2-1]
\arrow["g", from=2-2, to=1-2, swap]
\end{tikzcd}
\end{document}
```

is the image of $\mathsf{Sp}^\text{op}$ under $F$. Then, the pushout of $F$ may be denoted as $A+_{Z}B$.

Given a description of the image of $F$ above, a cocone over $F$ consists of an object $P$ together with morphisms $p_{A}:A\to P$, $p_{B}:B\to P$, and $p_{Z}:Z\to P$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
Z & B \\
A & P
\arrow["f", from=1-1, to=2-1, swap]
\arrow["g", from=1-1, to=1-2]
\arrow["p_A", from=2-1, to=2-2, swap]
\arrow["p_B", from=1-2, to=2-2]
\arrow["p_Z" description, from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. Commutativity here means $p_{A}\circ f=p_{Z}$ and $p_{B}\circ g=p_{Z}$, so $p_{A}\circ f=p_{B}\circ g$; hence, $p_{Z}$ is completely determined from $p_{A}$ and $p_{B}$. We can therefore conclude that a cone over $F$ simply consists of an object $P$ together with morphisms $p_{A}:A\to P$ and $p_{B}:B\to P$ such that $p_{A}\circ f=p_{B}\circ g$.

Explicitly, the limit property of $A+_{Z}B$ therefore states that
- $A+_{Z}B$ is equipped with morphisms $\iota_{A}:A\to A+_{Z}B$ and $\iota_{B}:B\to A+_{Z}B$ satisfying $\iota_{A}\circ f=\iota_{B}\circ g$ and
- for all objects $P$ equipped with morphisms $p_{A}:A\to P$ and $p_{B}:B\to P$ satisfying $p_{A}\circ f=p_{B}\circ g$, there is a unique morphism $k:A+_{Z}B\to P$ such that $p_{A}=k\circ \iota_{A}$ and $p_{B}=k\circ \iota_{B}$.

***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Cone and Cocone]]
- [[Categorical Limit and Colimit]]
- [[Span Category]]