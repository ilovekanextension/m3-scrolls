**Theorem.** Let $\mathsf{I}$ and $\mathsf{C}$ be categories, and suppose that $\mathsf{I}$ is small. Let $F:\mathsf{I}\to \mathsf{C}$. Then, the map $H$ that assigns
- to each object $A$ in $\mathsf{C}^\text{op}$ the set $\text{Cone}(A,F)$ in $\mathsf{Set}$ and
- to each morphism $f:A\to B$ in $\mathsf{C}^\text{op}$ the function $\text{Cone}(B,F)\to \text{Cone}(A,F)$ that maps a cone $(B,\sigma)$ to the cone $(A,\nu)$, where $\nu$ is the natural transformation (well-defined by [[Change of Legs of Cones and Cocones by Compositions with Morphisms]]) defined as $$\nu_{X}=\sigma_{X}\circ f$$

is a functor from $\mathsf{C}^\text{op}$ to $\mathsf{Set}$. Likewise, the map $H$ that assigns
- to each object $A$ in $\mathsf{C}$ the set $\text{Cone}(F,A)$ in $\mathsf{Set}$ and
- to each morphism $f:A\to B$ in $\mathsf{C}$ the function $\text{Cone}(F,A)\to \text{Cone}(F,B)$ that maps a cone $(A,\sigma)$ to the cone $(B,\nu)$, where $\nu$ is the natural transformation (well-defined by [[Change of Legs of Cones and Cocones by Compositions with Morphisms]]) defined as $$\nu_{X}=f\circ\sigma_{X}$$

is a functor from $\mathsf{C}$ to $\mathsf{Set}$.

**Proof of First Statement.** First suppose $A$ is an object in $\mathsf{C}$. Suppose $(A,\sigma)$ is a cone in $\text{Cone}(A,F)$. By definition, $[H(\text{id}_{A})](A,\sigma)$ is the cone $(A,\nu)$ with $\nu$ defined as $$\nu_{X}=\sigma_{X}\circ\text{id}_{A}=\sigma_{X}.$$Therefore, $\nu=\sigma$. This means
$$\begin{align}
[H(\text{id}_{A})](A,\sigma) & =(A,\nu) \\
 & =(A,\sigma) \\
 & =\text{id}_{\text{Cone}(A,F)}(A,\sigma) \\
 & =\text{id}_{H(A)}(A,\sigma).
\end{align}$$
By [[Extensionality of Functions]], we can conclude that $H(\text{id}_{A})=\text{id}_{H(A)}$.

Next suppose $f:A\to B$ and $g:B\to C$ are morphisms in $\mathsf{C}$. Suppose $(C,\eta)$ is a cone in $\text{Cone}(C,F)$. By definition, $[H(g)](C,\eta)$ is the cone $(B,\sigma)$ with $\sigma$ defined as $$\sigma_{X}=\eta_{X}\circ g.$$Also by definition, $[H(f)](B,\sigma)$ is the cone $(A,\nu)$ with $\nu$ defined as $$\nu_{X}=\sigma_{X}\circ f.$$Notice that $[H(g\circ f)](C,\eta)$ is the cone $(A,\nu')$ with $\nu'$ defined as $$\nu'_{X}=\eta_{X}\circ(g\circ f)=(\eta_{X}\circ g)\circ f=\sigma_{X}\circ f=\nu_{X}.$$Therefore, $\nu'=\nu$, so $(A,\nu')=(A,\nu)$. By [[Evaluations of Composite Functions]], this means
$$\begin{align}
[H(g\circ f)](C,\eta) & =(A,\nu') \\
 & =(A,\nu) \\
 & =[H(f)](B,\sigma) \\
 & =[H(f)]([H(g)](C,\eta)) \\
 & =[H(f)\circ H(g)](C,\eta).
\end{align}$$
By [[Extensionality of Functions]], we can conclude that $H(g\circ f)=H(f)\circ H(g)$. $\blacksquare$

**Proof of Second Statement.** First suppose $A$ is an object in $\mathsf{C}$. Suppose $(A,\sigma)$ is a cone in $\text{Cone}(F,A)$. By definition, $[H(\text{id}_{A})](A,\sigma)$ is the cone $(A,\nu)$ with $\nu$ defined as $$\nu_{X}=\text{id}_{A}\circ\sigma_{X}=\sigma_{X}.$$Therefore, $\nu=\sigma$. This means
$$\begin{align}
[H(\text{id}_{A})](A,\sigma) & =(A,\nu) \\
 & =(A,\sigma) \\
 & =\text{id}_{\text{Cone}(F,A)}(A,\sigma) \\
 & =\text{id}_{H(A)}(A,\sigma).
\end{align}$$
By [[Extensionality of Functions]], we can conclude that $H(\text{id}_{A})=\text{id}_{H(A)}$.

Next suppose $f:A\to B$ and $g:B\to C$ are morphisms in $\mathsf{C}$. Suppose $(A,\eta)$ is a cone in $\text{Cone}(F,A)$. By definition, $[H(f)](A,\eta)$ is the cone $(B,\sigma)$ with $\sigma$ defined as $$\sigma_{X}=f\circ\eta_{X}.$$Also by definition, $[H(g)](B,\sigma)$ is the cone $(C,\nu)$ with $\nu$ defined as $$\nu_{X}=g\circ\sigma_{X}.$$Notice that $[H(g\circ f)](C,\eta)$ is the cone $(C,\nu')$ with $\nu'$ defined as $$\nu'_{X}=(g\circ f)\circ\eta_{X}=g\circ(f\circ \eta_{X})\circ f=g\circ\sigma_{X}\circ f=\nu_{X}.$$Therefore, $\nu'=\nu$, so $(A,\nu')=(A,\nu)$. By [[Evaluations of Composite Functions]], this means
$$\begin{align}
[H(g\circ f)](A,\eta) & =(C,\nu') \\
 & =(C,\nu) \\
 & =[H(g)](B,\sigma) \\
 & =[H(g)]([H(f)](A,\eta)) \\
 & =[H(g)\circ H(f)](A,\eta).
\end{align}$$
By [[Extensionality of Functions]], we can conclude that $H(g\circ f)=H(g)\circ H(f)$. $\blacksquare$
***
Definitions used:
- [[Category]]
- [[Small Category]]
- [[Opposite Category]]
- [[Functor]]
- [[Categorical Diagram]]
- [[Covariant and Contravariant Functor]]
- [[Constant Functor]]
- [[Natural Transformation]]

Theorems used:
- [[Change of Legs of Cones and Cocones by Compositions with Morphisms]]
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]