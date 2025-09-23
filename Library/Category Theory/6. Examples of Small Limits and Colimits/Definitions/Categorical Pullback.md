**Definition.** Let $\mathsf{C}$ be a category. Let $a,b,$ and $c$ be objects in $\mathsf{C}$. Let $f:a\to c$ and $g:b\to c$ be morphisms in $\mathsf{C}$. A **pullback** of $f$ and $g$ consists of
- an object $p$,
- a morphism $\phi_{1}:p\to a$, and
- a morphism $\phi_{2}:p\to b$

such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
p & a \\
b & c
\arrow["\phi_1", from=1-1, to=1-2]
\arrow["\phi_2", from=1-1, to=2-1, swap]
\arrow["g", from=2-1, to=2-2]
\arrow["f", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes and for all objects $q$ and morphisms $x:q\to a$ and $y:q\to b$ making the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
q & a \\
b & c
\arrow["x", from=1-1, to=1-2]
\arrow["y", from=1-1, to=2-1, swap]
\arrow["g", from=2-1, to=2-2]
\arrow["f", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commute, there is a unique morphism $k:p\to q$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & p & \\
b & q & a \\
\arrow["k" description, from=1-2, to=2-2]
\arrow["y", from=2-2, to=2-1]
\arrow["x", from=2-2, to=2-3, swap]
\arrow["\phi_2", from=1-2, to=2-1]
\arrow["\phi_1", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

commutes.