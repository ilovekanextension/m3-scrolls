**Theorem.** Let $A$ be a set. Suppose $F$ is a partition of $A$. Then, there is an equivalence relation $\sim$ on $A$ such that $A/{\sim}=F$.

**Proof.** Define $${\sim}=\bigcup_{X\in F}(X\times X)=\{(a,b)\in A\times A\mid \exists X\in F \ ((a,b)\in X\times X)\}.$$We will first show that $\sim$ is an equivalence relation.
- **Reflexivity.** Suppose $a\in A$. Since $F$ is a partition of $A$, there is $X\in F$ such that $a\in X$. Then, $(a,a)\in X\times X$, so $(a,a)\in{\sim}$.
- **Symmetry.** Suppose $a,b\in A$, and suppose that $(a,b)\in{\sim}$. Then, there is $X\in F$ such that $(a,b)\in X\times X$. We then have $a\in X$ and $b\in X$, so $(b,a)\in X\times X$ and therefore $(b,a)\in{\sim}$.
- **Transitivity.** Suppose $a,b,c\in A$, and suppose that $(a,b)\in{\sim}$ and $(b,c)\in{\sim}$. Then, there are $X\in F$ and $Y\in F$ such that $(a,b)\in X\times X$ and $(b,c)\in Y\times Y$. We then have $a,b\in X$ and $b,c\in Y$. Since $F$ is a partition, the set $Z$ such that $b\in Z$ is unique. Since $b\in X$ and $b\in Y$, we therefore must have $X=Y$. This means $a\in X$ and $c\in X$, so $(a,c)\in X\times X$ and therefore $(a,c)\in{\sim}$.

We now show that $A/{\sim}=F$.
- **Forward Implication.** Suppose $X\in A/{\sim}$. Then, $X=[a]_{\sim}$ for some $a\in A$. Since $F$ is a partition, there is a unique $Y\in F$ such that $a\in Y$. First suppose $x\in X$. Then, $x\in[a]_{\sim}$, so $x\sim a$. This means there is $Z\in F$ such that $(x,a)\in Z\times Z$. Since $a\in Y$ and $a\in Z$, we must have $Y=Z$, so $x\in Y$. Now suppose $x\in Y$. Then, $(x,a)\in Y\times Y$, so $x\sim a$. This means $x\in[a]_{\sim}$, so $x\in X$. We therefore have $X=Y$, so $X\in F$.
- **Backward Implication.** Suppose $X\in F$. Since $F$ is a partition, $X$ is nonempty, so there is $a\in X$. We will show that $X=[a]_{\sim}$. First suppose $x\in X$. Then, $(x,a)\in X\times X$, so $x\sim a$ and therefore $x\in[a]_{\sim}$. Now suppose $x\in[a]_{\sim}$. Then, $x\sim a$. Since $a\in X$, by a recurring argument $x\in X$. We therefore have $X=[a]_{\sim}$, so $X\in A/{\sim}$. $\blacksquare$

***
Definitions used:
- [[Set]]
- [[Nonempty Set]]
- [[Equivalence Relation]]
- [[Equivalence Class]]
- [[Quotient Set]]
- [[Partition of Set]]