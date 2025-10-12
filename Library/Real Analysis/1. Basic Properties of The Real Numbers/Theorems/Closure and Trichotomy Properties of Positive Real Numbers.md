**Theorem.**
1. Suppose $a,b\in \mathbb{R}^+$. Then, $a+b\in \mathbb{R}^+$.
2. Suppose $a,b\in \mathbb{R}^+$. Then, $a\cdot b\in \mathbb{R}^+$.
3. Suppose $a\in \mathbb{R}$. Then, exactly one of the following holds:
	- $a\in \mathbb{R}^+$.
	- $-a\in \mathbb{R}^+$.
	- $a=0$.

**Proof of First Statement.** Since $a,b\in \mathbb{R}^+$, by definition we have $a>0$ and $b>0$. By the first order property, we then have $a+b>0+b$, so $a+b>b$. Since $<$ is a strict total order, by definition it is transitive, so since $a+b>b$ and $b>0$ we have $a+b>0$. By definition, we can conclude that $a+b\in \mathbb{R}^+$. $\blacksquare$

**Proof of Second Statement.** Since $a,b\in \mathbb{R}^+$, by definition we have $a>0$ and $b>0$. By the second order property, we then have $a\cdot b>0\cdot b$, so by [[Multiplications with Ring Zeros]] $a\cdot b>0$. By definition, this means $a\cdot b\in \mathbb{R}^+$. $\blacksquare$

**Proof of Third Statement.** Since $<$ is a strict total order, $<$ is trichotomous, so exactly one of the following holds:
- $0<a$.
- $a<0$.
- $a=0$.

The first point is equivalent to $a>0$, which is equivalent to $a\in \mathbb{R}^+$. To show that the second is equivalent to $-a\in \mathbb{R}^+$, observe that, by the first order property,
$$\begin{align}
a<0 & \iff a+(-a)<0+(-a) \\
 & \iff 0<-a \\
 & \iff-a>0 \\
 & \iff-a\in \mathbb{R}^+.\blacksquare
\end{align}$$
***
Definitions used:
- [[Real Numbers]]
- [[Strict Total Order]]

Theorems used:
- [[Multiplications with Ring Zeros]]