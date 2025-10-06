**Definition.** Let $\mathsf{C}$ be a category. The limit of a functor $F:\mathsf{Par}\to \mathsf{C}$, if it exists, is called the **equalizer** of $F$. It is denoted as $\text{eq}(F)$.

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

is the image of $\mathsf{Par}$ under $F$. Then, $\text{eq}(F)$ may be denoted as $\text{eq}(f,g)$.

Given a description of the image of $F$ above, a cone over $F$ consists of an object $A$ together with morphisms $a_{X}:A\to X$ and $a_{Y}:A\to Y$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
A & \\
X & Y
\arrow["a_X", from=1-1, to=2-1, swap]
\arrow["a_Y", from=1-1, to=2-2]
\arrow["f", from=2-1, to=2-2, shift left=1]
\arrow["g", from=2-1, to=2-2, shift right=1, swap]
\end{tikzcd}
\end{document}
```

commutes. Commutativity here means $f\circ a_{X}=a_{Y}$ and $g\circ a_{X}=a_{Y}$, so $f\circ a_{X}=g\circ a_{X}$; hence, $a_{Y}$ is completely determined from $a_{X}$. We can therefore conclude that a cone over $F$ simply consists of an object $A$ and a morphism $a:A\to X$ such that $f\circ a=g\circ a$.

Explicitly, the limit property of $\text{eq}(f,g)$ therefore states that
- $\text{eq}(f,g)$ is equipped with a morphism $e: \text{eq}(f,g)\to X$ satisfying $f\circ e=g\circ e$ and
- for all objects $A$ equipped with a morphism $a:A\to X$ satisfying $f\circ a=g\circ a$, there is a unique morphism $k:A\to \text{eq}(f,g)$ such that $a=e\circ k$.

***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Cone and Cocone]]
- [[Categorical Limit and Colimit]]
- [[Parallel Category]]