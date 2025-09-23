**Theorem.** Let $R$ be a commutative ring. Let $I$ be an ideal of $R$. Then, $I$ is prime if and only if $I\neq(1)$ and for all $a,b\in I$, $$a\cdot b\in I\iff(a\in I\vee b\in I).$$
**Proof of Forward Implication.** Suppose $I$ is prime.

To prove that $I\neq(1)$, assume for the sake of negation that $I=(1)$. Then, by [[Triviality of Self-Quotient Rings]], $R/I$ is trivial. This contradicts the assumption that $I$ is prime. Therefore, the assumption that $I=(1)$ must be false, so $I\neq(1)$.

Now suppose $a,b\in I$. 
- **Forward Implication.** Suppose $a\cdot b\in I$. By [[Criterion for Equality of Cosets]], this means $(a\cdot b)+I=0+I$, so $$(a+I)\cdot(b+I)=(a\cdot b)+I=0+I.$$Since $I$ is prime, $R/I$ is an integral domain, so $a+I=0+I$ or $b+I=0+I$. By [[Criterion for Equality of Cosets]], this means $a\in I$ or $b\in I$.
- **Backward Implication.** Suppose $a\in I$ or $b\in I$. We proceed by cases; in each case we will show that $a\cdot b\in I$.
	- **Case** $a\in I$. By [[Criterion for Equality of Cosets]], this means $a+I=0+I$. By [[Multiplications with Ring Zeros]], $$(a\cdot b)+I=(a+I)\cdot(b+I)=(0+I)\cdot(b+I)=(0\cdot b)+I=0+I,$$so $a\cdot b\in I$.
	- **Case** $b\in I$. By [[Criterion for Equality of Cosets]], this means $b+I=0+I$. By [[Multiplications with Ring Zeros]], $$(a\cdot b)+I=(a+I)\cdot(b+I)=(a+I)\cdot(0+I)=(a\cdot 0)+I=0+I,$$so $a\cdot b\in I$. $\blacksquare$

**Proof of Backward Implication.** Suppose that $I\neq(1)$ and for all $a,b\in I$, $$a\cdot b\in I\iff(a\in I\vee b\in I).$$To show that $I$ is prime, we will show that $R/I$ is an integral domain.
First assume for the sake of negation that $R/I$ is trivial. Then, by [[Triviality of Self-Quotient Rings]] $I=(1)$. This contradicts the assumption that $I\neq(1)$. Therefore, the assumption that $R/I$ is trivial must be false, so $R/I$ is nontrivial.

Now suppose $X\in R/I$ and $Y\in R/I$, and suppose that $X\cdot Y=0+I$. Then, there is $x,y\in R$ such that $X=x+I$ and $Y=y+I$. We then have $$(x\cdot y)+I=(x+I)\cdot(y+I)=0+I,$$so by [[Criterion for Equality of Cosets]] $x\cdot y\in I$. By assumption, this means $x\in I$ or $y\in I$, so by [[Criterion for Equality of Cosets]] $x+I=0+I$ or $y+I=0+I$. Therefore, $X=0+I$ or $Y=0+I$. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Commutative Ring]]
- [[Ideal]]
- [[Quotient Ring]]
- [[Principal Ideal]]
- [[Integral Domain]]
- [[Prime Ideal]]
- [[Left and Right Coset]]

Theorems used:
- [[Multiplications with Ring Zeros]]
- [[Special Ideals as Principal Ideals]]
- [[Criterion for Equality of Cosets]]