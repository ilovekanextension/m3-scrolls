**Definition.** Let $\mathsf{C}$ and $\mathsf{D}$ be categories. Two functors $F:\mathsf{C}\to \mathsf{D}$ and $G:\mathsf{D}\to \mathsf{C}$, together with an isomorphism $$\mathsf{D}(F(C),D)\cong\mathsf{C}(C,G(D))$$for each object $C$ in $\mathsf{C}$ and $D$ in $\mathsf{D}$ that is natural in both variables, is said to form an **adjunction**. In this case, we say that $F$ is **left adjoint** to $G$ (or that $G$ is **right adjoint** to $F$) and write $$F\dashv G.$$In diagrams, we may draw $F$ and $G$ as 

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{C} & \mathsf{D}
\arrow["F"{name=F}, from=1-1, to=1-2, bend left=25]
\arrow["G"{name=G}, from=1-2, to=1-1, bend left=25]
\arrow["\perp", phantom, from=F, to=G]
\end{tikzcd}
\end{document}
```

For all objects $C$ in $\mathsf{C}$ and $D$ in $\mathsf{D}$, given a morphism $f:F(C)\to D$, the image of $f$ under the isomorphism defined above will be denoted as $\bar{f}:C\to G(D)$. For clarity, the image of a morphism $g:C\to G(D)$ under the isomorphism defined above will also be denoted as $\bar{g}:F(C)\to D$. Morphisms $f$ and $\bar{f}$ are said to be **adjuncts** or **transposes** of each other.
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Functor]]
- [[Natural Isomorphism]]