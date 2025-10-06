**Definition.** Let $\mathsf{C}$ be a category. The colimit of a functor $F:\mathsf{Par}\to \mathsf{C}$, if it exists, is called the **coequalizer** of $F$. It is denoted as $\text{coeq}(F)$.

Suppose that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
X & Y
\arrow["f", from=1-1, to=1-2, shift left=1]
\arrow["g", from=1-1, to=1-2, shift right=1, swap]
\end{tikzcd}
\end{document}
```

is the image of $\mathsf{Par}$ under $F$. Then, $\text{coeq}(F)$ may be denoted as $\text{coeq}(f,g)$.

Given a description of the image of $F$ above, a cocone over $F$ consists of an object $A$ together with morphisms $a_{X}:X\to A$ and $a_{Y}:Y\to A$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
X & Y \\
 & A
\arrow["a_X", from=1-1, to=2-2, swap]
\arrow["a_Y", from=1-2, to=2-2]
\arrow["f", from=1-1, to=1-2, shift left=1]
\arrow["g", from=1-1, to=1-2, shift right=1, swap]
\end{tikzcd}
\end{document}
```

commutes. Commutativity here means $a_{Y}\circ f=a_{X}$ and $a_{Y}\circ g=a_{X}$, so $a_{Y}\circ f=a_{Y}\circ g$; hence, $a_{X}$ is completely determined from $a_{Y}$. We can therefore conclude that a cocone over $F$ simply consists of an object $A$ and a morphism $a:Y\to A$ such that $a\circ f=a\circ g$.

Explicitly, the colimit property of $\text{coeq}(F)$ therefore states that
- $\text{coeq}(f,g)$ is equipped with a morphism $e:Y\to \text{coeq}(f,g)$ satisfying $e\circ f=e\circ g$ and
- for all objects $A$ equipped with a morphism $a:Y\to A$ satisfying $a\circ f=a\circ g$, there is a unique morphism $k: \text{coeq}(f,g)\to A$ such that $a=k\circ e$.

***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Cone and Cocone]]
- [[Categorical Limit and Colimit]]
- [[Parallel Category]]