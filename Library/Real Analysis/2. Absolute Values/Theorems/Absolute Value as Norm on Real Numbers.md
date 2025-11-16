**Theorem.**
1. Suppose $a,b\in \mathbb{R}$. Then, $|a+b|\leq|a|+|b|$.
2. Suppose $a,b\in \mathbb{R}$. Then, $|a\cdot b|=|a|\cdot|b|$.
3. Suppose $a\in \mathbb{R}$. Then, $|a|=0$ if and only if $a=0$.
4. Suppose $a\in \mathbb{R}$. Then, $|a|\geq 0$.

**Proof of First Statement.** Since $\leq$ is a total order, we have $a\leq 0$ or $0\leq a$. Likewise, we also have $b\leq 0$ or $0\leq b$. We will explicitly prove the statement for the cases $a\leq 0\wedge b\leq 0$ and $a\leq 0\wedge 0\leq b$; by symmetry, the other two cases are proven in a similar way.
- **Case** $a\leq 0\wedge b\leq 0$. This means $|a|=-a$ and $|b|=-b$. Also, by [[Preservation of Total Orders Under Addition and Multiplication]], $a+b\leq 0$, so $|a+b|=-(a+b)$. Therefore, by [[Inverses of Group Compositions]], $$|a+b|=-(a+b)=-a+(-b)=|a|+|b|,$$so $|a+b|\leq|a|+|b|$.
- **Case** $a\leq 0\wedge 0\leq b$. This means $|a|=-a$ and $|b|=b$. By totality of $\leq$, we have $a+b\leq 0$ or $0\leq a+b$. We proceed by cases.
	- **Case** $a+b\leq 0$. This means $|a+b|=-(a+b)$. Since $0\leq b$, by [[Orders Between Additive and Multiplicative Inverses]] and [[Inverses of Group Identities]] $-b\leq 0$. Since $0\leq b$ and $-b\leq 0$, by transitivity of $\leq$ we have $-b\leq b$, so $$|a+b|=-(a+b)=-a+(-b)\leq-a+b=|a|+|b|.$$
	- **Case** $0\leq a+b$. This means $|a+b|=a+b$. Since $a\leq 0$, by [[Orders Between Additive and Multiplicative Inverses]] and [[Inverses of Group Identities]] $0\leq -a$. Since $a\leq 0$ and $0\leq -a$, by transitivity of $\leq$ we have $a\leq -a$, so $$|a+b|=a+b\leq -a+b=|a|+|b|.\blacksquare$$

**Proof of Second Statement.** Since $\leq$ is a total order, we have $a\leq 0$ or $0\leq a$. Likewise, we also have $b\leq 0$ or $0\leq b$. We will explicitly prove the statement for the cases $a\leq 0\wedge b\leq 0$ and $a\leq 0\wedge 0\leq b$; by symmetry, the other two cases are proven in a similar way.
- **Case** $a\leq 0\wedge b\leq 0$. This means $|a|=-a$ and $|b|=-b$. Also, by [[Orders Between Additive and Multiplicative Inverses]] and [[Inverses of Group Identities]] $0\leq -a$ and $0\leq -b$. Thus, by [[Closure and Trichotomy Properties of Positive and Nonnegative Real Numbers]] $0\leq (-a)\cdot(-b)$, so by [[Multiplications with Additive Inverses]] $0\leq a\cdot b$. Therefore, $$|a\cdot b|=a\cdot b=(-a)\cdot(-b)=|a|\cdot|b|.$$
- **Case** $a\leq 0\wedge 0\leq b$. This means $|a|=-a$ and $|b|=b$. Also, by [[Orders Between Additive and Multiplicative Inverses]] and [[Inverses of Group Identities]] $0\leq-a$. Thus, by [[Closure and Trichotomy Properties of Positive and Nonnegative Real Numbers]] $0\leq (-a)\cdot b$, so by [[Multiplications with Additive Inverses]] $0\leq -(a\cdot b)$, which means $a\cdot b\leq 0$. Therefore, $$|a\cdot b|=-(a\cdot b)=(-a)\cdot b=|a|\cdot |b|.\blacksquare$$

**Proof of Third Statement.**
- **Forward Implication.** Suppose $|a|=0$. By trichotomy of $<$, we have $a<0$, $a=0$, or $0<a$. We will show that $\neg(a<0)$ and $\neg(0<a)$; from this we can conclude that $a=0$.
  
  To prove that $\neg(a<0)$, assume for the sake of negation that $a<0$. Then, $a\leq 0$, so $|a|=-a$. Since $|a|=0$, we then must have $-a=0$, so $a=0$. This contradicts the fact that $a<0$.
  
  To prove that $\neg(0<a)$, assume for the sake of negation that $0<a$. Then, $0\leq a$, so $|a|=a$. Since $|a|=0$, we then must have $a=0$. This contradicts the fact that $0<a$.
- **Backward Implication.** Suppose $a=0$. Then, $a\geq 0$, so $|a|=a=0$. $\blacksquare$

**Proof of Fourth Statement.** First observe that, by [[Positivity of Squares of Real Numbers]], $1\geq0$, so by [[Orders Between Additive and Multiplicative Inverses]] and [[Inverses of Group Identities]] $-1\leq 0$. This means $|{-1}|=-(-1)=1$. Now, by [[Multiplications with Additive Inverses of Ring Ones]], [[Multiplications with Ring Zeros]], and the first, second, and third statement above, since $a+(-a)=0$, we have
$$\begin{align}
2\cdot 0 & =0 \\
 & =|0| \\
 & =|a+(-a)| \\
 & \leq|a|+|{-a}| \\
 & =|a|+|(-1)\cdot a| \\
 & =|a|+|{-1}|\cdot|a| \\
 & =|a|+1\cdot|a| \\
 & =2\cdot|a|.
\end{align}$$
Since $1>0$, we have $2=1+1>1+0=1$, so by transitivity $2>0$. Therefore, by [[Cancellation Properties on Orders Between Real Numbers]], since $2\cdot 0\leq 2\cdot|a|$, we must have $0\leq |a|$. $\blacksquare$
***
Definitions used:
- [[Real Numbers]]
- [[Absolute Value]]

Theorems used:
- [[Closure and Trichotomy Properties of Positive and Nonnegative Real Numbers]]
- [[Positivity of Squares of Real Numbers]]
- [[Preservation of Total Orders Under Addition and Multiplication]]
- [[Orders Between Additive and Multiplicative Inverses]]
- [[Cancellation Properties on Orders Between Real Numbers]]
- [[Multiplications with Ring Zeros]]
- [[Multiplications with Additive Inverses]]
- [[Multiplications with Additive Inverses of Ring Ones]]
- [[Inverses of Group Identities]]
- [[Inverses of Group Compositions]]