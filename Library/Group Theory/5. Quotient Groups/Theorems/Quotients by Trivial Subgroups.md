**Theorem.** Let $G$ be a group.
1. $\{1\}$ is a normal subgroup of $G$. Moreover, as groups, $$G/\{0\}\cong G.$$
2. $G$ is a normal subgroup of $G$. Moreover, as groups, $$G/G\cong \{1\}.$$

**Proof of First Statement.** By [[Trivial Subgroups]], $\{1\}$ is a subgroup of $G$. Now suppose $a\in G$ and $n\in\{1\}$. Then, $n=1$, so $$a\circ n\circ a^{-1}=a\circ 1\circ a^{-1}=1\in\{1\}.$$This shows that $\{1\}$ is normal. 

By [[Identity Functions as Group Homomorphisms]], $\text{id}_{G}$ is a group homomorphism $G\to G$. Clearly it is surjective, so by [[First Isomorphism Theorem for Groups]] $$\frac{G}{\ker(\text{id}_{G})}\cong G.$$We have
$$\begin{align}
\ker(\text{id}_{G}) & =\{a\in G\mid \text{id}_{G}(a)=1\} \\
 & =\{a\in G\mid a=1\} \\
 & =\{1\},
\end{align}$$
so the statement follows. $\blacksquare$

**Proof of Second Statement.** Clearly $G$ is normal in $G$.

Define a function $\phi:G\to\{1\}$ as $$\phi(a)=1.$$For all $a,b\in G$, $$\phi(a\circ b)=1=1\circ 1=\phi(a)\circ\phi(b),$$so $\phi$ is a group homomorphism. Clearly $\phi$ is surjective, so by [[First Isomorphism Theorem for Groups]] $$\frac{G}{\ker(\phi)}\cong\{1\}.$$We have
$$\begin{align}
\ker(\phi) & =\{a\in G\mid \phi(a)=1\} \\
 & =G,
\end{align}$$
so the statement follows. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Subgroup]]
- [[Normal Subgroup]]
- [[Quotient Group]]

Theorems used:
- [[Identity Functions as Group Homomorphisms]]
- [[Trivial Subgroups]]
- [[First Isomorphism Theorem for Groups]]