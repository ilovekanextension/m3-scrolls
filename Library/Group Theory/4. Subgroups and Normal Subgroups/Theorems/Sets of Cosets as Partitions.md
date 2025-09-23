**Theorem.** Let $G$ be a group. Let $S$ be a subgroup of $G$.
1. $G/S$ is a partition of $G$.
2. $S\backslash G$ is a partition of $G$.

**Proof of First Statement.** First suppose $X\in G/S$. Then, there is $g\in G$ such that $X=g\circ S$. Since $S$ is a subgroup of $G$, we have $1\in G$, so $$g=g\circ 1\in g\circ S.$$This means $g\in X$, so $X$ is nonempty.

Next suppose $g\in G$.
- **Existence.** We have $g\in g\circ S$.
- **Uniqueness.** Suppose $X\in G/S$, and suppose that $g\in X$. Since $X\in G/S$, there is $h\in G$ such that $X=h\circ S$. Since $g\in X$, we have $g\in h\circ S$, so there is $s\in S$ such that $g=h\circ s$. This means $$h^{-1}\circ g=s\in S,$$so by [[Criterion for Equality of Cosets]] $h\circ S=g\circ S$. Therefore, $X=g\circ S$. $\blacksquare$

**Proof of Second Statement.** First suppose $X\in S\backslash G$. Then, there is $g\in G$ such that $X=S\circ g$. Since $S$ is a subgroup of $G$, we have $1\in G$, so $$g=1\circ g\in S\circ g.$$This means $g\in X$, so $X$ is nonempty.

Next suppose $g\in G$.
- **Existence.** We have $g\in S\circ g$.
- **Uniqueness.** Suppose $X\in S\backslash G$, and suppose that $g\in X$. Since $X\in S\backslash G$, there is $h\in G$ such that $X=S\circ h$. Since $g\in X$, we have $g\in S\circ h$, so there is $s\in S$ such that $g=s\circ h$. This means $$g\circ h^{-1}=s\in S,$$so by [[Criterion for Equality of Cosets]] $S\circ h=S\circ g$. Therefore, $X=S\circ g$. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Subgroup]]
- [[Left and Right Coset]]
- [[Partition of Set]]

Theorems used:
- [[Criterion for Equality of Cosets]]