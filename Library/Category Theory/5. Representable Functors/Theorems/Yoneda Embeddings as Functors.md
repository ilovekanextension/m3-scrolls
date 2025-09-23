**Theorem.** Let $\mathsf{C}$ be a locally small category. Then, the map $H$ that assigns
- to each object $x$ in $\mathsf{C}$ the functor $h^x$ and
- to each morphism $f:x\to y$ in $\mathsf{C}$ the natural transformation $h^f:h^y\Rightarrow h^x$

is a functor from $\mathsf{C}^\text{op}$ to $\mathsf{Set}^\mathsf{C}$. Likewise, the map $H$ that assigns
- to each object $x$ in $\mathsf{C}$ the functor $h_{x}$ and
- to each morphism $f:x\to y$ in $\mathsf{C}$ the natural transformation $h_{f}:h_{x}\Rightarrow h_{y}$

is a functor from $\mathsf{C}$ to $\mathsf{Set}^{\mathsf{C}^\text{op}}$.

**Proof of First Statement.**
- **Preservation of Identities.** Suppose $x$ is an object in $\mathsf{C}$. For all objects $a$ in $\mathsf{C}$ and morphisms $s:x\to a$, $$\begin{align}
(h^{\text{id}_{x}})_{a}(s) & =s\circ \text{id}_{x} \\
 & =s \\
 & =\text{id}_{\mathsf{C}(x,a)}(s) \\
 & =(\text{id}_{h^x})_{a}(s).
\end{align}$$Therefore, by [[Extensionality of Functions]], for all objects $a$ in $\mathsf{C}$ we have $(h^{\text{id}_{x}})_{a}=(\text{id}_{h^x})_{a}$, so $$h^{\text{id}_{x}}=\text{id}_{h^x}.$$
- **Preservation of Composition.** Suppose $f:x\to y$ and $g:y\to z$ are morphisms in $\mathsf{C}$. For all objects $a$ in $\mathsf{C}$ and morphisms $s:z\to a$, $$\begin{align}
(h^{g\circ f})_{a}(s) & =s\circ(g\circ f) \\
 & =(s\circ g)\circ f \\
 & =(h^f)_{a}(s\circ g) \\
 & =(h^f)_{a}((h^g)_{a}(s)) \\
 & =(h^f)_{a}\circ (h^g)_{a}(s).
\end{align}$$Therefore, by [[Extensionality of Functions]], for all objects $a$ in $\mathsf{C}$ we have $(h^{g\circ f})_{a}=(h^f)_{a}\circ (h^g)_{a}$, so $$h^{g\circ f}=h^f\circ h^g.\blacksquare$$

**Proof of Second Statement.** This follows by applying [[Principle of Duality]] on the first statement. $\blacksquare$

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
- [[Principle of Duality]]
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]