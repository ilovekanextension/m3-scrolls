Let $\mathsf{I}$ and $\mathsf{C}$ be categories, and suppose that $\mathsf{I}$ is small. Let $F:\mathsf{I}\to \mathsf{C}$. A **limit cone** of $F$ is a cone $(L,\nu)$ in $\text{Cone}(L,F)$ such that for all objects $A$ in $\mathsf{C}$ and cones $(A,\sigma)$ in $\text{Cone}(A,F)$ there is a unique morphism $f:A\to L$ making the diagram

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

commute for all objects $X$ in $\mathsf{I}$. A **colimit cocone** of $F$ is a cocone $(C,\nu)$ in $\text{Cone}(F,L)$ such that for all objects $A$ in $\mathsf{C}$ and cocones $(A,\sigma)$ in $\text{Cone}(F,A)$ there is a unique morphism $f:C\to A$ making the diagram

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

commute for all objects $X$ in $\mathsf{I}$.

**Theorem.** Let $\mathsf{I}$ and $\mathsf{C}$ be categories, and suppose that $\mathsf{I}$ is small. Let $F:\mathsf{I}\to \mathsf{C}$. Suppose $(L,\nu)$ and $(K,\sigma)$ are limit cones of $F$. Then, there is a unique isomorphism $i:L\to K$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
L & \\
K & F(X)
\arrow["i", from=1-1, to=2-1, swap]
\arrow["\sigma_X", from=2-1, to=2-2, swap]
\arrow["\nu_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commutes for all objects $X$ in $\mathsf{I}$. Likewise, suppose $(C,\nu)$ and $(D,\sigma)$ are colimit cocones of $F$. Then there is a unique isomorphism $i:C\to D$ such that the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
C & \\
D & F(X)
\arrow["i", from=1-1, to=2-1, swap]
\arrow["\sigma_X", from=2-1, to=2-2, swap]
\arrow["\nu_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commutes for all objects $X$ in $\mathsf{I}$.

**Proof of First Statement.** For brevity, fix an object $X$ in $\mathsf{I}$. Since $(K,\sigma)$ is a limit and $(L,\nu)$ is a cone, there is a morphism $f:L\to K$ such that the diagram (1)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
L & \\
K & F(X)
\arrow["f", from=1-1, to=2-1, swap]
\arrow["\sigma_X", from=2-1, to=2-2, swap]
\arrow["\nu_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. Likewise, since $(L,\nu)$ is a limit and $(K,\sigma)$ is a cone, there is a morphism $g:K\to L$ such that the diagram (2)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
K & \\
L & F(X)
\arrow["g", from=1-1, to=2-1, swap]
\arrow["\nu_X", from=2-1, to=2-2, swap]
\arrow["\sigma_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. We will show that $f$ is an isomorphism with inverse $g$.

By commutativity of (1), we have $\nu_{X}=\sigma_{X}\circ f$. By commutativity of (2), we have $\sigma_{X}=\nu_{X}\circ g$. Substituting the latter equality into the former gives $\nu_{X}=\nu_{X}\circ(g\circ f)$. Therefore, the diagram (3)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
L & \\
L & F(X)
\arrow["g\circ f", from=1-1, to=2-1, swap]
\arrow["\nu_X", from=2-1, to=2-2, swap]
\arrow["\nu_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. Now notice that the diagram (4)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
L & \\
L & F(X)
\arrow["\text{id}_L", from=1-1, to=2-1, swap]
\arrow["\nu_X", from=2-1, to=2-2, swap]
\arrow["\nu_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

also commutes. Since $(L,\nu)$ is a limit, the morphism $L\to L$ making the diagram commute must be unique. Therefore, by commutativity of (3) and (4), we can conclude that $g\circ f=\text{id}_{L}$. By a similar reasoning, we can also conclude that $f\circ g=\text{id}_{K}$. This shows that $f$ is an isomorphism with inverse $g$.

Now suppose $h:L\to K$ is another isomorphism making the diagram commute. Since $(K,\sigma)$ is a limit, the morphism $L\to K$ making the diagram commute must be unique. The morphisms $f$ and $h$ satisfy the property, so we must have $f=h$. $\blacksquare$

**Proof of Second Statement.** For brevity, fix an object $X$ in $\mathsf{I}$. Since $(C,\nu)$ is a colimit and $(D,\sigma)$ is a cocone, there is a morphism $f:C\to D$ such that the diagram (1)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
C & \\
D & F(X)
\arrow["f", from=1-1, to=2-1, swap]
\arrow["\sigma_X", from=2-1, to=2-2, swap]
\arrow["\nu_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. Likewise, since $(D,\sigma)$ is a colimit and $(C,\nu)$ is a cocone, there is a morphism $g:D\to C$ such that the diagram (2)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
D & \\
C & F(X)
\arrow["g", from=1-1, to=2-1, swap]
\arrow["\nu_X", from=2-1, to=2-2, swap]
\arrow["\sigma_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. We will show that $f$ is an isomorphism with inverse $g$.

By commutativity of (1), we have $\nu_{X}=\sigma_{X}\circ f$. By commutativity of (2), we have $\sigma_{X}=\nu_{X}\circ g$. Substituting the latter equality into the former gives $\nu_{X}=\nu_{X}\circ(g\circ f)$. Therefore, the diagram (3)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
C & \\
C & F(X)
\arrow["g\circ f", from=1-1, to=2-1, swap]
\arrow["\nu_X", from=2-1, to=2-2, swap]
\arrow["\nu_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. Now notice that the diagram (4)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
C & \\
C & F(X)
\arrow["\text{id}_C", from=1-1, to=2-1, swap]
\arrow["\nu_X", from=2-1, to=2-2, swap]
\arrow["\nu_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

also commutes. Since $(C,\nu)$ is a colimit, the morphism $C\to C$ making the diagram commute must be unique. Therefore, by commutativity of (3) and (4), we can conclude that $g\circ f=\text{id}_{C}$. By a similar reasoning, we can also conclude that $f\circ g=\text{id}_{D}$. This shows that $f$ is an isomorphism with inverse $g$.

Now suppose $h:C\to D$ is another isomorphism making the diagram commute. Since $(C,\nu)$ is a colimit, the morphism $C\to D$ making the diagram commute must be unique. The morphisms $f$ and $h$ satisfy the property, so we must have $f=h$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Small Category]]
- [[Opposite Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Natural Transformation]]
- [[Cone and Cocone]]