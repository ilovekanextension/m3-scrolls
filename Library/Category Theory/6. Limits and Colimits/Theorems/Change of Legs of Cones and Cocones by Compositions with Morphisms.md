**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F:\mathsf{C}\to \mathsf{D}$. Suppose $f:A\to B$ is a morphism in $\mathsf{D}$.
1. Let $\sigma:\Delta_{B}\Rightarrow F$. Then, the transformation $\nu$ from $\Delta_{A}$ to $F$ defined as $$\nu_{X}=\sigma_{X}\circ f$$is also natural.
2. Let $\sigma:F\Rightarrow \Delta_{A}$. Then, the transformation $\nu$ from $F$ to $\Delta_{B}$ defined as $$\nu_{X}=f\circ\sigma_{X}$$is also natural.

**Proof of First Statement.** Suppose $s:X\to Y$ be a morphism in $\mathsf{C}$. Consider the following diagram (1).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
A & A \\
F(X) & F(Y)
\arrow["\text{id}_A", from=1-1, to=1-2]
\arrow["\nu_X", from=1-1, to=2-1, swap]
\arrow["F(s)", from=2-1, to=2-2]
\arrow["\nu_Y", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```


By definition, $\nu_{X}=\sigma_{X}\circ f$ and $\nu_{Y}=\sigma_{Y}\circ f$. We can therefore extend (1) into the following diagram (2).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
A & A \\
B & B \\
F(X) & F(Y)
\arrow["\text{id}_A", from=1-1, to=1-2]
\arrow["\text{id}_B", from=2-1, to=2-2]
\arrow["F(s)", from=3-1, to=3-2]
\arrow["f", from=1-1, to=2-1]
\arrow["\sigma_X", from=2-1, to=3-1]
\arrow["f", from=1-2, to=2-2]
\arrow["\sigma_Y", from=2-2, to=3-2]
\arrow["\nu_X" description, from=1-1, to=3-1, bend right=50, dashed]
\arrow["\nu_Y" description, from=1-2, to=3-2, bend left=50, dashed]
\end{tikzcd}
\end{document}
```

Clearly the upper square of (2) commutes. Since $\sigma$ is natural, the lower square of (2) also commutes. Therefore, by [[Compositions of Commutative Squares as Commutative Squares]] the outer square of (2), which is precisely (1), also commutes. $\blacksquare$

**Proof of Second Statement.** Suppose $s:X\to Y$ be a morphism in $\mathsf{C}$. Consider the following diagram (1).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(X) & F(Y) \\
B & B
\arrow["F(s)", from=1-1, to=1-2]
\arrow["\nu_X", from=1-1, to=2-1, swap]
\arrow["\text{id}_B", from=2-1, to=2-2]
\arrow["\nu_Y", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```


By definition, $\nu_{X}=f\circ \sigma_{X}$ and $\nu_{Y}=f\circ \sigma_{Y}$. We can therefore extend (1) into the following diagram (2).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(X) & F(Y) \\
A & A \\
B & B
\arrow["F(s)", from=1-1, to=1-2]
\arrow["\text{id}_A", from=2-1, to=2-2]
\arrow["\text{id}_B", from=3-1, to=3-2]
\arrow["\sigma_X", from=1-1, to=2-1]
\arrow["f", from=2-1, to=3-1]
\arrow["\sigma_Y", from=1-2, to=2-2]
\arrow["f", from=2-2, to=3-2]
\arrow["\nu_X" description, from=1-1, to=3-1, bend right=50, dashed]
\arrow["\nu_Y" description, from=1-2, to=3-2, bend left=50, dashed]
\end{tikzcd}
\end{document}
```

Clearly the lower square of (2) commutes. Since $\sigma$ is natural, the upper square of (2) also commutes. Therefore, by [[Compositions of Commutative Squares as Commutative Squares]] the outer square of (2), which is precisely (1), also commutes. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Constant Functor]]
- [[Natural Transformation]]