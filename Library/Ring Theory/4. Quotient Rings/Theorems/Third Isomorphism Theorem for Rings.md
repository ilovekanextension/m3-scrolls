**Theorem.** Let $R$ be a ring. Let $I$ be an ideal of $R$.
1. Suppose $K$ is an ideal of $R/I$. Then, there is an ideal $J$ of $R$ such that $K=J/I$.
2. Suppose $J$ is a subgroup of $R$, and suppose that $I\subseteq J$. Then, $J$ is an ideal of $R$ if and only if $J/I$ is an ideal of $R/I$.
3. Suppose $J$ is an ideal of $R$, and suppose that $I\subseteq J$. Then, as rings, $$\frac{R/I}{J/I}\cong \frac{R}{J}.$$

**Proof of First Statement.** Since $K$ is an ideal of $R/I$, by definition it is a subgroup of $R/I$, so by [[Third Isomorphism Theorem for Groups]] there is a subgroup $J$ of $R$ such that $K=J/I$. We will show that $J$ is an ideal of $R$.

Suppose $r\in R$ and $a\in J$. Then, $a+I\in J/I$, so $a+I\in K$. Since $K$ is an ideal and $r+I\in R/I$, we have $$(a\cdot r)+I=(a+I)\cdot(r+I)\in K,$$so by [[Criterion for Membership of Cosets in Quotient Groups]] $a\cdot r\in J$. Likewise, $$(r\cdot a)+I=(r+I)\cdot(a+I)\in K,$$so by [[Criterion for Membership of Cosets in Quotient Groups]] $r\cdot a\in J$. $\blacksquare$

**Proof of Second Statement.**
- **Forward Implication.** Suppose $J$ is an ideal of $R$. Suppose $X\in R/I$ and $Y\in J/I$. Then, there is $r\in R$ and $a\in J$ such that $X=r+I$ and $Y=a+I$. Since $J$ is an ideal, $r\cdot a\in J$ and $a\cdot r\in J$, so $$X\cdot Y=(r+I)\cdot(a+I)=(r\cdot a)+I\in J/I$$and $$Y\cdot X=(a+I)\cdot(r+I)=(a\cdot r)+I\in J/I.$$
- **Backward Implication.** Suppose $J/I$ is an ideal of $R/I$. Suppose $r\in R$ and $a\in J$. Then, $r+I\in R/I$ and $a+I\in J/I$. Since $J/I$ is an ideal, $$(r\cdot a)+I=(r+I)\cdot(a+I)\in J/I$$and $$(a\cdot r)+I=(a+I)\cdot(r+I)\in J/I,$$so by [[Criterion for Membership of Cosets in Quotient Groups]] $r\cdot a\in J$ and $a\cdot r\in J$. $\blacksquare$

**Proof of Third Statement.** By [[Third Isomorphism Theorem for Groups]], the function $\phi:R\to(R/I)/(J/I)$ defined as $$\phi(a)=(a+I)+(J/I)$$is a surjective group homomorphism with $\ker(\phi)=J$. We will show that $\phi$ is a ring homomorphism. From here, $\phi$ is then a surjective ring homomorphism, so by [[First Isomorphism Theorem for Rings]] the statement follows.
- **Preservation of Multiplications.** Suppose $a,b\in R$. We have $$\begin{align}
\phi(a\cdot b) & =((a\cdot b)+I)+(J/I) \\
 & =((a+I)\cdot(b+I))+(J/I) \\
 & =((a+I)+(J/I))\cdot((b+I)+(J/I)) \\
 & =\phi(a)\cdot \phi(b).
\end{align}$$
- **Preservation of Multiplicative Identities.** We have $$\begin{align}
\phi(1_{R}) & =(1_{R}+I)+(J/I) \\
 & =1_{R/I}+(J/I) \\
 & =1_{(R/I)/(J/I)}.\blacksquare
\end{align}$$
***
Definitions used:
- [[Ring]]
- [[Ring Homomorphism]]
- [[Ring Isomorphism]]
- [[Ideal]]
- [[Quotient Ring]]
- [[Group Homomorphism]]
- [[Subgroup]]
- [[Left and Right Coset]]
- [[Kernel of Group Homomorphism]]
- [[Quotient Group]]
- [[Surjective Function]]

Theorems used:
- [[First Isomorphism Theorem for Rings]]
- [[Criterion for Membership of Cosets in Quotient Groups]]
- [[Third Isomorphism Theorem for Groups]]

