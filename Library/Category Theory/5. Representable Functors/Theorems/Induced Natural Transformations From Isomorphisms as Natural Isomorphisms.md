**Theorem.** Let $\mathsf{C}$ be a locally small category. Let $f:x\to y$ be a morphism in $\mathsf{C}$.
1. $f$ is an isomorphism if and only if $h^f:h^y\Rightarrow h^x$ is a natural isomorphism. Therefore, $x\cong y$ if and only if $h^x\cong h^y$.
2. $f$ is an isomorphism if and only if $h_{f}:h_{x}\Rightarrow h_{y}$ is a natural isomorphism. Therefore, $x\cong y$ if and only if $h_{x}\cong h_{y}$.

**Proof of First Statement.**
- **Forward Implication.** Suppose $f$ is an isomorphism. For all objects $a$ in $\mathsf{C}$ and morphisms $s:x\to a$, $$\begin{align}
(h^f\circ h^{f^{-1}})_{a}(s) & =(h^f)_{a}\circ (h^{f^{-1}})_{a}(s) \\
 & =(h^f)_{a}(s\circ f^{-1}) \\
 & =(s\circ f^{-1})\circ f \\
 & =s \\
 & =(\text{id}_{h^x})_{a}(s).
\end{align}$$Therefore, by [[Extensionality of Functions]], for all objects $a$ in $\mathsf{C}$ we have $(h^f\circ h^{f^{-1}})_{a}=(\text{id}_{h^x})_{a}$, so $$h^f\circ h^{f^{-1}}=\text{id}_{h^x}.$$ Also, for all objects $a$ in $\mathsf{C}$ and morphisms $s:y\to a$, $$\begin{align}
(h^{f^{-1}}\circ h^f)_{a}(s) & =(h^{f^{-1}})_{a}\circ (h^f)_{a}(s) \\
 & =(h^{f^{-1}})_{a}(s\circ f) \\
 & =(s\circ f)\circ f^{-1} \\
 & =s \\
 & =(\text{id}_{h^y})_{a}(s).
\end{align}$$Therefore, by [[Extensionality of Functions]], for all objects $a$ in $\mathsf{C}$ we have $(h^{f^{-1}}\circ h^f)_{a}=(\text{id}_{h^y})_{a}$, so $$h^{f^{-1}}\circ h^f=\text{id}_{h^y}.$$These show that $h^f$ is a natural isomorphism. $\blacksquare$
- **Backward Implication.** Suppose $h^f$ is a natural isomorphism. Then, there is $s:h^x\Rightarrow h^y$ such that $h^f\circ s=\text{id}_{h^x}$ and $s\circ h^f=\text{id}_{h^y}$. By [[Fullness and Faithfulness of Yoneda Embeddings]], $h^{\bullet}$ is full, so there is $g:y\to x$ such that $s=h^g$. We will show that $g=f^{-1}$.
  
  Since $h^f\circ h^g=\text{id}_{h^x}$, in particular $(h^f\circ h^g)_{x}=(\text{id}_{h^x})_{x}$, so $(h^f\circ h^g)_{x}(\text{id}_{x})=(\text{id}_{h^x})_{x}(\text{id}_{x})$. This means $$\begin{align}
&& (h^f)_{x}\circ h^g_{x}(\text{id}_{x}) & =\text{id}_{x} \\
\iff && (h^f)_{x}(\text{id}_{x}\circ g) & =\text{id}_{x} \\
\iff && (h^f)_{x}(g) & =\text{id}_{x} \\
\iff && g\circ f & =\text{id}_{x}.
\end{align}$$Using a similar reasoning, from $h^g\circ h^f=\text{id}_{h^y}$ we obtain $f\circ g=\text{id}_{y}$. This means $f$ is an isomorphism with inverse $g$. $\blacksquare$

**Proof of Second Statement.** This follows by applying [[Principle of Duality]] on the first statement. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Isomorphism]]
- [[Locally Small Category]]
- [[Vertical Composition of Natural Transformations]]
- [[Natural Isomorphism]]
- [[Hom-Functor]]
- [[Natural Transformation Between Hom-Functors]]

Theorems used:
- [[Principle of Duality]]
- [[Fullness and Faithfulness of Yoneda Embeddings]]
- [[Extensionality of Functions]]

