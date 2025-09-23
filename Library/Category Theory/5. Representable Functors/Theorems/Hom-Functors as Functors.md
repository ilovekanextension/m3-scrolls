**Theorem.** Let $\mathsf{C}$ be a locally small category. Suppose $x$ is an object in $\mathsf{C}$. Then, the map $H$ that assigns
- to each object $a$ in $\mathsf{C}$ the set $\mathsf{C}(x,a)$ and
- to each morphism $f:a\to b$ in $\mathsf{C}$ the post-composition function $f\circ -:\mathsf{C}(x,a)\to \mathsf{C}(x,b)$

is a functor from $\mathsf{C}$ to $\mathsf{Set}$. Likewise, the map $H$ that assigns
- to each object $a$ in $\mathsf{C}$ the set $\mathsf{C}(a,x)$ and
- to each morphism $f:a\to b$ in $\mathsf{C}$ the pre-composition function $-\circ f:\mathsf{C}(b,x)\to \mathsf{C}(a,x)$

is a functor from $\mathsf{C}^\text{op}$ to $\mathsf{Set}$.

**Proof of First Statement.**
- **Preservation of Identities.** Suppose $a$ is an object in $\mathsf{C}$. For all $s:x\to a$ we have  $$\begin{align}
H(\text{id}_{a})(s) & =\text{id}_{a}\circ s \\
 & =s \\
 & =\text{id}_{H(a)}(s),
\end{align}$$so by [[Extensionality of Functions]] $H(\text{id}_{a})=\text{id}_{H(a)}$.
- **Preservation of Composition.** Suppose $f:a\to b$ and $g:b\to c$ are morphisms in $\mathsf{C}$. By [[Evaluations of Composite Functions]], for all $s:x\to a$ we have  $$\begin{align}
H(g\circ f)(s) & =(g\circ f)\circ s \\
 & =g\circ (f\circ s) \\
 & =H(g)(f\circ s) \\
 & =H(g)(H(f)(s)) \\
 & =H(g)\circ H(f)(s),
\end{align}$$so by [[Extensionality of Functions]] $H(g\circ f)=H(g)\circ H(f)$. $\blacksquare$

**Proof of Second Statement.** This follows by applying [[Principle of Duality]] on the first statement. $\blacksquare$

***
Definitions used:
- [[Category]]
- [[Locally Small Category]]
- [[Functor]]
- [[Covariant and Contravariant Functor]]
- [[Category of Sets]]
- [[Function]]
- [[Composition of Functions]]

Theorems used:
- [[Principle of Duality]]
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]