**Definition.** Up to isomorphism, the **span category** $\mathsf{Sp}$ is the category that consists of three objects $A$, $B$, and $R$ (with their corresponding identity morphisms) and two morphisms $m_{A}:A\to R$ and $m_{B}:B\to R$. Visually, it is completely described by the following diagram.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
 & B \\
A & R
\arrow["m_A", from=2-1, to=2-2]
\arrow["m_B", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

By definition, $\text{Ob}(\mathsf{Sp})=\{A,B,R\}$. Therefore, $\mathsf{Sp}$ is a small category.
***
Definitions used:
- [[Category]]
- [[Small Category]]
- [[Categorical Diagram]]