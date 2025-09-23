**Theorem.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories. Let $F,G:\mathsf{C}\to \mathsf{D}$ and $H,K:\mathsf{D}\to \mathsf{E}$. Let $\nu:F\Rightarrow G$ and $\sigma:H\Rightarrow K$. Then, the map $\eta$ that assigns to each object $a$ in $\mathsf{C}$ the morphism $$\eta_{a}=K(\nu_{a})\circ \sigma_{F(a)}$$in $\mathsf{E}$ is a natural transformation from $H\circ F$ to $K\circ G$.

**Proof.** Suppose $f:a\to b$ is a morphism in $\mathsf{C}$. Consider the following diagram (hereafter denoted as (1)).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
H\circ F(a) \arrow["H(F(f))", r] \arrow["\eta_a", d] & H\circ F(b) \arrow["\eta_b", d] \\
K\circ G(a) \arrow["K(G(f))", r] & K\circ G(b)
\end{tikzcd}
\end{document}
```

By definition of $\eta$, we can extend the diagram into the following diagram (hereafter denoted as (2)).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
H\circ F(a) \arrow["H(F(f))", r] \arrow["\sigma_{F(a)}", d] \arrow["\eta_a" description, dd, bend right=70, dashed, swap] & H\circ F(b) \arrow["\sigma_{F(b)}", d] \arrow["\eta_b" description, dd, bend left=70, dashed] \\
K\circ F(a) \arrow["K(F(f))", r] \arrow["K(\nu_a)", d] & K\circ F(b) \arrow["K(\nu_b)", d] \\
K\circ G(a) \arrow["K(G(f))", r] & K\circ G(b)
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