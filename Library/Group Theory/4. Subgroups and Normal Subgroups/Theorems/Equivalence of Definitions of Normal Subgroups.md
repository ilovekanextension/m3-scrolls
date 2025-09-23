**Theorem.** Let $G$ be a group. Let $N$ be a subgroup of $G$. Then, the following statements are equivalent.
1. For all $a\in G$ and $n\in N$, $a\circ n\circ a^{-1}\in N$.
2. For all $a\in G$, $a\circ N=N\circ a$.

**Proof of** $1\Rightarrow 2.$ Suppose that for all $a\in G$ and $n\in N$, $a\circ n\circ a^{-1}\in N$. Suppose $a\in G$. We will show that $a\circ N=N\circ a$.

Suppose $x\in a\circ N$. Then, there is $n\in N$ such that $x=a\circ n$. We then have $$x\circ a^{-1}=a\circ n\circ a^{-1}\in N,$$so by [[Criterion for Equality of Cosets]] $N\circ a=N\circ x$. Since $x\in N\circ x$, we have $x\in N\circ a$.
Next suppose $x\in N\circ a$. Then, there is $n\in N$ such that $x=n\circ a$. By [[Involution Property on Group Inverses]], $$a^{-1}\circ x=a^{-1}\circ n\circ a=a^{-1}\circ n\circ (a^{-1})^{-1}\in N,$$so by [[Criterion for Equality of Cosets]] $a\circ N=x\circ N$. Since $x\in N\circ x$, we have $x\in N\circ a$. $\blacksquare$

**Proof of** $2\Rightarrow 1$. Suppose that for all $a\in G$, $a\circ N=N\circ a$. Suppose $a\in G$ and $n\in N$. Then, $a\circ n\in a\circ N$, so $a\circ n\in N\circ a$. This means there is $m\in N$ such that $a\circ n=m\circ a$. We then have $$a\circ n\circ a^{-1}=m\in N.\blacksquare$$
***
Definitions used:
- [[Group]]
- [[Subgroup]]

Theorems used:
- [[Involution Property on Group Inverses]]
- [[Criterion for Equality of Cosets]]