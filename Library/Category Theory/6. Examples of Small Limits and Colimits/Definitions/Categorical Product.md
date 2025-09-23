**Definition.** Let $\mathsf{C}$ be a category. Let $a$ and $b$ be objects in $\mathsf{C}$. A **product** of $a$ with $b$ consists of
- an object $p$,
- a morphism $\pi_{1}:p\to a$, and
- a morphism $\pi_{2}:p\to b$

such that for all objects $x$ and morphisms $f:x\to a$ and $g:x\to b$, there is a unique morphism $k:x\to p$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & x & \\
a & p & b
\arrow["k" description, from=1-2, to=2-2]
\arrow["\pi_1", from=2-2, to=2-1]
\arrow["\pi_2", from=2-2, to=2-3, swap]
\arrow["f", from=1-2, to=2-1, swap]
\arrow["g", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

commutes.

By [[Uniqueness of Categorical Products]], the product of $a$ with $b$, if it exists, is unique up to isomorphism. Therefore, we may speak of **the** product of $a$ with $b$. The product of $a$ with $b$ is denoted as $a\times b$. The morphisms $\pi_{1}:a\times b\to a$ and $\pi_{2}:a\times b\to b$ are called the **left projection** and **right projection** of $a\times b$ respectively.
***
Definitions used:
- [[Category]]
- [[Categorical Diagram]]

Theorems used:
- [[Uniqueness of Categorical Products]]