**Theorem.** Let $A$ be a set. Suppose $F$ is a family of subsets of $A$. Then, the following statements are equivalent.
1. The following properties are satisfied.
	- For all $X\in F$, $X$ is nonempty.
	- $\bigcup F=A$.
	- For all $X,Y\in F$, if $X\cap Y$ is nonempty, then $X=Y$.
2. The following properties are satisfied.
	- For all $X\in F$, $X$ is nonempty.
	- For all $a\in A$, there is a unique $X\in F$ such that $a\in X$.

**Proof of** $1\Rightarrow 2$. Suppose that
- For all $X\in F$, $X$ is nonempty.
- $\bigcup F=A$.
- For all $X,Y\in F$, if $X\cap Y$ is nonempty, then $X=Y$.

Suppose $a\in A$.
- **Existence.** By the second point, $\bigcup F=A$, so $A\subseteq \bigcup F$. Therefore, $a\in\bigcup F$, so there is $X\in F$ such that $a\in X$.
- **Uniqueness.** Suppose $X,Y\in F$, and suppose that $a\in X$ and $a\in Y$. Then, $a\in X\cap Y$, so $X\cap Y$ is nonempty. By the third point, since $X\cap Y$ is nonempty, $X=Y$. $\blacksquare$

**Proof of** $2\Rightarrow 1$. Suppose that
- For all $X\in F$, $X$ is nonempty.
- For all $a\in A$, there is a unique $X\in F$ such that $a\in X$.

We first prove that $\bigcup F=A$. First suppose $a\in\bigcup F$. Then, there is $X\in F$ such that $a\in X$. Since $F$ is a family if subsets of $A$, $X\subseteq A$, so $a\in A$. Now suppose $a\in A$. By the second point, there is $X\in F$ such that $a\in X$. This means $a\in\bigcup F$.

We next prove that for all $X,Y\in F$, if $X\cap Y$ is nonempty, then $X=Y$. Suppose $X,Y\in F$, and suppose that $X\cap Y$ is nonempty. Then, there is $a\in X\cap Y$. We then have $a\in X$ and $a\in Y$. By the second point, there is a unique $Z\in F$ such that $a\in Z$, so we must have $X=Y$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Nonempty Set]]
- [[Intersection of Two Sets]]
- [[Union of Family of Sets]]