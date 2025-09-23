**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F,G,H:\mathsf{C}\to \mathsf{D}$. Let $\nu:F\Rightarrow G$ and $\sigma:G\Rightarrow H$. Then, the map $\alpha$ that assigns to each object $a$ in $\mathsf{C}$ the morphism $$\alpha_{a}=\sigma_{a}\circ \nu_{a}$$is a natural transformation from $F$ to $H$.

**Proof.** Suppose $f:a\to b$ is a morphism in $\mathsf{C}$. Consider the following diagram (hereafter denoted as (1)).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(a) \arrow["F(f)", r] \arrow["\alpha_a", d] & F(b) \arrow["\alpha_b", d] \\
H(a) \arrow["H(f)", r] & H(b)
\end{tikzcd}
\end{document}
```

By definition, $\alpha_{a}=\sigma_{a}\circ \nu_{a}$ and $\alpha_{b}=\sigma_{b}\circ \nu_{b}$. We can therefore extend (1) into the following diagram (hereafter denoted as (2)).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(a) \arrow["F(f)", r] \arrow["\nu_a", d] \arrow["\alpha_a" description, dd, bend right=50, dashed] & F(b) \arrow["\nu_b", d] \arrow["\alpha_b" description, dd, bend left=50, dashed] \\
G(a) \arrow["G(f)", r] \arrow["\sigma_a", d] & G(b) \arrow["\sigma_b", d] \\
H(a) \arrow["H(f)", r] & H(b)
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