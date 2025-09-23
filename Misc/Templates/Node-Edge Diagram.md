Use as template for categorical diagrams.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(a) & F(b) \\
G(a) & G(b)
\arrow["F(f)", from=1-1, to=1-2]
\arrow["\nu_a", from=1-1, to=2-1]
\arrow["G(f)", from=2-1, to=2-2]
\arrow["\nu_b", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```