*Theorem.* For all natural numbers $a$, we have $0+a=a$.

*Proof.* Consider the set $$A=\{a\in \mathbb{N}\mid 0+a=a\}.$$We need to show that $A=\mathbb{N}$, so by induction it is enough to prove that $0\in A$ and $A$ is closed under $\mathsf{s}$.
- *First Statement.* Since $0$ is a left identity of addition, we have $0+0=0$, so $0\in A$.
- *Second Statement.* Suppose $a\in A$. Then, $0+a=a$. By recursion property of addition, we have $0+\mathsf{s}(a)=\mathsf{s}(0+a)$. Since $0+a=a$, we have $0+\mathsf{s}(a)=\mathsf{s}(a)$, so $\mathsf{s}(a)\in A$. $\blacksquare$