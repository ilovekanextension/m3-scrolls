**Theorem.** Let $G$ be a group. Let $N$ be a normal subgroup of $G$. Then, the function $\phi:G\to G/N$ defined as $$\phi(a)=a\circ N$$is a surjective group homomorphism.

**Proof.** We will first show that $\phi$ is a group homomorphism. Suppose $a,b\in G$. We have
$$\begin{align}
\phi(a\circ b) & =(a\circ b)\circ N \\
 & =(a\circ N)*(b\circ N) \\
 & =\phi(a)*\phi(b).\blacksquare
\end{align}$$
We now show that $\phi$ is surjective. Suppose $X\in G/N$. Then, there is $a\in G$ such that $X=a\circ N$. This means $\phi(a)=a\circ N=X$. $\blacksquare$
***
Definitions used:
- [[Group]]
- [[Group Homomorphism]]
- [[Subgroup]]
- [[Left and Right Coset]]
- [[Normal Subgroup]]
- [[Quotient Group
- [[Surjective Function]]]]