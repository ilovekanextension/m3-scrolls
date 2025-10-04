**Definition.** Let $\mathsf{C}$ be a category. Let $\mathsf{D}$ be a small discrete category. The colimit of a functor $F:\mathsf{D}\to \mathsf{C}$ is called the **coproduct** of $F$. It is denoted as $\coprod F$. The leg of $\coprod F$ at an object $X$ in $\mathsf{D}$ is denoted as $\iota_{X}$ and is called the **insertion** at $X$.

Explicitly, the limit property of $\coprod F$ states that
- $\coprod F$ is equipped with morphisms $\iota_{X}:X\to \coprod F$ for each object $X$ in $\mathsf{D}$ and
- for all objects $A$ in $\mathsf{C}$ equipped with morphisms $f_{X}:X\to A$ for each object $X$ in $\mathsf{D}$, there is a unique morphism $g:\coprod F\to A$ such that $$f_{X}=g\circ \iota_{X}$$for all objects $X$ in $\mathsf{D}$.

When $\mathsf{D}$ consists of only two objects, call $X_{A}$ and $X_{B}$, $\coprod F$ is usually denoted as $$A+B,$$where $A$ and $B$ are the images of $X_{A}$ and $X_{B}$ under $F$ respectively. The insertion morphisms are denoted more specifically as $\iota_{A}:A\to A+B$ and $\iota_{B}:B\to A+B$. The limit property states that for all objects $C$ with morphisms $f_{A}:A\to C$ and $f_{B}:B\to C$ there is a unique morphism $g:A+B\to C$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}[row sep=large]
A & A+B & B \\
 & C &
\arrow["g" description, from=1-2, to=2-2]
\arrow["f_A", from=1-1, to=2-2, swap]
\arrow["f_B", from=1-3, to=2-2]
\arrow["\iota_A", from=1-1, to=1-2]
\arrow["\iota_B", from=1-3, to=1-2, swap]
\end{tikzcd}
\end{document}
```

commutes.
***
Definitions used:
- [[Category]]
- [[Small Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Categorical Limit and Colimit]]
- [[Discrete Category]]