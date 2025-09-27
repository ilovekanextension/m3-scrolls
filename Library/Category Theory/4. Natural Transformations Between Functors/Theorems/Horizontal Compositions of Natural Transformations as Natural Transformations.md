**Theorem.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories. Let $F,G:\mathsf{C}\to \mathsf{D}$ and $H,K:\mathsf{D}\to \mathsf{E}$. Let $\nu:F\Rightarrow G$ and $\sigma:H\Rightarrow K$. Then, the transformation $\eta$ from $H\circ F$ to $K\circ G$ defined as $$\eta_{A}=K(\nu_{A})\circ \sigma_{F(A)}$$is a natural transformation.

**Proof.** Suppose $f:A\to B$ is a morphism in $\mathsf{C}$. Consider the following diagram (1).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
H\circ F(A) & H\circ F(B) \\
K\circ G(A) & K\circ G(B)
\arrow["H(F(f))", from=1-1, to=1-2]
\arrow["\eta_A", from=1-1, to=2-1]
\arrow["K(G(f))", from=2-1, to=2-2]
\arrow["\eta_B", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

By definition of $\eta$, we can extend (1) into the following diagram (2).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
H\circ F(A) & H\circ F(B) \\
K\circ F(A) & K\circ F(B) \\
K\circ G(A) & K\circ G(B)
\arrow["H(F(f))", from=1-1, to=1-2]
\arrow["K(F(f))", from=2-1, to=2-2]
\arrow["K(G(f))", from=3-1, to=3-2]
\arrow["\sigma_{F(A)}", from=1-1, to=2-1]
\arrow["K(\nu_A)", from=2-1, to=3-1]
\arrow["\sigma_{F(B)}", from=1-2, to=2-2]
\arrow["K(\nu_B)", from=2-2, to=3-2]
\arrow["\eta_A" description, from=1-1, to=3-1, dashed, bend right=70]
\arrow["\eta_B" description, from=1-2, to=3-2, dashed, bend left=70]
\end{tikzcd}
\end{document}
```

Since $\sigma$ is a natural transformation, the upper square of (2) commutes. Since $\nu$ is a natural transformation, the lower square of (2) commutes. Therefore, by [[Compositions of Commutative Squares as Commutative Squares]], the outer square of (2), which is precisely (1), also commutes. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Composition of Functors]]
- [[Natural Transformation]]

Theorems used:
- [[Compositions of Commutative Squares as Commutative Squares]]