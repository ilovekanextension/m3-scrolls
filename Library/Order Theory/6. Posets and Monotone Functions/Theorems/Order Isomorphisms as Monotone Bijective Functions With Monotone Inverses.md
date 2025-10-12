**Theorem.** Let $A$ and $B$ be posets. Let $f:A\to B$. Then, the following statements are equivalent.
1. $f$ is an isomorphism in $\mathsf{Pos}$.
2. $f$ is bijective, and the inverse function $f^{-1}$ is monotone.

**Proof of** $1\Rightarrow 2$. Suppose $f$ is an isomorphism in $\mathsf{Pos}$. Then, $f$ is a monotone function, and there is a monotone function $g:B\to A$ such that $g\circ f=\text{id}_{A}$ and $f\circ g=\text{id}_{B}$. By [[Bijective Functions as Isomorphisms]], this means $f$ is bijective.

To prove that $f^{-1}$ is monotone, suppose $x,y\in B$, and suppose that $x\leq y$. Since $f$ is bijective, $f$ is surjective, so there are $a,b\in A$ such that $f(a)=x$ and $f(b)=y$. Since $x\leq y$, we then have $f(a)\leq f(b)$. Since $g$ is monotone, $g(f(a))\leq g(f(b))$, so by [[Evaluations of Composite Functions]] $g\circ f(a)\leq g\circ f(b)$. By [[Extensionality of Functions]], this means $$a=\text{id}_{A}(a)=g\circ f(a)\leq g\circ f(b)=\text{id}_{A}(b)=b,$$ so $a\leq b$. By [[Values of Inverse Functions]], this means $f^{-1}(x)\leq f^{-1}(y)$. $\blacksquare$

**Proof of** $2\Rightarrow 1$. Suppose that $f$ is bijective and $f^{-1}$ is monotone. Then, both $f$ and $f^{-1}$ are morphisms in $\mathsf{Pos}$. Moreover, by [[Compositions of Bijective Functions with Their Inverses as Identity Functions]], $f^{-1}\circ f=\text{id}_{A}$ and $f\circ f^{-1}=\text{id}_{B}$. Therefore, by definition $f$ is an isomorphism in $\mathsf{Pos}$ with inverse $f^{-1}$. $\blacksquare$
***
Definitions used:
- [[Poset]]
- [[Monotone Function]]
- [[Category of Posets]]
- [[Function]]
- [[Bijective Function]]
- [[Inverse of Bijective Function]]
- [[Isomorphism]]

Theorems used:
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]
- [[Compositions of Bijective Functions with Their Inverses as Identity Functions]]
- [[Values of Inverse Functions]]
- [[Bijective Functions as Isomorphisms]]