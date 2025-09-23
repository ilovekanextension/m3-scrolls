**Theorem.** Let $G$ be a group. Let $N$ be a normal subgroup of $G$.
1. Suppose $T$ is a subgroup of $G/N$. Then, there is a subgroup $S$ of $G$ such that $T=S/N$.
2. Suppose $S$ is a subgroup of $G$, and suppose that $N\subseteq S$. Then, $S/N$ is a subgroup of $G/N$. Moreover, $S$ is normal in $G$ if and only if $S/N$ is normal in $G/N$.
3. Suppose $S$ is a normal subgroup of $G$, and suppose that $N\subseteq S$. Then, as groups, $$\frac{G}{S}\cong\frac{G/N}{S/N}.$$

**Proof of First Statement.** By [[Projection Functions on Quotient Groups as Group Homomorphisms]], the function $\phi:G\to G/N$ defined as $$\phi(a)=a\circ N$$is a surjective group homomorphism. By [[Preimages of Subgroups Under Group Homomorphisms as Subgroups]], since $T$ is a subgroup of $G/N$, $\phi^{-1}[T]$ is a subgroup of $G$. We will show that $T=\phi^{-1}[T]/N$.

First suppose $X\in T$. Since $T\subseteq G/N$, there is $a\in G$ such that $X=a\circ N$. By definition then, $$\phi(a)=a\circ N=X\in T,$$so $a\in \phi^{-1}[T]$. Therefore, $X=a\circ N\in \phi^{-1}[T]/N$. Now suppose $X\in \phi^{-1}[T]/N$. Then, there is $a\in \phi^{-1}[T]$ such that $X=a\circ N$. Since $a\in \phi^{-1}[T]$, we have $\phi(a)\in T$, so $X=a\circ N=\phi(a)\in T$. $\blacksquare$

**Proof of Second Statement.** We first show that $S/N$ is a subgroup of $G/N$.
- **Closure Under Identity.** Since $S$ is a subgroup of $G$, $1\in S$. Therefore, by [[Group Actions on Cosets]], $$N=1\circ N\in S/N.$$
- **Closure Under Composition.** Suppose $a\circ N\in S/N$ and $b\circ N\in S/N$. Then, $a\circ b\in S$, so $$(a\circ N)*(b\circ N)=(a\circ b)\circ N\in S/N.$$
- **Closure Under Identity.** Suppose $a\circ N\in S/N$. Then, $a^{-1}\in S$, so $$(a\circ N)^{-1}=a^{-1}\circ N\in S/N.$$

We now show that $S$ is normal in $G$ if and only if $S/N$ is normal in $G/N$. First suppose $S$ is normal in $G$. Suppose $A\in G/N$ and $T\in S/N$. Then, there is $a\in G$ and $t\in S$ such that $A=a\circ N$ and $T=t\circ N$. Since $S$ is normal, $a\circ t\circ a^{-1}\in S$, so
$$\begin{align}
A*T*A^{-1} & =(a\circ N)*(t\circ N)*(a\circ N)^{-1} \\
 & =(a\circ N)*(t\circ N)*(a^{-1}\circ N) \\
 & =(a\circ t\circ a^{-1})\circ N \\
 & \in S/N.
\end{align}$$
Now suppose $S/N$ is normal in $G/N$. Suppose $a\in G$ and $s\in S$. Then, $a\circ N\in G/N$ and $s\circ N\in S/N$. Since $S/N$ is normal, we must have
$$\begin{align}
(a\circ s\circ a^{-1})\circ N & =(a\circ N)*(s\circ N)*(a^{-1}\circ N) \\
 & =(a\circ N)*(s\circ N)*(a\circ N)^{-1} \\
 & \in S/N,
\end{align}$$
so by [[Criterion for Membership of Cosets in Quotient Groups]] $a\circ s\circ a^{-1}\in S$. $\blacksquare$

**Proof of Third Statement.** For clarity, denote the group operation in $(G/N)/(S/N)$ as $+$.

Since $S$ is normal in $G$, by the second statement $S/N$ is normal in $G/N$. Define a function $\phi:G\to(G/N)/(S/N)$ as $$\phi(a)=(a\circ N)*(S/N).$$We first show that $\phi$ is a group homomorphism. Suppose $a,b\in G$. We have
$$\begin{align}
\phi(a\circ b) & =((a\circ b)\circ N)*(S/N) \\
 & =((a\circ N)*(b\circ N))*(S/N) \\
 & =((a\circ N)*(S/N))+((b\circ N)*(S/N)) \\
 & =\phi(a)+\phi(b).
\end{align}$$
Next, we show that $\phi$ is surjective. Suppose $X\in(G/N)/(S/N)$. Then, there is $A\in G/N$ such that $X=A*(S/N)$. Since $A\in G/N$, there is $a\in G$ such that $A=a\circ N$. Therefore, $$X=(a\circ N)*(S/N)=\phi(a).$$
Since $\phi$ is a surjective group homomorphism, by [[First Isomorphism Theorem for Groups]] $$\frac{G}{\ker(\phi)}\cong\frac{G/N}{S/N}.$$Observe that, by [[Inverses of Group Identities]], [[Criterion for Equality of Cosets]], [[Group Actions on Cosets]], and [[Criterion for Membership of Cosets in Quotient Groups]],
$$\begin{align}
\ker(\phi) & =\{a\in G\mid \phi(a)=1_{(G/N)/(S/N)}\} \\
 & =\{a\in G\mid (a\circ N)*(S/N)=S/N\}, \\
 & =\{a\in G\mid (a\circ N)*(S/N)=1_{G/N}*(S/N)\} \\
 & =\{a\in G\mid 1_{G/N}^{-1}*(a\circ N)\in S/N\} \\
 & =\{a\in G\mid a\circ N\in S/N\} \\
 & =\{a\in G\mid a\in S\} \\
 & =S.\blacksquare
\end{align}$$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Subgroup]]
- [[Left and Right Coset]]
- [[Kernel of Group Homomorphism]]
- [[Normal Subgroup]]
- [[Quotient Group]]

Theorems used:
- [[Inverses of Group Identities]]
- [[Preimages of Subgroups Under Group Homomorphisms as Subgroups]]
- [[Criterion for Equality of Cosets]]
- [[Group Actions on Cosets]]
- [[Projection Functions on Quotient Groups as Group Homomorphisms]]
- [[First Isomorphism Theorem for Groups]]
- [[Criterion for Membership of Cosets in Quotient Groups]]