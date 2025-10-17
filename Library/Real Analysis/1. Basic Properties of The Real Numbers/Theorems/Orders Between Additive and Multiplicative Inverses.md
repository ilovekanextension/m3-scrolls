**Theorem.**
1. Suppose $a,b\in \mathbb{R}$, and suppose that $a<b$. Then, $-b<-a$.
2. Suppose $a,b\in \mathbb{R}$, and suppose that $a\leq b$. Then, $-b\leq-a$.
3. Suppose $a\in \mathbb{R}$, and suppose that $a>0$. Then, $1/a>0$.
4. Suppose $a,b\in \mathbb{R}$. Suppose that $a>0$ and $b>0$, and suppose that $a<b$. Then, $1/b<1/a$.
5. Suppose $a,b\in \mathbb{R}$. Suppose that $a>0$ and $b>0$, and suppose that $a\leq b$. Then, $1/b\leq1/a$.

**Proof of First Statement.** By the first order property, we have
$$\begin{align}
a<b & \iff a-a-b<b-a-b \\
 & \iff 0-b<0-a \\
 & \iff-b<-a.\blacksquare
\end{align}$$

**Proof of Second Statement.** By [[Basic Order Properties for Total Order on Real Numbers]], we have
$$\begin{align}
a\leq b & \iff a-a-b\leq b-a-b \\
 & \iff 0-b\leq 0-a \\
 & \iff-b\leq -a.\blacksquare
\end{align}$$

**Proof of Third Statement.** Since $<$ is a strict total order, $<$ is trichotomous, so $1/a>0$ or $0>1/a$ or $1/a=0$. We will show that $\neg(0>1/a)$ and $\neg(1/a=0)$; from these we can conclude that $1/a>0$.

To prove that $\neg(0>1/a)$, assume for the sake of negation that $0>1/a$. Then, since $a>0$, we have $0\cdot a>(1/a) \cdot a$, so by [[Multiplications with Ring Zeros]] $0>1$. However, by [[Positivity of Squares of Real Numbers]] $1>0$. This contradicts the fact that $<$ is trichotomous: exactly one of $0<1$, $1<0$, and $1=0$ must hold. Therefore, the assumption that $0>1/a$ must be false, so $\neg(0>1/a)$.

To prove that $\neg(1/a=0)$, assume for the sake of negation that $1/a=0$. Then, by [[Multiplications with Ring Zeros]] $$1=(1/a)\cdot a=0\cdot a=0.$$This contradicts the fact that $\mathbb{R}$ is a field: by definition, fields are nontrivial, so $1\neq 0$. Therefore, the assumption that $1/a=0$ must be false, so $\neg(1/a=0)$. $\blacksquare$

**Proof of Fourth Statement.** Since $a>0$ and $b>0$, by the third statement we have $1/a>0$ and $1/b>0$. By the second order property, since $a<b$ we have
$$\begin{align}
& a\cdot(1/a)\cdot(1/b)<b\cdot(1/a)\cdot(1/b) \\
 & \Rightarrow 1\cdot(1/b)<1\cdot(1/a) \\
 & \Rightarrow 1/b<1/a.\blacksquare
\end{align}$$

**Proof of Fifth Statement.** Since $a>0$ and $b>0$, by the third statement we have $1/a>0$ and $1/b>0$, so $1/a\geq 0$ and $1/b\geq 0$. By the second order property, since $a\leq b$ we have
$$\begin{align}
& a\cdot(1/a)\cdot(1/b)\leq b\cdot(1/a)\cdot(1/b) \\
 & \Rightarrow 1\cdot(1/b)\leq 1\cdot(1/a) \\
 & \Rightarrow 1/b\leq 1/a.\blacksquare
\end{align}$$
***
Definitions used:
- [[Real Numbers]]
- [[Strict Total Order]]
- [[Subtraction Notation on Rings]]
- [[Field]]

Theorems used:
- [[Positivity of Squares of Real Numbers]]
- [[Multiplications with Ring Zeros]]