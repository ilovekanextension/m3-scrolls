**Theorem.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories. Let $F,G:\mathsf{C}\to \mathsf{D}$ and $H,K:\mathsf{D}\to \mathsf{E}$. Let $\nu:F\Rightarrow G$ and $\sigma:H\Rightarrow K$. Suppose $A$ is an object in $\mathsf{C}$. Then, the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
H\circ F(A) & H\circ G(A) \\
K\circ F(A) & K\circ G(A)
\arrow["H(\nu_A)", from=1-1, to=1-2]
\arrow["\sigma_{F(A)}", from=1-1, to=2-1]
\arrow["K(\nu_A)", from=2-1, to=2-2]
\arrow["\sigma_{G(A)}", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes.

**Proof.** For clarity, define $X=F(A)$ and $Y=G(A)$. Since $\sigma$ is a natural transformation and $\nu_{A}:X\to Y$ is a morphism in $\mathsf{D}$, the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
H(X) & H(Y) \\
K(X) & K(Y)
\arrow["H(\nu_A)", from=1-1, to=1-2]
\arrow["\sigma_X", from=1-1, to=2-1]
\arrow["K(\nu_A)", from=2-1, to=2-2]
\arrow["\sigma_Y", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. Substituting $X=F(A)$ and $Y=G(A)$ gives the diagram posed in the theorem, so it commutes. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Composition of Functors]]
- [[Natural Transformation]]