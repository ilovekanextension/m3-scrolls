**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F,G:\mathsf{C}\to \mathsf{D}$. Let $\nu:F\Rightarrow G$. Then, the following statements are equivalent.
1. $\nu$ is an isomorphism in $\mathsf{D}^\mathsf{C}$.
2. For all objects $a$ in $\mathsf{C}$, the morphism $\nu_{a}:F(a)\to G(a)$ is an isomorphism in $\mathsf{D}$.

**Proof of** $1\Rightarrow 2$. Suppose $\nu$ is an isomorphism in $\mathsf{D}^\mathsf{C}$. Suppose $a$ is an object in $\mathsf{C}$. Since $\nu$ is an isomorphism, there is a natural transformation $\nu^{-1}:G\Rightarrow F$ such that $\nu^{-1}\circ \nu=\text{id}_{F}$ and $\nu\circ \nu^{-1}=\text{id}_{G}$. We then have $$(\nu^{-1})_{a}\circ \nu_{a}=(\nu^{-1}\circ \nu)_{a}=(\text{id}_{F})_{a}=\text{id}_{F(a)}$$and $$\nu_{a}\circ (\nu^{-1})_{a}=(\nu\circ \nu^{-1})_{a}=(\text{id}_{G})_{a}=\text{id}_{G(a)},$$so $\nu_{a}$ is an isomorphism with inverse $(\nu^{-1})_{a}$.

**Proof of** $2\Rightarrow 1$. Suppose for all objects $a$ in $\mathsf{C}$, the morphism $\nu_{a}:F(a)\to G(a)$ is an isomorphism. Define $\sigma$ as the map that assigns to each object $a$ in $\mathsf{C}$ the morphism $\sigma_{a}=(\nu_{a})^{-1}$.

We first show that $\sigma$ is a natural transformation. Suppose $f:a\to b$ is a morphism in $\mathsf{C}$. Consider the following diagram (hereafter denoted as (1)).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
G(a) \arrow["G(f)", r] \arrow["\sigma_a", d] & G(b) \arrow["\sigma_b", d] \\
F(a) \arrow["F(f)", r] & F(b)
\end{tikzcd}
\end{document}
```

Since $\nu$ is a natural transformation, the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(a) \arrow["F(f)", r] \arrow["\nu_a", d] & F(b) \arrow["\nu_b", d] \\
G(a) \arrow["G(f)", r] & G(b)
\end{tikzcd}
\end{document}
```

commutes, so by [[Square Diagrams with Inverse Morphisms as Commutative Squares]] (1) commutes.

We now show that $\sigma$ is the inverse of $\nu$. For all objects $a$ in $\mathsf{C}$ we have $$(\sigma\circ \nu)_{a}=\sigma_{a}\circ \nu_{a}=(\nu_{a})^{-1}\circ \nu_{a}=\text{id}_{F(a)}=(\text{id}_{F})_{a}$$and $$(\nu\circ \sigma)_{a}=\nu_{a}\circ \sigma_{a}=\nu_{a}\circ(\nu_{a})^{-1}=\text{id}_{G(a)}=(\text{id}_{G})_{a}.$$This shows that $\sigma\circ \nu=\text{id}_{F}$ and $\nu\circ \sigma=\text{id}_{G}$, so $\nu$ is an isomorphism with inverse $\sigma$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Natural Transformation]]
- [[Functor Category]]
- [[Identity Natural Transformation]]
- [[Vertical Composition of Natural Transformations]]

Theorems used:
- [[Square Diagrams with Inverse Morphisms as Commutative Squares]]