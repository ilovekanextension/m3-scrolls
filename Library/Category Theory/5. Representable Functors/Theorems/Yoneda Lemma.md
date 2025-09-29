**Theorem.** Let $\mathsf{C}$ be a locally small category. Let $X$ be an object in $\mathsf{C}$.
1. Suppose $F:\mathsf{C}\to \mathsf{Set}$. Then, $$\mathsf{Set}^\mathsf{C}(h^X,F)\cong F(X)$$naturally in $X$ and $F$.
2. Suppose $F:\mathsf{C}^\text{op}\to \mathsf{Set}$. Then, $$\mathsf{Set}^{\mathsf{C}^\text{op}}(h_{X},F)\cong F(X)$$naturally in $X$ and $F$.

**Proof of First Statement.** Define functions $\phi:\mathsf{Set}^\mathsf{C}(h^X,F)\to F(X)$ and $\gamma:F(X)\to \mathsf{Set}^\mathsf{C}(h^X,F)$ as $$\phi(\alpha)=\alpha_{X}(\text{id}_{X})\wedge \gamma(c)=\{f_{X\to A}\mapsto [F(f)](c)\}_{A\in \text{Ob}(\mathsf{C})}$$respectively. We first show that $\gamma$ is well-defined (that is, for all $c\in F(X)$, $\gamma(c)$ is indeed a natural transformation from $h^X$ to $F$).

