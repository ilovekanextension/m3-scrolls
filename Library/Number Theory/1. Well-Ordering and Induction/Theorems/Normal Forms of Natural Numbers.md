**Theorem.** Let $n\in \mathbb{N}$. Then, $n=0$ or $n=k+1$ for some $k\in \mathbb{N}$.

**Proof.** Define a proposition $\varphi$ on $\mathbb{N}$ as $$\varphi(x):\equiv x=0\vee(\exists k\in \mathbb{N} \ (x=k+1)).$$To prove the statement, it is enough to show that $\varphi(x)$ is true when $x=n$. We will show by [[Principle of Mathematical Induction]] that $\varphi(x)$ is actually true for all $x\in \mathbb{N}$.
- **Base Case.** By reflexivity, $0=0$. Therefore, $\varphi(0)$ is true.
- **Induction Step.** Suppose $x\in \mathbb{N}$, and suppose that $\varphi(x)$ is true. Then, $x=0$ or $x=k+1$ for some $k\in \mathbb{N}$. We proceed by cases, in each case we will show that $\varphi(x+1)$ is true.
	- **Case** $x=0$. Pick $k=0$. Since $x=0$, we have $$x+1=0+1=k+1.$$Therefore, $\varphi(x+1)$ is also true.
	- **Case** $\exists k\in \mathbb{N} \ (x=k+1)$. Let $k_{0}\in \mathbb{N}$ be such that $x=k_{0}+1$. Then, $$x+1=(k_{0}+1)+1.$$Since $k_{0}\in \mathbb{N}$, by definition of $\mathbb{N}$ we also have $k_{0}+1\in \mathbb{N}$. Therefore, $\varphi(x+1)$ is also true. $\blacksquare$

***
Definitions used:
- [[Natural Numbers]]

Theorems used:
- [[Principle of Mathematical Induction]]