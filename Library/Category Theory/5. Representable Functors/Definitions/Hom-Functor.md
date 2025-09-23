**Definition.** Let $\mathsf{C}$ be a locally small category. Suppose $x$ is an object in $\mathsf{C}$. By [[Hom-Functors as Functors]], the map that assigns
- to each object $a$ in $\mathsf{C}$ the set $\mathsf{C}(x,a)$ and
- to each morphism $f:a\to b$ in $\mathsf{C}$ the post-composition function $f\circ -:\mathsf{C}(x,a)\to \mathsf{C}(x,b)$

is a functor from $\mathsf{C}$ to $\mathsf{Set}$, and the map that assigns
- to each object $a$ in $\mathsf{C}$ the set $\mathsf{C}(a,x)$ and
- to each morphism $f:a\to b$ in $\mathsf{C}$ the pre-composition function $-\circ f:\mathsf{C}(b,x)\to \mathsf{C}(a,x)$

is a functor from $\mathsf{C}^\text{op}$ to $\mathsf{Set}$. The former and the latter are denoted as $h^x$ and $h_{x}$ respectively. Functors taking either of these forms are called **hom-functors**.
***
Definitions used:
- [[Category]]
- [[Locally Small Category]]
- [[Functor]]
- [[Covariant and Contravariant Functor]]
- [[Category of Sets]]
- [[Function]]

Theorems used:
- [[Hom-Functors as Functors]]