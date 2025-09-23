**Theorem.** Let $R$ be a commutative ring. Let $I$ be an ideal of $R$. Then, $I$ is maximal if and only if $I\neq(1)$ and for all ideals $J$ of $R$, $$I\subseteq J\Rightarrow(J=I\vee J=R).$$
**Proof of Forward Implication.** Suppose $I$ is maximal.

We first show that $I\neq(1)$. Since $I$ is maximal, by [[Maximal Ideals as Prime Ideals]] $I$ is prime, so by [[Criterion for Prime Ideals]] $I\neq(1)$.

Now suppose $J$ is an ideal of $R$, and suppose that $I\subseteq J$. Then, by [[Third Isomorphism Theorem for Rings]] $J/I$ is an ideal of $R/I$. Since $I$ is maximal, $R/I$ is a field, so by [[Fields as Nontrivial Commutative Rings With Only Trivial Ideals]] $J/I=(0+I)$ or $J/I=(1+I)$. We proceed by cases; in each case we will show that $J=I$ or $J=R$.
- **Case** $J/I=(0+I)$. We will show that $J=I$. First suppose $x\in J$. Then, $x+I\in J/I$, so $x+I\in(0+I)$. This means there is $y\in R$ such that $$x+I=(y+I)\cdot(0+I)=(y\cdot 0)+I.$$By [[Multiplications with Ring Zeros]], $y\cdot 0=0$, so $x+I=0+I$. By [[Criterion for Equality of Cosets]], this means $x\in I$. Now suppose $x\in I$. Then, by [[Criterion for Equality of Cosets]] $x+I=0+I$. We have $0+I\in(0+I)$, so $x+I\in(0+I)$. Since $J/I=(0+I)$, we then have $x+I\in J/I$. By [[Criterion for Membership of Cosets in Quotient Groups]], this means $x\in J$.
- **Case** $J/I=(1+I)$. We will show that $J=R$. By definition, $J\subseteq R$. Now suppose $x\in R$. Then, $x+I\in R/I$. By [[Special Ideals as Principal Ideals]], $(1+I)=R/I$, so $x+I\in(1+I)$. Since $J/I=(1+I)$, this means $x+I\in J/I$, so by [[Criterion for Membership of Cosets in Quotient Groups]] $x\in J$. $\blacksquare$

**Proof of Backward Implication.** Suppose that $I\neq(1)$ and for all ideals $J$ of $R$, $$I\subseteq J\Rightarrow(J=I\vee J=R).$$To show that $I$ is maximal, we will show that $R/I$ is a field. By [[Fields as Nontrivial Commutative Rings With Only Trivial Ideals]], it is enough to show that $R/I$ is nontrivial and that for all ideals $J$ of $R/I$, we have $J=(0+I)$ or $J=(1+I)$.

First assume for the sake of negation that $R/I$ is trivial. Then, by [[Triviality of Self-Quotient Rings]] $I=(1)$. This contradicts the assumption that $I\neq(1)$. Therefore, the assumption that $R/I$ is trivial must be false, so $R/I$ is nontrivial.

Next suppose $J$ is an ideal of $R/I$. Then, by [[Third Isomorphism Theorem for Rings]] there is an ideal $K$ of $R$ with $I\subseteq K$ such that $J=K/I$. Since $I\subseteq K$, this means $K=I$ or $K=R$. In each cases respectively, by [[Quotients by Trivial Subgroups]] and [[Special Ideals as Principal Ideals]], $$J=I/I=(0+I)$$and $$J=R/I=(1+I).\blacksquare$$
***
Definitions used:
- [[Ring]]
- [[Commutative Ring]]
- [[Ideal]]
- [[Quotient Ring]]
- [[Principal Ideal]]
- [[Field]]
- [[Maximal Ideal]]

Theorems used:
- [[Multiplications with Ring Zeros]]
- [[Third Isomorphism Theorem for Rings]]
- [[Triviality of Self-Quotient Rings]]
- [[Special Ideals as Principal Ideals]]
- [[Criterion for Prime Ideals]]
- [[Fields as Nontrivial Commutative Rings With Only Trivial Ideals]]
- [[Maximal Ideals as Prime Ideals]]
- [[Criterion for Equality of Cosets]]
- [[Quotients by Trivial Subgroups]]
- [[Criterion for Membership of Cosets in Quotient Groups]]