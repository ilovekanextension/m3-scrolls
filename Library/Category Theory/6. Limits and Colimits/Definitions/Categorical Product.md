**Definition.** Let $\mathsf{C}$ be a category. Let $\mathsf{D}$ be a small discrete category. The limit of a functor $F:\mathsf{D}\to \mathsf{C}$ is called the **product** of $F$. It is denoted as $\prod F$. The leg of $\prod F$ at an object $X$ in $\mathsf{D}$ is denoted as $\pi_{X}$ and is called the **projection** at $X$.

Explicitly, the limit property of $\prod F$ states that
- $\prod F$ is equipped with morphisms $\pi_{X}:\prod F\to X$ for each object $X$ in $\mathsf{D}$ and
- for all objects $A$ in $\mathsf{C}$ equipped with morphisms $f_{X}:A\to X$ for each object $X$ in $\mathsf{D}$, there is a unique morphism $g:A\to \prod F$ such that $$f_{X}=\pi_{X}\circ g$$for all objects $X$ in $\mathsf{D}$.

When $\mathsf{D}$ consists of only two objects, call $X_{A}$ and $X_{B}$, $\prod F$ is usually denoted as $$A\times B,$$where $A$ and $B$ are the images of $X_{A}$ and $X_{B}$ under $F$ respectively. The projection morphisms are denoted more specifically as $\pi_{A}:A\times B\to A$ and $\pi_{B}:A\times B\to B$. The limit property states that for all objects $P$ with morphisms $f_{A}:P\to A$ and $f_{B}:P\to B$ there is a unique morphism $g:P\to A\times B$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}[row sep=large]
 & P & \\
A & A\times B & B
\arrow["g" description, from=1-2, to=2-2]
\arrow["f_A", from=1-2, to=2-1, swap]
\arrow["f_B", from=1-2, to=2-3]
\arrow["\pi_A", from=2-2, to=2-1]
\arrow["\pi_B", from=2-2, to=2-3, swap]
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