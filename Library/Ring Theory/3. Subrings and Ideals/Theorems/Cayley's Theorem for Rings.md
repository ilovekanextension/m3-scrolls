**Theorem.** Let $R$ be a ring. Then, there is a subring $S$ of $\text{End}(R)$ such that $R\cong S$.

**Proof.** By [[Left Multiplications By Elements of Rings as Group Endomorphisms]], the function $\phi:R\to \text{End}(R)$ defined as $$\phi(a)=a\cdot-$$is well-defined. We first show that $\phi$ is a ring homomorphism.
- **Preservation of Additions.** Suppose $a,b\in R$. For all $r\in R$ we have $$\begin{align}
\phi(a+b)(r) & =(a+b)\cdot r \\
 & =a\cdot r+b\cdot r \\
 & =\phi(a)(r)+\phi(b)(r) \\
 & =(\phi(a)+\phi(b))(r),
\end{align}$$so by [[Extensionality of Functions]] $\phi(a+b)=\phi(a)+\phi(b)$.
- **Preservation of Multiplications.** Suppose $a,b\in R$. By [[Evaluations of Composite Functions]], for all $r\in R$ we have $$\begin{align}
\phi(a\cdot b)(r) & =(a\cdot b)\cdot r \\
 & =a\cdot(b\cdot r) \\
 & =\phi(a)(b\cdot r) \\
 & =\phi(a)(\phi(b)(r)) \\
 & =\phi(a)\circ\phi(b)(r),
\end{align}$$so by [[Extensionality of Functions]] $\phi(a\cdot b)=\phi(a)\circ\phi(b)$.
- **Preservation of Multiplicative Identities.** For all $r\in R$ we have $$\begin{align}
\phi(1)(r) & =1\cdot r \\
 & =r \\
 & =\text{id}_{R}(r),
\end{align}$$so by [[Extensionality of Functions]] $\phi(1)=\text{id}_{R}$.

Now consider the restriction $\phi:R\to \text{im}(\phi)$. Clearly it is surjective. We will show that it is also injective; the statement follows by [[Images of Ring Homomorphisms as Subrings]].

Suppose $a,b\in R$ satisfy $\phi(a)=\phi(b)$. Then, $a\cdot-=b\cdot-$, so by [[Extensionality of Functions]] $$a=a\cdot 1=a\cdot-(1)=b\cdot-(1)=b\cdot 1=b.\blacksquare$$
***
Definitions used:
- [[Ring]]
- [[Ring Homomorphism]]
- [[Subring]]
- [[Endomorphism Ring]]
- [[Injective Function]]
- [[Image of Function]]

Theorems used:
- [[Images of Ring Homomorphisms as Subrings]]
- [[Left Multiplications By Elements of Rings as Group Endomorphisms]]
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]