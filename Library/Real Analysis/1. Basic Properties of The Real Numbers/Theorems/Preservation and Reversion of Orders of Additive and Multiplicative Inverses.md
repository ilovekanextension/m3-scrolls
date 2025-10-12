**Theorem.**
1. Suppose $a,b\in \mathbb{R}$, and suppose that $a<b$. Then, $-b<-a$.
2. Suppose $a\in \mathbb{R}$, and suppose that $a>0$. Then, $1/a>0$.
3. Suppose $a,b\in \mathbb{R}$. Suppose that $a\neq 0$ and $b\neq 0$, and suppose that $a<b$. Then, $1/b<1/a$.

**Proof of First Statement.** By the first order property, we have
$$\begin{align}
a<b & \iff a-a-b<b-a-b \\
 & \iff 0-b<0-a \\
 & \iff-b<-a.\blacksquare
\end{align}$$

**Proof of Second Statement.** Since $<$ is a strict total order, $<$ is trichotomous, so $1/a>0$ or $0>1/a$ or $1/a=0$. We will show that $\neg(0>1/a)$ and $\neg(1/a=0)$; from these we can conclude that $1/a>0$.

To prove that $\neg(0>1/a)$, assume for the sake of negation that $0>1/a$. Then, since $a>0$, we have $0\cdot a>(1/a) \cdot a$, so by [[Multiplications with Ring Zeros]] $0>1$. However, by [[Positivity of Squares of Real Numbers]] $1>0$. This contradicts the fact that $<$ is trichotomous: exactly one of $0<1$, $1<0$, and $1=0$ must hold. Therefore, the assumption that $0>1/a$ must be false, so $\neg(0>1/a)$.

To prove that $\neg(1/a=0)$, assume for the sake of negation that $1/a=0$. Then, by [[Multiplications with Ring Zeros]] $$1=(1/a)\cdot a=0\cdot a=0.$$This contradicts the fact that $\mathbb{R}$ is a field: by definition, fields are nontrivial, so $1\neq 0$. Therefore, the assumption that $1/a=0$ must be false, so $\neg(1/a=0)$. $\blacksquare$

**Proof of Third Statement.** Since $<$ is a strict total order, $<$ is trichotomous, so $a<0$ or $0<a$ or $a=0$. Since $a\neq 0$, we must have $a<0$ or $0<a$. By a similar reasoning, we can conclude that $b<0$ or $0<b$. We proceed by cases on the first disjunction; in each case we will show that $1/b<1/a$.
- **Case** $a<0$. By the first statement, this means $-0<-a$, so by [[Inverses of Group Identities]] $-a>0$. By the second statement, we then have $1/(-a)>0$, so by [[Multiplicative Inverses of Additive Inverses]] $-(1/a)>0$. Since $a<b$, by the second order property we have $a\cdot(-(1/a))<b\cdot(-(1/a))$, so by [[Multiplications with Additive Inverses]] $$-1=-(a\cdot(1/a))=a\cdot(-(1/a))<b\cdot(-(1/a))=-(b/a).$$