**Definition.** Let $\mathsf{I}$ and $\mathsf{C}$ be categories, and suppose that $\mathsf{I}$ is small. Let $F:\mathsf{I}\to \mathsf{C}$. A **limit** of $F$ is a representation of the cone functor $\text{Cone}(-,F):\mathsf{C}^\text{op}\to \mathsf{Set}$. A **colimit** of $F$ is a representation of the cocone functor $\text{Cone}(F,-):\mathsf{C}\to \mathsf{Set}$.

By definition of functor representations, there are then two equivalent ways to define a limit of $F$. First, a limit of $F$ consists of
- an object $L$ in $\mathsf{C}$ and
- a natural isomorphism $\nu:h^L\Rightarrow \text{Cone}(-,F)$.

Second, a limit of $F$ consists of
- an object $L$ in $\mathsf{C}$ and
- a cone $(L,\nu)$ in $\text{Cone}(L,F)$ called a **limit cone**

such that for all objects $A$ in $\mathsf{C}$ and cones $(A,\sigma)$ in $\text{Cone}(A,F)$ there is a unique morphism $f:A\to L$ making the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
A & \\
L & F(X)
\arrow["f", from=1-1, to=2-1, swap]
\arrow["\nu_X", from=2-1, to=2-2, swap]
\arrow["\sigma_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commute for all objects $X$ in $\mathsf{I}$. In both cases, we say that $L$ is the **limit object** of $F$. When $\nu$ is known from context, we can say that $L$ itself is a limit of $F$.

Likewise, there are two equivalent ways to define a colimit of $F$. First, a colimit of $F$ consists of
- an object $C$ in $\mathsf{C}$ and
- a natural isomorphism $\nu:h_{C}\Rightarrow \text{Cone}(F,-)$.

Second, a colimit of $F$ consists of
- an object $C$ in $\mathsf{C}$ and
- a cocone $(C,\nu)$ in $\text{Cone}(F,C)$ called a **colimit cocone**

such that for all objects $A$ in $\mathsf{C}$ and cocones $(A,\sigma)$ in $\text{Cone}(F,A)$ there is a unique morphism $f:C\to A$ making the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
C & \\
A & F(X)
\arrow["f", from=1-1, to=2-1, swap]
\arrow["\sigma_X", from=2-1, to=2-2, swap]
\arrow["\nu_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commute for all objects $X$ in $\mathsf{I}$. In both cases, we say that $C$ is the **colimit object** of $F$. When $\nu$ is known from context, we can say that $C$ itself is a colimit of $F$.

By [[Uniqueness of Categorical Limits and Colimits]], limits and colimits of $F$, when they exist, are unique up to isomorphism. Therefore, we can speak of **the** limit and **the** colimit of $F$. Generally, the limit and colimit of $F$ is denoted as $\lim(F)$ and $\text{colim}(F)$ respectively.
***
Definitions used;
- [[Category]]
- [[Small Category]]
- [[Opposite Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Covariant and Contravariant Functor]]
- [[Natural Transformation]]
- [[Natural Isomorphism]]
- [[Representable Functor]]
- [[Cone and Cocone]]
- [[Cone Functor and Cocone Functor]]