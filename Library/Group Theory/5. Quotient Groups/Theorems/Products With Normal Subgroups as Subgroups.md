**Theorem.** Let $G$ be a group. Let $S$ and $N$ be subgroups of $G$, and suppose that $N$ is normal in $G$.
1. The set $$S\circ N=\{s\circ n\in G\mid s\in S\wedge n\in N\}$$is a subgroup of $G$. Moreover, $N$ is a normal subgroup of $S\circ N$.
2. The set $S\cap N$ is a normal subgroup of $S$.

**Proof of First Statement.** We first show that $S\circ N$ is a subgroup of $G$.
- **Closure Under Identity.** Since $S$ and $N$ are subgroups, $1\in S$ and $1\in N$. Therefore, $1=1\circ 1\in S\circ N$.
- **Closure Under Composition.** Suppose $a,b\in S\circ N$. Then, there is $s,t\in S$ and $m,n\in N$ such that $a=s\circ m$ and $b=t\circ n$. Since $N$ is normal, $N\circ t=t\circ N$. Since $m\circ t\in N\circ t$, we then have $m\circ t\in t\circ N$, so there is $m'\in N$ such that $$m\circ t=t\circ m'.$$Therefore, $$a\circ b=s\circ m\circ t\circ n=s\circ t\circ m'\circ n\in S\circ N.$$
- **Closure Under Inverses.** Suppose $a\in S\circ N$. Then, there is $s\in S$ and $n\in N$ such that $a=s\circ n$. Since $N$ is normal, $N\circ s^{-1}=s^{-1}\circ N$. Since $n^{-1}\circ s^{-1}\in N\circ s^{-1}$, we then have $n^{-1}\circ s^{-1}\in s^{-1}\circ N$, so there is $n'\in N$ such that $$n^{-1}\circ s^{-1}=s^{-1}\circ n.$$Therefore, by [[Inverses of Group Compositions]], $$a^{-1}=(s\circ n)^{-1}=n^{-1}\circ s^{-1}=s^{-1}\circ n\in S\circ N.$$

We now show that $N$ is a normal subgroup of $S\circ N$. Suppose $a\in S\circ N$ and $n\in N$. Since $S\circ N$ is a subgroup of $G$, $a\in G$. Since $N$ is normal, we then have $a\circ n\circ a^{-1}\in N$. $\blacksquare$

**Proof of Second Statement.** Suppose $a\in S$ and $x\in S\cap N$. We will show that $a\circ x\circ a^{-1}\in S\cap N$.

Since $x\in S\cap N$, we have $x\in S$. Therefore, $a\circ x\circ a^{-1}\in S$. Also, since $x\in S\cap N$, we have $x\in N$. Since $N$ is normal, $a\circ x\circ a^{-1}\in N$. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Subgroup]]
- [[Normal Subgroup]]
- [[Set Builder Notation]]
- [[Intersection of Two Sets]]

Theorems used:
- [[Inverses of Group Compositions]]