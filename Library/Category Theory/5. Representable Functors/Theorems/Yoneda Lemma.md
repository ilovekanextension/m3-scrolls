**Theorem.** Let $\mathsf{C}$ be a locally small category. Then, for all functors $F:\mathsf{C}\to \mathsf{Set}$ and objects $x$ in $\mathsf{C}$, $$\mathsf{Set}^\mathsf{C}(h^x,F)\cong F(x)$$naturally in $x$ and $F$. Likewise, for all functors $F:\mathsf{C}^\text{op}\to \mathsf{Set}$ and objects $x$ in $\mathsf{C}$, $$\mathsf{Set}^{\mathsf{C}^\text{op}}(h_{x},F)\cong F(x)$$naturally in $x$ and $F$.

**Proof of First Statement.** Suppose $F:\mathsf{C}\to \mathsf{Set}$. Suppose $x$ is an object in $\mathsf{C}$. Define $\Phi:\mathsf{Set}^\mathsf{C}(h^x,F)\Rightarrow F(x)$ as $$\Phi(\alpha)=\alpha_{x}(\text{id}_{x}).$$Define $\Gamma:F(x)\to \mathsf{Set}^\mathsf{C}(h^x,F)$ as $$\Gamma(c)_{y}(f)=F(f)(c).$$Clearly $\Phi$ is well-defined. We will show that $\Gamma$ is also well-defined: that is, for all $c\in F(x)$, $\Gamma(c)$ is indeed a natural transformation from $h^x$ to $F$.