Suppose $c\in F(X)$. Suppose $g:A\to B$ is a morphism in $\mathsf{C}$. By definition, $h^X(A)=\mathsf{C}(X,A)$ and $h^X(B)=\mathsf{C}(X,B)$. Checking naturality therefore amounts to checking commutativity of the following diagram (1).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{C}(X,A) & \mathsf{C}(X,B) \\
F(A) & F(B)
\arrow["g\circ -", from=1-1, to=1-2]
\arrow["\gamma(c)_A", from=1-1, to=2-1, swap]
\arrow["F(g)", from=2-1, to=2-2]
\arrow["\gamma(c)_B", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

By [[Evaluations of Composite Functions]], for all morphisms $f:X\to A$ mapping $f$ along the lower functions of (1) gives $$[F(g)\circ \gamma(c)_{A}](f)=[F(g)]([F(f)](c))=[F(g)\circ F(f)](c)$$whereas mapping $f$ along the upper functions of (1) gives $$[\gamma(c)_{B}\circ(g\circ-)](f)=[\gamma(c)_{B}](g\circ f)=[F(g\circ f)](c).$$Since $F$ is a functor, $F(g\circ f)=F(g)\circ F(f)$, so the two expressions are the same. Therefore, by [[Extensionality of Functions]] (1) commutes. This shows that $\gamma(c)$ is a natural transformation.

Next we show that $\phi$ and $\gamma$ are inverses. First we show that for all $c\in F(X)$ we have $\phi(\gamma(c))=c$. To do this, suppose $c\in F(X)$. By definition, $$\phi(\gamma(c))=\gamma(c)_{X}(\text{id}_{X})=[F(\text{id}_{X})](c).$$Since $F$ is a functor, $F(\text{id}_{X})=\text{id}_{F(X)}$, so $F(\text{id}_{X})$ is the identity function of $F(X)$. Therefore, $[F(\text{id}_{X})](c)=c$, so $\phi(\gamma(c))=c$. Next we show that $\gamma(\phi(\alpha))=\alpha$ for all $\alpha:h^X\Rightarrow F$. To do this, we need to show that $[\gamma(\phi(\alpha))]_{A}=\alpha_{A}$ for all objects $A$ in $\mathsf{C}$. Since both are functions, by [[Extensionality of Functions]] it is enough to show that $$[\gamma(\phi(\alpha))]_{A}(f)=\alpha_{A}(f)$$for all morphisms $f:X\to A$ in $\mathsf{C}$.

Suppose $\alpha:h^X\Rightarrow F$. Suppose $A$ is an object in $\mathsf{C}$. Suppose $f:X\to A$ is a morphism in $\mathsf{C}$. Since $\alpha$ is a natural transformation, the diagram (2)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{C}(X,X) & \mathsf{C}(X,A) \\
F(X) & F(A)
\arrow["f\circ -", from=1-1, to=1-2]
\arrow["\alpha_X", from=1-1, to=2-1, swap]
\arrow["F(f)", from=2-1, to=2-2]
\arrow["\alpha_A", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. This means $F(f)\circ \alpha_{X}=\alpha_{A}\circ(f\circ-)$. This is an equality of functions, so by [[Extensionality of Functions]] for all morphisms $g:X\to X$ we have $[F(f)\circ \alpha_{X}](g)=[\alpha_{A}\circ(f\circ-)](g)$. In particular, since $\text{id}_{X}:X\to X$, $$[F(f)\circ \alpha_{X}](\text{id}_{X})=[\alpha_{A}\circ(f\circ-)](\text{id}_{X}).$$By [[Evaluations of Composite Functions]], the left side of this equality evaluates to $$[F(f)](\alpha_{X}(\text{id}_{X}))=[F(f)](\phi(\alpha))=[\gamma(\phi(\alpha))]_{A}(f)$$whereas the right side evaluates to $\alpha_{A}(f\circ \text{id}_{X})=\alpha_{A}(f)$. Therefore, $[\gamma(\phi(\alpha))]_{A}(f)=\alpha_{A}(f)$. This is precisely what we wanted to show.

Finally we show that $\phi$ is natural in $X$ and $F$. To show that $\phi$ is natural in $X$, suppose $f:X\to A$ is a morphism in $\mathsf{C}$. Define a function $\phi_{A}:\mathsf{Set}^\mathsf{C}(h^A,F)\to F(A)$ similarly to $\phi$ as $$\phi_{A}(\alpha)=\alpha_{A}(\text{id}_{A}).$$We need to show that the diagram (3) 

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{Set}^{\mathsf{C}}(h^X,F) & \mathsf{Set}^{\mathsf{C}}(h^A,F) \\
F(X) & F(A)
\arrow["-\circ h^f", from=1-1, to=1-2]
\arrow["\phi", from=1-1, to=2-1, swap]
\arrow["F(f)", from=2-1, to=2-2]
\arrow["\phi_A", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. By [[Evaluations of Composite Functions]], for all natural transformations $\alpha:h^X\Rightarrow F$ mapping $\alpha$ along the lower functions of (3) gives $$[F(f)\circ\phi](\alpha)=[F(f)](\phi(\alpha))=[\gamma(\phi(\alpha))]_{A}(f)$$whereas mapping $\alpha$ along the upper functions of (3) gives $$[\phi_{A}\circ(-\circ h^f)](\alpha)=\phi_{A}(\alpha\circ h^f)=(\alpha\circ h^f)_{A}(\text{id}_{A})=[\alpha_{A}\circ h^f_{A}](\text{id}_{A})=\alpha_{A}(\text{id}_{A}\circ f)=\alpha_{A}(f).$$This is precisely the commutativity of (2), so (3) commutes. To show that $\phi$ is natural in $F$, suppose $\nu:F\Rightarrow G$. Define a function $\phi_{G}:\mathsf{Set}^\mathsf{C}(h^X,G)\to G(X)$ similarly to $\phi$ as $$\phi_{G}(\alpha)=\alpha_{X}(\text{id}_{X}).$$We need to show that the diagram (4)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{Set}^{\mathsf{C}}(h^X,F) & \mathsf{Set}^{\mathsf{C}}(h^X,G) \\
F(X) & G(X)
\arrow["\nu\circ -", from=1-1, to=1-2]
\arrow["\phi", from=1-1, to=2-1, swap]
\arrow["\nu_X", from=2-1, to=2-2]
\arrow["\phi_G", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. By [[Evaluations of Composite Functions]], for all natural transformations $\alpha:h^X\Rightarrow F$ mapping $\alpha$ along the lower functions of (4) gives $$[\nu_{X}\circ\phi](\alpha)=\nu_{X}(\alpha_{X}(\text{id}_{X}))=[\nu_{X}\circ\alpha_{X}](\text{id}_{X})$$whereas mapping $\alpha$ along the upper functions of (4) gives $$[\phi_{G}\circ(\nu \circ-)](\alpha)=\phi_{G}(\nu\circ\alpha)=[(\nu\circ\alpha)_{X}](\text{id}_{X}).$$By definition of vertical composition, $(\nu\circ\alpha)_{X}=\nu_{X}\circ\alpha_{X}$, so the two expressions are the same. Therefore, by [[Extensionality of Functions]] (4) commutes. $\blacksquare$

**Proof of Second Statement.** Define functions $\phi:\mathsf{Set}^\mathsf{C^\text{op}}(h_{X},F)\to F(X)$ and $\gamma:F(X)\to \mathsf{Set}^\mathsf{C^\text{op}}(h_{X},F)$ as $$\phi(\alpha)=\alpha_{X}(\text{id}_{X})\wedge \gamma(c)=\{f_{A\to X}\mapsto [F(f)](c)\}_{A\in \text{Ob}(\mathsf{C})}$$respectively. We first show that $\gamma$ is well-defined (that is, for all $c\in F(X)$, $\gamma(c)$ is indeed a natural transformation from $h_{X}$ to $F$).

Suppose $c\in F(X)$. Suppose $g:A\to B$ is a morphism in $\mathsf{C}$. By definition, $h_{X}(A)=\mathsf{C}(A,X)$ and $h_{X}(B)=\mathsf{C}(B,X)$. Checking naturality therefore amounts to checking commutativity of the following diagram (1).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{C}(B,X) & \mathsf{C}(A,X) \\
F(B) & F(A)
\arrow["-\circ g", from=1-1, to=1-2]
\arrow["\gamma(c)_B", from=1-1, to=2-1, swap]
\arrow["F(g)", from=2-1, to=2-2]
\arrow["\gamma(c)_A", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

By [[Evaluations of Composite Functions]], for all morphisms $f:B\to X$ mapping $f$ along the lower functions of (1) gives $$[F(g)\circ \gamma(c)_{B}](f)=[F(g)]([F(f)](c))=[F(g)\circ F(f)](c)$$whereas mapping $f$ along the upper functions of (1) gives $$[\gamma(c)_{A}\circ(-\circ g)](f)=[\gamma(c)_{A}](f\circ g)=[F(f\circ g)](c).$$Since $F$ is a functor, $F(f\circ g)=F(g)\circ F(f)$, so the two expressions are the same. Therefore, by [[Extensionality of Functions]] (1) commutes. This shows that $\gamma(c)$ is a natural transformation.

Next we show that $\phi$ and $\gamma$ are inverses. First we show that for all $c\in F(X)$ we have $\phi(\gamma(c))=c$. To do this, suppose $c\in F(X)$. By definition, $$\phi(\gamma(c))=\gamma(c)_{X}(\text{id}_{X})=[F(\text{id}_{X})](c).$$Since $F$ is a functor, $F(\text{id}_{X})=\text{id}_{F(X)}$, so $F(\text{id}_{X})$ is the identity function of $F(X)$. Therefore, $[F(\text{id}_{X})](c)=c$, so $\phi(\gamma(c))=c$. Next we show that $\gamma(\phi(\alpha))=\alpha$ for all $\alpha:h_{X}\Rightarrow F$. To do this, we need to show that $[\gamma(\phi(\alpha))]_{A}=\alpha_{A}$ for all objects $A$ in $\mathsf{C}$. Since both are functions, by [[Extensionality of Functions]] it is enough to show that $$[\gamma(\phi(\alpha))]_{A}(f)=\alpha_{A}(f)$$for all morphisms $f:A\to X$ in $\mathsf{C}$.

Suppose $\alpha:h_{X}\Rightarrow F$. Suppose $A$ is an object in $\mathsf{C}$. Suppose $f:A\to X$ is a morphism in $\mathsf{C}$. Since $\alpha$ is a natural transformation, the diagram (2)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{C}(X,X) & \mathsf{C}(A,X) \\
F(X) & F(A)
\arrow["-\circ f", from=1-1, to=1-2]
\arrow["\alpha_X", from=1-1, to=2-1, swap]
\arrow["F(f)", from=2-1, to=2-2]
\arrow["\alpha_A", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. This means $F(f)\circ \alpha_{X}=\alpha_{A}\circ(-\circ f)$. This is an equality of functions, so by [[Extensionality of Functions]] for all morphisms $g:X\to X$ we have $[F(f)\circ \alpha_{X}](g)=[\alpha_{A}\circ(-\circ f)](g)$. In particular, since $\text{id}_{X}:X\to X$, $$[F(f)\circ \alpha_{X}](\text{id}_{X})=[\alpha_{A}\circ(-\circ f)](\text{id}_{X}).$$By [[Evaluations of Composite Functions]], the left side of this equality evaluates to $$[F(f)](\alpha_{X}(\text{id}_{X}))=[F(f)](\phi(\alpha))=[\gamma(\phi(\alpha))]_{A}(f)$$whereas the right side evaluates to $\alpha_{A}(\text{id}_{X}\circ f)=\alpha_{A}(f)$. Therefore, $[\gamma(\phi(\alpha))]_{A}(f)=\alpha_{A}(f)$. This is precisely what we wanted to show.

Finally we show that $\phi$ is natural in $X$ and $F$. To show that $\phi$ is natural in $X$, suppose $f:A\to X$ is a morphism in $\mathsf{C}$. Define a function $\phi_{A}:\mathsf{Set}^\mathsf{C}(h_{A},F)\to F(A)$ similarly to $\phi$ as $$\phi_{A}(\alpha)=\alpha_{A}(\text{id}_{A}).$$We need to show that the diagram (3) 

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{Set}^{\mathsf{C^\text{op}}}(h_X,F) & \mathsf{Set}^{\mathsf{C^\text{op}}}(h_A,F) \\
F(X) & F(A)
\arrow["-\circ h_f", from=1-1, to=1-2]
\arrow["\phi", from=1-1, to=2-1, swap]
\arrow["F(f)", from=2-1, to=2-2]
\arrow["\phi_A", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. By [[Evaluations of Composite Functions]], for all natural transformations $\alpha:h_{X}\Rightarrow F$ mapping $\alpha$ along the lower functions of (3) gives $$[F(f)\circ\phi](\alpha)=[F(f)](\phi(\alpha))=[\gamma(\phi(\alpha))]_{A}(f)$$whereas mapping $\alpha$ along the upper functions of (3) gives $$[\phi_{A}\circ(-\circ h_{f})](\alpha)=\phi_{A}(\alpha\circ h_{f})=(\alpha\circ h_{f})_{A}(\text{id}_{A})=[\alpha_{A}\circ (h_{f})_{A}](\text{id}_{A})=\alpha_{A}(f\circ \text{id}_{A})=\alpha_{A}(f).$$This is precisely the commutativity of (2), so (3) commutes. To show that $\phi$ is natural in $F$, suppose $\nu:F\Rightarrow G$. Define a function $\phi_{G}:\mathsf{Set}^\mathsf{C}(h_{X},G)\to G(X)$ similarly to $\phi$ as $$\phi_{G}(\alpha)=\alpha_{X}(\text{id}_{X}).$$We need to show that the diagram (4)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{Set}^{\mathsf{C^\text{op}}}(h_X,F) & \mathsf{Set}^{\mathsf{C^\text{op}}}(h_X,G) \\
F(X) & G(X)
\arrow["\nu\circ -", from=1-1, to=1-2]
\arrow["\phi", from=1-1, to=2-1, swap]
\arrow["\nu_X", from=2-1, to=2-2]
\arrow["\phi_G", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes. By [[Evaluations of Composite Functions]], for all natural transformations $\alpha:h_{X}\Rightarrow F$ mapping $\alpha$ along the lower functions of (4) gives $$[\nu_{X}\circ\phi](\alpha)=\nu_{X}(\alpha_{X}(\text{id}_{X}))=[\nu_{X}\circ\alpha_{X}](\text{id}_{X})$$whereas mapping $\alpha$ along the upper functions of (4) gives $$[\phi_{G}\circ(\nu \circ-)](\alpha)=\phi_{G}(\nu\circ\alpha)=[(\nu\circ\alpha)_{X}](\text{id}_{X}).$$By definition of vertical composition, $(\nu\circ\alpha)_{X}=\nu_{X}\circ\alpha_{X}$, so the two expressions are the same. Therefore, by [[Extensionality of Functions]] (4) commutes. $\blacksquare$

***
Definitions used:
- [[Category]]
- [[Locally Small Category]]
- [[Opposite Category]]
- [[Functor]]
- [[Natural Transformation]]
- [[Vertical Composition of Natural Transformations]]
- [[Hom-Functor]]
- [[Natural Transformation Between Hom-Functors]]
- [[Function]]
- [[Composition of Functions]]
- [[Bijective Function]]
- [[Category of Sets]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]
- [[Bijective Functions as Isomorphisms]]