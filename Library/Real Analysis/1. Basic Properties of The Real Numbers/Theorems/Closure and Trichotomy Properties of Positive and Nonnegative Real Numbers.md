**Theorem.**
1. Suppose $a>0$ and $b>0$. Then, $a+b>0$.
2. Suppose $a\geq 0$ and $b\geq 0$. Then, $a+b\geq 0$.
3. Suppose $a>0$ and $b>0$. Then, $a\cdot b>0$.
4. Suppose $a\geq 0$ and $b\geq 0$. Then, $a\cdot b\geq 0$.
5. Suppose $a\in \mathbb{R}$. Then, exactly one of the following holds:
	- $a>0$.
	- $-a>0$.
	- $a=0$.

**Proof of First Statement.** Since $a>0$ and $b>0$, by the first order property we have $a+b>0+b$, so $a+b>b$. Since $<$ is a strict total order, by definition it is transitive, so since $a+b>b$ and $b>0$ we have $a+b>0$. $\blacksquare$

**Proof of Second Statement.** Since $a\geq 0$ and $b\geq 0$, by [[Basic Order Properties for Total Order on Real Numbers]] we have $a+b\geq 0+b$, so $a+b\geq b$. Since $\leq$ is a total order, by definition it is transitive, so since $a+b\geq b$ and $b\geq 0$ we have $a+b\geq 0$. $\blacksquare$

**Proof of Third Statement.** Since $a>0$ and $b>0$, by the second order property we have $a\cdot b>0\cdot b$, so by [[Multiplications with Ring Zeros]] $a\cdot b>0$. $\blacksquare$

**Proof of Fourth Statement.** Since $a\geq 0$ and $b\geq 0$, by [[Basic Order Properties for Total Order on Real Numbers]] we have $a\cdot b\geq 0\cdot b$, so by [[Multiplications with Ring Zeros]] $a\cdot b\geq 0$.

**Proof of Fifth Statement.** Since $<$ is a strict total order, $<$ is trichotomous, so exactly one of the following holds:
- $0<a$.
- $a<0$.
- $a=0$.

The first point is equivalent to $a>0$. To show that the second is equivalent to $-a>0$, observe that, by the first order property,
$$\begin{align}
a<0 & \iff a+(-a)<0+(-a) \\
 & \iff 0<-a \\
 & \iff-a>0.\blacksquare
\end{align}$$
***
Definitions used:
- [[Real Numbers]]
- [[Strict Total Order]]

Theorems used:
- [[Basic Order Properties for Total Order on Real Numbers]]
- [[Multiplications with Ring Zeros]]