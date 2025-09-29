**Theorem.** Let $\mathsf{C}$ be a locally small category. Suppose $X$ is an object in $\mathsf{C}$. Then, the map $H$ that assigns
- to each object $A$ in $\mathsf{C}$ the set $\mathsf{C}(X,A)$ and
- to each morphism $f:A\to B$ in $\mathsf{C}$ the post-composition function $f\circ -:\mathsf{C}(X,A)\to \mathsf{C}(X,B)$

is a functor from $\mathsf{C}$ to $\mathsf{Set}$. Likewise, the map $H$ that assigns
- to each object $A$ in $\mathsf{C}$ the set $\mathsf{C}(A,X)$ and
- to each morphism $f:A\to B$ in $\mathsf{C}$ the pre-composition function $-\circ f:\mathsf{C}(B,X)\to \mathsf{C}(A,X)$

is a functor from $\mathsf{C}^\text{op}$ to $\mathsf{Set}$.

**Proof of First Statement.** First suppose $A$ is an object in $\mathsf{C}$. For all $s:X\to A$ we have
$$\begin{align}
[H(\text{id}_{A})](s) & =\text{id}_{A}\circ s \\
 & =s \\
 & =\text{id}_{H(A)}(s),
\end{align}$$
so by [[Extensionality of Functions]] $H(\text{id}_{A})=\text{id}_{H(A)}$.

Next suppose $f:A\to B$ and $g:B\to C$ are morphisms in $\mathsf{C}$. By [[Evaluations of Composite Functions]], for all $s:X\to A$ we have  $$\begin{align}
[H(g\circ f)](s) & =(g\circ f)\circ s \\
 & =g\circ (f\circ s) \\
 & =[H(g)](f\circ s) \\
 & =[H(g)]([H(f)](s)) \\
 & =[H(g)\circ H(f)](s),
\end{align}$$so by [[Extensionality of Functions]] $H(g\circ f)=H(g)\circ H(f)$. $\blacksquare$

**Proof of Second Statement.** First suppose $A$ is an object in $\mathsf{C}$. For all $s:A\to X$ we have
$$\begin{align}
[H(\text{id}_{A})](s) & =s\circ\text{id}_{A} \\
 & =s \\
 & =\text{id}_{H(A)}(s),
\end{align}$$
so by [[Extensionality of Functions]] $H(\text{id}_{A})=\text{id}_{H(A)}$.

Next suppose $f:A\to B$ and $g:B\to C$ are morphisms in $\mathsf{C}$. By [[Evaluations of Composite Functions]], for all $s:C\to X$ we have  $$\begin{align}
[H(g\circ f)](s) & =s\circ(g\circ f) \\
 & =(s\circ g)\circ f \\
 & =[H(f)](s\circ g) \\
 & =[H(f)]([H(g)](s)) \\
 & =[H(f)\circ H(g)](s),
\end{align}$$so by [[Extensionality of Functions]] $H(g\circ f)=H(f)\circ H(g)$. $\blacksquare$

***
Definitions used:
- [[Category]]
- [[Locally Small Category]]
- [[Opposite Category]]
- [[Functor]]
- [[Covariant and Contravariant Functor]]
- [[Category of Sets]]
- [[Function]]
- [[Composition of Functions]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]