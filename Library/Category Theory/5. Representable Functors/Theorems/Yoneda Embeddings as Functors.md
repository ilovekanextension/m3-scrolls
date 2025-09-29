**Theorem.** Let $\mathsf{C}$ be a locally small category. Then, the map $H$ that assigns
- to each object $X$ in $\mathsf{C}$ the functor $h^X$ and
- to each morphism $f:X\to Y$ in $\mathsf{C}$ the natural transformation $h^f:h^Y\Rightarrow h^X$

is a functor from $\mathsf{C}^\text{op}$ to $\mathsf{Set}^\mathsf{C}$. Likewise, the map $H$ that assigns
- to each object $X$ in $\mathsf{C}$ the functor $h_{X}$ and
- to each morphism $f:X\to Y$ in $\mathsf{C}$ the natural transformation $h_{f}:h_{X}\Rightarrow h_{Y}$

is a functor from $\mathsf{C}$ to $\mathsf{Set}^{\mathsf{C}^\text{op}}$.

**Proof of First Statement.** First suppose $X$ is an object in $\mathsf{C}$. For all objects $A$ in $\mathsf{C}$ and morphisms $s:X\to A$, $$\begin{align}
[h^{\text{id}_{X}}]_{A}(s) & =s\circ \text{id}_{X} \\
 & =s \\
 & =\text{id}_{\mathsf{C}(X,A)}(s) \\
 & =(\text{id}_{h^X})_{A}(s).
\end{align}$$Therefore, by [[Extensionality of Functions]] $h^{\text{id}_{X}}=\text{id}_{h^X}$. Next suppose $f:X\to Y$ and $g:Y\to Z$ are morphisms in $\mathsf{C}$. For all objects $A$ in $\mathsf{C}$ and morphisms $s:Z\to A$, $$\begin{align}
[h^{g\circ f}]_{A}(s) & =s\circ(g\circ f) \\
 & =(s\circ g)\circ f \\
 & =(h^f)_{A}(s\circ g) \\
 & =[(h^f)_{A}]((h^g)_{A}(s)) \\
 & =[(h^f)_{A}\circ (h^g)_{A}](s).
\end{align}$$Therefore, by [[Extensionality of Functions]] $h^{g\circ f}=h^f\circ h^g$. $\blacksquare$

**Proof of Second Statement.** First suppose $X$ is an object in $\mathsf{C}$. For all objects $A$ in $\mathsf{C}$ and morphisms $s:A\to X$, $$\begin{align}
[h_{\text{id}_{X}}]_{A}(s) & =\text{id}_{X}\circ s \\
 & =s \\
 & =\text{id}_{\mathsf{C}(A,X)}(s) \\
 & =(\text{id}_{h_{X}})_{A}(s).
\end{align}$$Therefore, by [[Extensionality of Functions]] $h_{\text{id}_{X}}=\text{id}_{h_{X}}$. Next suppose $f:X\to Y$ and $g:Y\to Z$ are morphisms in $\mathsf{C}$. For all objects $A$ in $\mathsf{C}$ and morphisms $s:A\to X$,
$$\begin{align}
[h_{g\circ f}]_{A}(s) & =(g\circ f)\circ s \\
 & =g\circ (f\circ s) \\
 & =(h_{g})_{A}(f\circ s) \\
 & =(h_{g})_{A}((h_{f})_{A}(s)) \\
 & =(h_{g})_{A}\circ (h_{f})_{A}(s).
\end{align}$$
Therefore, by [[Extensionality of Functions]] $h^{g\circ f}=h^f\circ h^g$. $\blacksquare$

***
Definitions used:
- [[Category]]
- [[Locally Small Category]]
- [[Opposite Category]]
- [[Functor]]
- [[Natural Transformation]]
- [[Functor Category]]
- [[Hom-Functor]]
- [[Natural Transformation Between Hom-Functors]]
- [[Function]]
- [[Composition of Functions]]
- [[Category of Sets]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]