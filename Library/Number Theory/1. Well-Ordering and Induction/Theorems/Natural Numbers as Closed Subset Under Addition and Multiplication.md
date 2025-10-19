**Theorem.**
1. Let $m,n\in \mathbb{N}$. Then, $m+n\in \mathbb{N}$.
2. Let $m,n\in \mathbb{N}$. Then, $m\cdot n\in \mathbb{N}$.

**Proof of First Statement.** Define a proposition $\varphi$ on $\mathbb{N}$ as $$\varphi(y):\equiv \forall x\in \mathbb{N} \ (x+y\in \mathbb{N}).$$To prove the statement, it is enough to show that $\varphi(y)$ is true when $y=n$; from this we have $\forall x\in \mathbb{N} \ (x+n\in \mathbb{N})$, so in particular, since $m\in \mathbb{N}$ we have $m+n\in \mathbb{N}$. We will show by [[Principle of Mathematical Induction]] that $\varphi(y)$ is actually true for all $y\in \mathbb{N}$.
- **Base Case.** Suppose $x\in \mathbb{N}$. Then, $x+0=x\in \mathbb{N}$. Therefore, $\varphi(0)$ is true.
- **Induction Step.** Suppose $y\in \mathbb{N}$, and suppose that $\varphi(y)$ is true. Suppose $x\in \mathbb{N}$. Since $\varphi(y)$ is true and $x\in \mathbb{N}$, we have $x+y\in \mathbb{N}$. By definition of $\mathbb{N}$, we then have $$x+(y+1)=(x+y)+1\in \mathbb{N}.$$Therefore, $\varphi(y+1)$ is also true. $\blacksquare$

**Proof of Second Statement.** Define a proposition $\varphi$ on $\mathbb{N}$ as  $$\varphi(y):\equiv \forall x\in \mathbb{N} \ (x\cdot y\in \mathbb{N}).$$To prove the statement, it is enough to show that $\varphi(y)$ is true when $y=n$; from this we have $\forall x\in \mathbb{N} \ (x\cdot n\in \mathbb{N})$, so in particular, since $m\in \mathbb{N}$ we have $m\cdot n\in \mathbb{N}$. We will show by [[Principle of Mathematical Induction]] that $\varphi(y)$ is actually true for all $y\in \mathbb{N}$.
- **Base Case.** Suppose $x\in \mathbb{N}$. By definition, $0\in \mathbb{N}$, so by [[Multiplications with Ring Zeros]] $x\cdot 0\in \mathbb{N}$. Therefore, $\varphi(0)$ is true.
- **Induction Step.** Suppose $y\in \mathbb{N}$, and suppose that $\varphi(y)$ is true. Suppose $x\in \mathbb{N}$. Since $\varphi(y)$ is true and $x\in \mathbb{N}$, we have $x\cdot y\in \mathbb{N}$. We also have $x\in \mathbb{N}$, so by the first statement $$x\cdot(y+1)=x\cdot y+x\cdot 1=x\cdot y+x\in \mathbb{N}.$$Therefore, $\varphi(y+1)$ is also true. $\blacksquare$

***
Definitions used:
- [[Natural Numbers]]

Theorems used:
- [[Principle of Mathematical Induction]]
- [[Multiplications with Ring Zeros]]