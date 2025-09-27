**Theorem.** Let $\mathsf{C}$ be a category. Let the following be a diagram of $\mathsf{C}$.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
A_1 & B_1 \\
A_2 & B_2 \\
A_3 & B_3
\arrow["x_1", from=1-1, to=1-2]
\arrow["x_2", from=2-1, to=2-2]
\arrow["x_3", from=3-1, to=3-2]
\arrow["f", from=1-1, to=2-1]
\arrow["g", from=2-1, to=3-1]
\arrow["h", from=1-2, to=2-2]
\arrow["k", from=2-2, to=3-2]
\end{tikzcd}
\end{document}
```

Suppose that the upper and the lower squares both commute. Then, the outer square i.e. the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
A_1 & B_1 \\
A_3 & B_3
\arrow["x_1", from=1-1, to=1-2]
\arrow["x_3", from=2-1, to=2-2]
\arrow["g\circ f", from=1-1, to=2-1, swap]
\arrow["k\circ h", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

also commutes.

**Proof.** Since the upper square commutes, we have $x_{2}\circ f=h\circ x_{1}$. Since the lower square commutes, we have $x_{3}\circ g=k\circ x_{2}$. Therefore, using the associativity law we have
$$\begin{align}
x_{3}\circ(g\circ f) & =(x_{3}\circ g)\circ f \\
 & =(k\circ x_{2})\circ f \\
 & =k\circ (x_{2}\circ f) \\
 & =k\circ(h\circ x_{1}) \\
 & =(k\circ h)\circ x_{1},
\end{align}$$
which means the outer square commutes. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Categorical Diagram]]