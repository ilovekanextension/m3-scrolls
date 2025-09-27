**Theorem.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Let $F,G:\mathsf{C}\to \mathsf{D}$. Let $\nu:F\Rightarrow G$. Then, the following statements are equivalent.
1. $\nu$ is an isomorphism in $\mathsf{D}^\mathsf{C}$.
2. For all objects $A$ in $\mathsf{C}$, the morphism $\nu_{A}:F(A)\to G(A)$ is an isomorphism in $\mathsf{D}$.

**Proof of** $1\Rightarrow 2$. Suppose $\nu$ is an isomorphism in $\mathsf{D}^\mathsf{C}$. Suppose $A$ is an object in $\mathsf{C}$. Since $\nu$ is an isomorphism, there is a natural transformation $\nu^{-1}:G\Rightarrow F$ such that $\nu^{-1}\circ \nu=\text{id}_{F}$ and $\nu\circ \nu^{-1}=\text{id}_{G}$. We then have $$(\nu^{-1})_{A}\circ \nu_{A}=(\nu^{-1}\circ \nu)_{A}=(\text{id}_{F})_{A}=\text{id}_{F(A)}$$and $$\nu_{A}\circ (\nu^{-1})_{A}=(\nu\circ \nu^{-1})_{A}=(\text{id}_{G})_{A}=\text{id}_{G(A)},$$so $\nu_{A}$ is an isomorphism with inverse $(\nu^{-1})_{A}$.

**Proof of** $2\Rightarrow 1$. Suppose for all objects $A$ in $\mathsf{C}$, the morphism $\nu_{A}:F(A)\to G(A)$ is an isomorphism. Define $\sigma$ as the transformation from $G$ to $F$ with components $\sigma_{A}=(\nu_{A})^{-1}$.

We first show that $\sigma$ is a natural transformation. Since $\nu$ is a natural transformation, the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
F(A) & F(B) \\
G(A) & G(B)
\arrow["F(f)", from=1-1, to=1-2]
\arrow["\sigma_A", from=1-1, to=2-1]
\arrow["G(f)", from=2-1, to=2-2]
\arrow["\sigma_B", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes, so by [[Square Diagrams with Inverse Morphisms as Commutative Squares]] the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
G(A) & G(B) \\
F(A) & F(B)
\arrow["G(f)", from=1-1, to=1-2]
\arrow["\nu_A", from=1-1, to=2-1]
\arrow["F(f)", from=2-1, to=2-2]
\arrow["\nu_B", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. This means $\sigma$ is natural.

We now show that $\sigma$ is the inverse of $\nu$. For all objects $a$ in $\mathsf{C}$ we have $$(\sigma\circ \nu)_{A}=\sigma_{a}\circ \nu_{A}=(\nu_{A})^{-1}\circ \nu_{A}=\text{id}_{F(A)}=(\text{id}_{F})_{A}$$and $$(\nu\circ \sigma)_{A}=\nu_{A}\circ \sigma_{A}=\nu_{A}\circ(\nu_{A})^{-1}=\text{id}_{G(A)}=(\text{id}_{G})_{A}.$$This shows that $\sigma\circ \nu=\text{id}_{F}$ and $\nu\circ \sigma=\text{id}_{G}$, so $\nu$ is an isomorphism with inverse $\sigma$. $\blacksquare$
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