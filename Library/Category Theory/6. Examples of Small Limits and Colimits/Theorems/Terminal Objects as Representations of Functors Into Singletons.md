**Theorem.** Let $\mathsf{C}$ be a locally small category. Suppose $t$ is an object in $\mathsf{C}$. Then, $t$ is terminal if and only if $h_{t}:\mathsf{C}^\text{op}\to \mathsf{Set}$ is naturally isomorphic to the constant functor $\{*\}:\mathsf{C}^\text{op}\to \mathsf{Set}$.

**Proof of Forward Implication.** Suppose $t$ is terminal. By [[Singleton Sets as Terminal Objects]], for all objects $a$ in $\mathsf{C}$ we can define $\eta_{a}$ to be the unique function $\mathsf{C}(a,t)\to\{*\}$. By definition, we then have $\eta_{a}:h_{t}(a)\to\{*\}$. We will show that $\eta$ is a natural isomorphism $h_{t}\Rightarrow \{*\}$.

First we will show that $\eta$ is a natural transformation. Suppose $f:a\to b$ is a morphism in $\mathsf{C}$. Consider the following diagram (hereafter denoted as (1)).

```tikz
\usepackage{amsmath, amssymb, amsfonts, tikz-cd}
\usetikzlibrary{arrows, arrows.meta}
\tikzcdset{arrow style = tikz, diagrams = {>=stealth}}
\begin{document}
\begin{tikzcd}
\mathsf{C}(b,t) & \mathsf{C}(a,t) \\
\{*\} & \{*\}
\arrow["-\circ f", from=1-1, to=1-2]
\arrow["\eta_a", from=1-1, to=2-1]
\arrow["\text{id}_{\{*\}}", from=2-1, to=2-2]
\arrow["\eta_b", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

For all morphisms $g:b\to t$ we have $$\eta_{b}\circ (-\circ f)(g)=*=\text{id}_{\{*\}}\circ \eta_{a}(g),$$so by [[Extensionality of Functions]] (1) commutes.

We now show that for all objects $a$ in $\mathsf{C}$, $\eta_{a}$ is an isomorphism. Clearly $\eta_{a}$ is surjective. Now suppose $f,g\in \mathsf{C}(a,t)$, and suppose that $\eta_{a}(f)=\eta_{a}(g)$. By definition, we have $f:a\to t$ and $g:a\to t$. Since $t$ is terminal, we must have $f=g$. This means $\eta_{a}$ is injective, so $\eta_{a}$ is bijective and therefore an isomorphism by [[Bijective Functions as Isomorphisms]]. $\blacksquare$

**Proof of Backward Implication.** Suppose $h_{t}$ is naturally isomorphic to $\{*\}:\mathsf{C}^\text{op}\to \mathsf{Set}$. Suppose $a$ is an object in $\mathsf{C}$. Since $h_{t}$ is naturally isomorphic to $\{*\}$, there is an isomorphism $\eta_{a}:\{*\}\to \mathsf{C}(a,t)$. By [[Bijective Functions as Isomorphisms]] $\eta_{a}$ is a bijective function.
- **Existence.** We have $\eta_{a}(*):a\to t$.
- **Uniqueness.** Suppose $f:a\to t$ and $g:a\to t$ are morphisms in $\mathsf{C}$. Then, $f,g\in \mathsf{C}(a,t)$. Since $\eta_{a}$ is bijective, by [[Relation Inverses of Bijective Functions as Functions]] $\eta_{a}^{-1}$ is a function, so we have $\eta_{a}^{-1}(f),\eta_{a}^{-1}(g)\in\{*\}$. This means $\eta_{a}^{-1}(f)=\eta_{a}^{-1}(g)$, so by [[Compositions of Bijective Functions with Their Inverses as Identity Functions]] and [[Evaluations of Composite Functions]] $$\begin{align}
f & =\eta_{a}\circ \eta_{a}^{-1}(f) \\
 & =\eta_{a}(\eta_{a}^{-1}(f)) \\
 & =\eta_{a}(\eta_{a}^{-1}(g)) \\
 & =\eta_{a}\circ \eta_{a}^{-1}(g) \\
 & =g.\blacksquare
\end{align}$$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Constant Functor]]
- [[Natural Transformation]]
- [[Natural Isomorphism]]
- [[Hom-Functor]]
- [[Terminal Object]]
- [[Category of Sets]]
- [[Bijective Function]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]
- [[Relation Inverses of Bijective Functions as Functions]]
- [[Compositions of Bijective Functions with Their Inverses as Identity Functions]]
- [[Bijective Functions as Isomorphisms]]
- [[Singleton Sets as Terminal Objects]]