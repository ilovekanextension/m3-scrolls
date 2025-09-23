**Theorem.** Let $G=(G,\circ)$ and $H=(H,+)$ be groups. Let $\phi:G\to H$ be a group homomorphism. Then, the following statements are equivalent.
1. There is a group homomorphism $\eta:H\to G$ such that $\eta\circ\phi=\text{id}_{G}$ and $\phi\circ\eta=\text{id}_{H}$.
2. $\phi$ is bijective.

**Proof of** $1\Rightarrow 2$. Suppose there is a group homomorphism $\eta:H\to G$ such that $\eta\circ\phi=\text{id}_{G}$ and $\phi\circ\eta=\text{id}_{H}$. Since group homomorphisms are functions, by [[Bijective Functions as Isomorphisms]] $\phi$ is bijective. $\blacksquare$

**Proof of** $2\Rightarrow 1$. Suppose $\phi$ is bijective. We will show that $\phi^{-1}$ is a group homomorphism; by [[Compositions of Bijective Functions with Their Inverses as Identity Functions]] the statement follows immediately.

Suppose $a,b\in H$. Since $\phi$ is bijective, it is surjective, so there are $x,y\in G$ such that $\phi(x)=a$ and $\phi(y)=b$. By [[Evaluations of Composite Functions]] and [[Values of Inverse Functions]],
$$\begin{align}
\phi^{-1}(a+b) & =\phi^{-1}(\phi(x)+\phi(y)) \\
 & =\phi^{-1}(\phi(x\circ y)) \\
 & =\phi^{-1}\circ\phi(x\circ y) \\
 & =\text{id}_{G}(x\circ y) \\
 & =x\circ y \\
 & =\phi^{-1}(a)\circ\phi^{-1}(b).\blacksquare
\end{align}$$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Identity Function]]
- [[Composition of Functions]]
- [[Surjective Function]]
- [[Bijective Function]]

Theorems used:
- [[Evaluations of Composite Functions]]
- [[Compositions of Bijective Functions with Their Inverses as Identity Functions]]
- [[Bijective Functions as Isomorphisms]]
- [[Values of Inverse Functions]]