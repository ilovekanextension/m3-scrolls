*Theorem.*
1. Zero is the smallest natural number under comparison. That is, for all $a\in \mathbb{N}$ we have $0\leq a$.
2. Zero is a minimal natural number under comparison. That is, for all $a\in \mathbb{N}$, if $a\leq 0$, then $a=0$.

*Proof of First Statement.* Suppose $a\in \mathbb{N}$. We have $a=0+a$, so $0\leq a$. $\blacksquare$

*Proof of Second Statement.* Consider the set $$A=\{a\in \mathbb{N}\mid a\leq 0\Rightarrow a=0\}.$$We need to show that $A=\mathbb{N}$, so by induction it is enough to prove that $0\in A$ and $A$ is closed under $\mathsf{s}$.
- *First Statement.* Suppose $0\leq 0$. Clearly $0=0$, so $0\in A$.
- *Second Statement.* Suppose $a\in A$. Suppose $\mathsf{s}(a)\leq 0$. Then, there is $k\in \mathbb{N}$ such that $0=\mathsf{s}(a)+k$. By [[Commutativity of Recursion Property of Natural Number Addition]], $0=\mathsf{s}(a+k)$. Since no natural numbers $a$ satisfy $\mathsf{s}(a)=0$, by explosion we can conclude that $\mathsf{s}(a)=0$. $\blacksquare$