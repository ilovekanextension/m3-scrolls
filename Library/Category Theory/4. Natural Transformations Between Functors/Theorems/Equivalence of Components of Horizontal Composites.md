**Theorem.** Let $\mathsf{C}$, $\mathsf{D}$, and $\mathsf{E}$ be categories. Let $F,G:\mathsf{C}\to \mathsf{D}$ and $H,K:\mathsf{D}\to \mathsf{E}$. Let $\nu:F\Rightarrow G$ and $\sigma:H\Rightarrow K$. Suppose $a$ is an object in $\mathsf{C}$. Then, the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
H\circ F(a) \arrow["H(\nu_a)", r] \arrow["\sigma_{F(a)}", d] & H\circ G(a) \arrow["\sigma_{G(a)}", d] \\
K\circ F(a) \arrow["K(\nu_a)", r] & K\circ G(a)
\end{tikzcd}
\end{document}
```

commutes.

**Proof.** Define $x=F(a)$ and $y=G(a)$. Since $\sigma$ is a natural transformation and $\nu_{a}:x\to y$ is a morphism in $\mathsf{D}$, the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
H(x) \arrow["H(\nu_a)", r] \arrow["\sigma_x", d] & H(y) \arrow["\sigma_y", d] \\
K(x) \arrow["K(\nu_a)", r] & K(y)
\end{tikzcd}
\end{document}
```

commutes. Substituting $x=F(a)$ and $y=G(a)$ gives the diagram posed in the theorem, so it commutes. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Composition of Functors]]
- [[Natural Transformation]]