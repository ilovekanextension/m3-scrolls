**Theorem.** Let $a,b,c\in \mathbb{R}$.
1. Suppose $a+c<b+c$. Then, $a<b$.
2. Suppose $a+c\leq b+c$. Then, $a\leq b$.
3. Suppose $c>0$, and suppose that $a\cdot c<b\cdot c$. Then, $a<b$.
4. Suppose $c>0$, and suppose that $a\cdot c\leq b\cdot c$. Then, $a\leq b$.

**Proof of First Statement.** We have
$$\begin{align}
a & =a+c-c \\
 & <b+c-c \\
 & =b.\blacksquare
\end{align}$$

**Proof of Second Statement.** By [[Basic Order Properties for Total Order on Real Numbers]],
$$\begin{align}
a & =a+c-c \\
 & \leq b+c-c \\
 & =b.\blacksquare
\end{align}$$

**Proof of Third Statement.** By [[Orders Between Additive and Multiplicative Inverses]], since $c>0$, we have $1/c>0$. Therefore,
$$\begin{align}
a & =a\cdot c\cdot(1/c) \\
 & <b\cdot c\cdot(1/c) \\
 & =b.\blacksquare
\end{align}$$

**Proof of Fourth Statement.** By [[Orders Between Additive and Multiplicative Inverses]], since $c>0$, we have $1/c>0$, so $1/c\geq 0$. Therefore, by [[Basic Order Properties for Total Order on Real Numbers]],
$$\begin{align}
a & =a\cdot c\cdot(1/c) \\
 & \leq b\cdot c\cdot(1/c) \\
 & =b.\blacksquare
\end{align}$$
***
Definitions used:
- [[Real Numbers]]
- [[Subtraction Notation on Rings]]

Theorems used:
- [[Basic Order Properties for Total Order on Real Numbers]]
- [[Orders Between Additive and Multiplicative Inverses]]