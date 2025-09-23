**Theorem.** Let $M=(M,\circ)$ and $N=(N,+)$ be monoids. Let $\phi:M\to N$ be a monoid homomorphism. Then, the following statements are equivalent.
1. There is a monoid homomorphism $\eta:N\to M$ such that $\eta\circ\phi=\text{id}_{M}$ and $\phi\circ\eta=\text{id}_{N}$.
2. $\phi$ is bijective.

**Proof of** $1\Rightarrow 2$. Suppose there is a monoid homomorphism $\eta:N\to M$ such that $\eta\circ\phi=\text{id}_{M}$ and $\phi\circ\eta=\text{id}_{N}$. Since monoid homomorphisms are functions, by [[Bijective Functions as Isomorphisms]] $\phi$ is bijective.

**Proof of** $2\Rightarrow 1$. Suppose $\phi$ is bijective. We will show that $\phi^{-1}$ is a monoid homomorphism; by [[Compositions of Bijective Functions with Their Inverses as Identity Functions]] the statement follows immediately.

By [[Values of Inverse Functions]], since $\phi(1_{M})=1_{N}$, we have $$\phi^{-1}(1_{N})=1_{M}.$$Now suppose $a,b\in N$. Since $\phi$ is bijective, it is surjective, so there are $x,y\in M$ such that $\phi(x)=a$ and $\phi(y)=b$. By [[Evaluations of Composite Functions]] and [[Values of Inverse Functions]],
$$\begin{align}
\phi^{-1}(a+b) & =\phi^{-1}(\phi(x)+\phi(y)) \\
 & =\phi^{-1}(\phi(x\circ y)) \\
 & =\phi^{-1}\circ\phi(x\circ y) \\
 & =\text{id}_{M}(x\circ y) \\
 & =x\circ y \\
 & =\phi^{-1}(a)\circ\phi^{-1}(b).\blacksquare
\end{align}$$
***
Definitions used:
- [[Monoid]]
- [[Monoid Homomorphism]]
- [[Identity Function]]
- [[Composition of Functions]]
- [[Surjective Function]]
- [[Bijective Function]]

Theorems used:
- [[Evaluations of Composite Functions]]
- [[Values of Inverse Functions]]
- [[Compositions of Bijective Functions with Their Inverses as Identity Functions]]
- [[Bijective Functions as Isomorphisms]]