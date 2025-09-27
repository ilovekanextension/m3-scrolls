**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F,G,H:\mathsf{C}\to \mathsf{D}$. Let $\nu:F\Rightarrow G$ and $\sigma:G\Rightarrow H$. Then, the transformation $\alpha$ from $F$ to $H$ defined as $$\alpha_{A}=\sigma_{A}\circ \nu_{A}$$is a natural transformation.

**Proof.** Suppose $f:A\to B$ is a morphism in $\mathsf{C}$. Consider the following diagram (1).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(A) & F(B) \\
H(A) & H(B)
\arrow["F(f)", from=1-1, to=1-2]
\arrow["\alpha_A", from=1-1, to=2-1]
\arrow["H(f)", from=2-1, to=2-2]
\arrow["\alpha_B", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

By definition, $\alpha_{A}=\sigma_{A}\circ \nu_{A}$ and $\alpha_{B}=\sigma_{B}\circ \nu_{B}$. We can therefore extend (1) into the following diagram (2).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(A) & F(B) \\
G(A) & G(B) \\
H(A) & H(B)
\arrow["F(f)", from=1-1, to=1-2]
\arrow["G(f)", from=2-1, to=2-2]
\arrow["H(f)", from=3-1, to=3-2]
\arrow["\nu_A", from=1-1, to=2-1]
\arrow["\sigma_A", from=2-1, to=3-1]
\arrow["\nu_B", from=1-2, to=2-2]
\arrow["\sigma_B", from=2-2, to=3-2]
\arrow["\alpha_A" description, from=1-1, to=3-1, dashed, bend right=50]
\arrow["\alpha_B" description, from=1-2, to=3-2, dashed, bend left=50]
\end{tikzcd}
\end{document}
```

Since $\nu$ is a natural transformation, the upper square in (2) commutes. Since $\sigma$ is a natural transformation, the lower square in (2) commutes. Therefore, by [[Compositions of Commutative Squares as Commutative Squares]], the outer square of (2), which is precisely (1), also commutes. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Natural Transformation]]

Theorems used:
- [[Compositions of Commutative Squares as Commutative Squares]]