Suppose $c\in F(x)$. Suppose $f:y\to z$ is a morphism in $\mathsf{C}$. Consider the following diagram (1).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
h^x(y)=\mathsf{C}(x,y) & h^x(z)=\mathsf{C}(x,z) \\
F(y) & F(z)
\arrow["f\circ -", from=1-1, to=1-2]
\arrow["\Gamma(c)_y", from=1-1, to=2-1]
\arrow["F(f)", from=2-1, to=2-2]
\arrow["\Gamma(c)_z", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

For all $s:x\to y$, mapping $s$ along the functions on (1) gives us the following diagram.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
s & f\circ s \\
F(s)(c) & F(f)(F(s)(c))=F(f\circ s)(c)
\arrow["f\circ -", from=1-1, to=1-2, mapsto]
\arrow["\Gamma(c)_y", from=1-1, to=2-1, mapsto]
\arrow["F(f)", from=2-1, to=2-2, mapsto]
\arrow["\Gamma(c)_z", from=1-2, to=2-2, mapsto]
\end{tikzcd}
\end{document}
```

Therefore, by [[Extensionality of Functions]] (1) commutes.

We will now show that $\Phi$ is an isomorphism with inverse $\Gamma$. First suppose $c\in F(x)$. We have $$\Phi(\Gamma(c))=\Gamma(c)_{x}(\text{id}_{x})=F(\text{id}_{x})(c)=\text{id}_{F(x)}(c)=c.$$Next, suppose $\alpha:h^x\Rightarrow F$. Suppose $f:x\to y$ is a morphism in $\mathsf{C}$. Then, the diagram (2)

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
h^x(x)=\mathsf{C}(x,x) & h^x(y)=\mathsf{C}(x,y) \\
F(x) & F(y)
\arrow["f\circ -", from=1-1, to=1-2]
\arrow["\alpha_x", from=1-1, to=2-1]
\arrow["F(f)", from=2-1, to=2-2]
\arrow["\alpha_y", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

commutes, so mapping $\text{id}_{x}:x\to x$ along the functions on (2) gives us the following commutative diagram.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\text{id}_x & f\circ \text{id}_x=f \\
\alpha_x(\text{id}_x) & F(f)(\alpha_x(\text{id}_x))=\alpha_y(f)
\arrow["f\circ -", from=1-1, to=1-2, mapsto]
\arrow["\alpha_x", from=1-1, to=2-1, mapsto]
\arrow["F(f)", from=2-1, to=2-2, mapsto]
\arrow["\alpha_y", from=1-2, to=2-2, mapsto]
\end{tikzcd}
\end{document}
```

Since $\alpha_{x}(\text{id}_{x})=\Phi(\alpha)$, we have $$F(f)(\alpha_{x}(\text{id}_{x}))=F(f)(\Phi(\alpha))=\Gamma(\Phi(\alpha))_{y}(f)=\alpha_{y}(f).$$Therefore, by [[Extensionality of Functions]] $\Gamma(\Phi(\alpha))_{y}=\alpha_{y}$, so $\Gamma(\Phi(\alpha))=\alpha$.

We now show that $\Phi$ is natural in $x$ and $F$. For naturality in $x$, consider a morphism $f:x\to y$ and a functor $F:\mathsf{C\to \mathsf{Set}}$. We have to show that the following diagram (3) commutes.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{Set}^\mathsf{C}(h^x,F) & \mathsf{Set}^\mathsf{C}(h^y,F) \\
F(x) & F(y)
\arrow["-\circ h^f", from=1-1, to=1-2]
\arrow["\Phi_x", from=1-1, to=2-1]
\arrow["F(f)", from=2-1, to=2-2]
\arrow["\Phi_y", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

For all $\alpha:h^x\Rightarrow F$, mapping $\alpha$ along the functions in (3) gives the following diagram.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\alpha & \alpha\circ h^f \\
\alpha_x(\text{id}_x) & F(f)(\alpha_x(\text{id}_x))=^?(\alpha\circ h^f)_y(\text{id}_y)
\arrow["-\circ h^f", from=1-1, to=1-2, mapsto]
\arrow["\Phi_x", from=1-1, to=2-1, mapsto]
\arrow["F(f)", from=2-1, to=2-2, mapsto]
\arrow["\Phi_y", from=1-2, to=2-2, mapsto]
\end{tikzcd}
\end{document}
```

By commutativity of (2), $$(\alpha\circ h^f)_{y}(\text{id}_{y})=\alpha_{y}\circ(h^f)_{y}(\text{id}_{y})=\alpha_{y}(\text{id}_{y}\circ f)=\alpha_{y}(f)=F(f)(\alpha_{x}(\text{id}_{x})),$$so by [[Extensionality of Functions]] (3) commutes.

For naturality in $F$, consider an object $x$ in $\mathsf{C}$ and a natural transformation $\alpha:F\Rightarrow G$, where $F,G:\mathsf{C}\to \mathsf{Set}$. We have to show that the following diagram (4) commutes.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{Set}^\mathsf{C}(h^x,F) & \mathsf{Set}^\mathsf{C}(h^x,G) \\
F(x) & G(x)
\arrow["\alpha\circ -", from=1-1, to=1-2]
\arrow["\Phi_F", from=1-1, to=2-1]
\arrow["\alpha_x", from=2-1, to=2-2]
\arrow["\Phi_G", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

For all $\beta:h^x\Rightarrow F$, mapping $\eta$ along the functions in (4) gives us the following diagram.

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\beta & \alpha\circ\beta \\
\beta_x(\text{id}_x) & \alpha_x(\beta_x(\text{id}_x))=(\alpha\circ\beta)_x(\text{id}_x)
\arrow["\alpha\circ -", from=1-1, to=1-2, mapsto]
\arrow["\Phi_F", from=1-1, to=2-1, mapsto]
\arrow["\alpha_x", from=2-1, to=2-2, mapsto]
\arrow["\Phi_G", from=1-2, to=2-2, mapsto]
\end{tikzcd}
\end{document}
```

Therefore, (4) commutes. $\blacksquare$

**Proof of Second Statement.** This follows by applying [[Principle of Duality]] on the first statement. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Locally Small Category]]
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
- [[Principle of Duality]]
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]
- [[Bijective Functions as Isomorphisms]]