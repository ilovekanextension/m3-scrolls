**Theorem.** Let $A$ be a set. Then, there does not exist a surjective function from $A$ to $\mathcal{P}(A)$.

**Proof.** For the sake of contradiction, assume that there is a surjective function $f:A\to\mathcal{P}(A)$. Since $f$ is surjective, for all subsets $S$ of $A$ there is $a\in A$ such that $f(a)=S$. In particular, the set $$X=\{x\in A\mid x\notin f(x)\}$$is a subset of $A$, so there is $a\in A$ such that $f(a)=X$. Now, by the Law of Excluded Middle, we have $a\in X$ or $a\notin X$. We proceed by cases; in each case we will show a contradiction.
- **Case** $a\in X$. By definition of $X$, this means $a\notin f(a)$. Since $f(a)=X$, this means $a\notin X$, which contradicts the fact that $a\in X$.
- **Case** $a\notin X$. By definition of $X$, this means $a\in X$, which is a contradiction.

Since in both cases we obtain a contradiction, the assumption that there is a surjective function from $A$ to $\mathcal{P}(A)$ must be false. Therefore, there is no surjective function from $A$ to $\mathcal{P}(A)$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Set Builder Notation]]
- [[Function]]
- [[Surjective Function]]
- [[Power Set]]