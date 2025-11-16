**Theorem.** The category $\mathsf{Set}$ is complete.

**Proof.** Let $\mathsf{I}$ be a small category. Let $F:\mathsf{I}\to \mathsf{Set}$. Let $1=\{*\}$ be a singleton. We will first show that the pair $(\text{Cone}(1,F),\mu)$, where $\mu$ is the transformation from $\Delta_{\text{Cone}(1,F)}$ to $F$ defined as $$\mu_{X}(1,\nu)=\nu_{X}(*),$$is a cone over $F$. To do this, we will show that $\mu$ is natural.

Suppose $f:X\to Y$ is a morphism in $\mathsf{I}$. We want to show that the following diagram (1) commutes.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}[column sep=tiny]
 & \text{Cone}(1,F) & \\
F(X) & & F(Y)
\arrow["\mu_X", from=1-2, to=2-1, swap]
\arrow["F(f)", from=2-1, to=2-3, swap]
\arrow["\mu_Y", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

To do this, suppose $(1,\nu)\in \text{Cone}(1,F)$. Then, the diagram (2)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}[column sep=tiny]
 & 1 & \\
F(X) & & F(Y)
\arrow["\nu_X", from=1-2, to=2-1, swap]
\arrow["F(f)", from=2-1, to=2-3, swap]
\arrow["\nu_Y", from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```

commutes. Since $*\in 1$, by [[Extensionality of Functions]] and [[Evaluations of Composite Functions]] commutativity of (2) means $$[F(f)](\nu_{X}(*))=[F(f)\circ \nu_{X}](*)=\nu_{Y}(*).$$Therefore, $$[F(f)\circ\mu_{X}](1,\nu)=[F(f)](\nu_{X}(*))=\nu_{Y}(*)=\mu_{Y}(1,\nu),$$so (1) commutes.

We will now show that $(\text{Cone}(1,F),\mu)$ is the limit of $F$. Suppose $(A,\sigma)$ is a cone over $F$. We want to show that there is a unique function $A\to \text{Cone}(1,F)$ making the diagram

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
A & \\
\text{Cone}(1,F) & F(X)
\arrow[from=1-1, to=2-1]
\arrow["\mu_X", from=2-1, to=2-2, swap]
\arrow["\sigma_X", from=1-1, to=2-2]
\end{tikzcd}
\end{document}
```

commute for all objects $X$ in $\mathsf{I}$.

Observe that for all objects $a\in A$ there is a function $f_{a}:1\to A$ such that $f_{a}(*)=a$. By [[Change of Legs of Cones and Cocones by Compositions with Morphisms]], the transformation $\eta_{a}$ from $\Delta_{1}$ to $F$ defined as $$(\eta_{a})_{X}=\sigma_{X}\circ f_{a}$$is natural, so $(1,\eta_{a})\in \text{Cone}(1,F)$.
- **Existence.** Define a function $g:A\to \text{Cone}(1,F)$ as $$g(a)=(1,\eta_{a}).$$Suppose $X$ is an object in $\mathsf{I}$. We will show that $g$ makes the diagram commute. By [[Extensionality of Functions]], it is enough to show that $$[\mu_{X}\circ g](a)=\sigma_{X}(a)$$for all $a\in A$.
  
  Suppose $a\in A$. By [[Evaluations of Composite Functions]], $$[\mu_{X}\circ g](a)=\mu_{X}(g(a))=\mu_{X}(1,\eta_{a})=(\eta_{a})_{X}(*)=\sigma_{X}(f_{a}(*))=\sigma_{X}(a).$$
- **Uniqueness.** Suppose $h:A\to \text{Cone}(1,F)$ makes the diagram commute for all objects $X$ in $\mathsf{I}$. We want to show that $h=g$. To do this, by [[Extensionality of Functions]] it is enough to show that $h(a)=g(a)$ for all $a\in A$.
  
  Suppose $a\in A$. For clarity, suppose that $h(a)=(1,\nu)$ for some $\nu:\Delta_{1}\Rightarrow F$. Then, for all objects $X$ in $\mathsf{I}$, $$\mu_{X}(h(a))=\mu_{X}(1,\nu)=\nu_{X}(*).$$Now suppose $X$ is an object in $\mathsf{I}$. By assumption, $[\mu_{X}\circ h](a)=\sigma_{X}(a)$, so $\nu_{X}(*)=\sigma_{X}(a)$. Observe also that $$(\eta_{a})_{X}(*)=\sigma_{X}(f_{a}(*))=\sigma_{X}(a).$$By [[Extensionality of Functions]], for all objects $X$ in $\mathsf{I}$ we can conclude that $\nu_{X}=(\eta_{a})_{X}$, so $\nu=\eta_{a}$. This means $(1,\nu)=(1,\eta_{a})$, so $h(a)=g(a)$. $\blacksquare$

***
Definitions used:
- [[Category]]
- [[Small Category]]
- [[Categorical Diagram]]
- [[Natural Transformation]]
- [[Cone and Cocone]]
- [[Categorical Limit and Colimit]]
- [[Category of Sets]]

Theorems used:
- [[Change of Legs of Cones and Cocones by Compositions with Morphisms]]
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]