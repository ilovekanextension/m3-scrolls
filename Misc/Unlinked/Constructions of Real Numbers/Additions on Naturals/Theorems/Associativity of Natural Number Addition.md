*Theorem.* For all natural numbers $a$, $b$, and $c$, we have $(a+b)+c=a+(b+c)$.

*Proof.* Consider the set $$A=\{b\in \mathbb{N}\mid \forall a,c\in \mathbb{N} \ ((a+b)+c=a+(b+c))\}.$$We need to show that $A=\mathbb{N}$, so it is enough to prove that $0\in A$ and $A$ is closed under $\mathsf{s}$.
- *First Statement.* Suppose $a,c\in \mathbb{N}$. By [[Zero as Right Identity of Natural Number Addition]], $0$ is the identity of addition, so we have $(a+0)+c=a+c=a+(0+c)$. This shows that $0\in A$.
- *Second Statement.* Suppose $b\in A$. Suppose $a,c\in \mathbb{N}$. Then, $(a+b)+c=a+(b+c)$. By recursion and [[Commutativity of Recursion Property of Natural Number Addition]], we have  $$\begin{align}
(a+\mathsf{s}(b))+c & =\mathsf{s}(a+b)+c \\
 & =\mathsf{s}((a+b)+c) \\
 & =\mathsf{s}(a+(b+c)) \\
 & =a+\mathsf{s}(b+c) \\
 & =a+(\mathsf{s}(b)+c).\blacksquare
\end{align}$$