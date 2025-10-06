**Definition.** Up to isomorphism, the **parallel category** $\mathsf{Par}$ is the category that consists of two objects $S$ and $T$ (together with their corresponding identity morphisms) and two distinct morphisms $m_{1}:S\to T$ and $m_{2}:S\to T$. Visually, it is completely described by the following diagram.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
S & T
\arrow["m_1", from=1-1, to=1-2, shift left=1]
\arrow["m_2", from=1-1, to=1-2, shift right=1, swap]
\end{tikzcd}
\end{document}
```

By definition, $\text{Ob}(\mathsf{Par})=\{S,T\}$. Therefore, $\mathsf{Par}$ is a small category.
***
Definitions used:
- [[Category]]
- [[Small Category]]
- [[Categorical Diagram]]